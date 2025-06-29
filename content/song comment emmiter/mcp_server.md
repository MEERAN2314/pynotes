---
title: Mcp Server
date: 2025-06-30
author: Your Name
cell_count: 2
score: 0
---

```python
from flask import Flask, request, jsonify
from flask_cors import CORS
from pymongo import MongoClient
from dotenv import load_dotenv
import os

load_dotenv()

app = Flask(__name__)
CORS(app)

# MongoDB connection
client = MongoClient(
    os.getenv("MONGODB_URI"),
    serverSelectionTimeoutMS=5000,  # 5 second timeout
    socketTimeoutMS=30000,  # 30 second socket timeout
    connectTimeoutMS=30000  # 30 second connection timeout
)
db = client[os.getenv("DB_NAME")]
comments_collection = db['song_comments']

@app.route('/store_comments', methods=['POST'])
def store_comments():
    data = request.json
    try:
        result = comments_collection.insert_many(data['comments'])
        return jsonify({
            "status": "success",
            "inserted_ids": len(result.inserted_ids)
        }), 200
    except Exception as e:
        return jsonify({
            "status": "error",
            "message": str(e)
        }), 500

@app.route('/get_comments', methods=['GET'])
def get_comments():
    try:
        song_id = request.args.get('song_id')
        limit = int(request.args.get('limit', 10))
        sort_by = request.args.get('sort_by', 'rating')
        
        query = {"song_id": song_id}
        comments = list(comments_collection.find(query, {'_id': 0}))
        
        # Sort comments
        if sort_by == 'rating':
            comments.sort(key=lambda x: x['rating'], reverse=True)
        elif sort_by == 'positive':
            comments.sort(key=lambda x: x['sentiment'], reverse=True)
        elif sort_by == 'negative':
            comments.sort(key=lambda x: x['sentiment'])
        
        return jsonify({
            "status": "success",
            "comments": comments[:limit]
        }), 200
    except Exception as e:
        return jsonify({
            "status": "error",
            "message": str(e)
        }), 500

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[6], line 19
         12 # MongoDB connection
         13 client = MongoClient(
         14     os.getenv("MONGODB_URI"),
         15     serverSelectionTimeoutMS=5000,  # 5 second timeout
         16     socketTimeoutMS=30000,  # 30 second socket timeout
         17     connectTimeoutMS=30000  # 30 second connection timeout
         18 )
    ---> 19 db = client[os.getenv("DB_NAME")]
         20 comments_collection = db['song_comments']
         22 @app.route('/store_comments', methods=['POST'])
         23 def store_comments():


    File ~/miniconda3/envs/py312/lib/python3.12/site-packages/pymongo/mongo_client.py:1597, in MongoClient.__getitem__(self, name)
       1588 def __getitem__(self, name: str) -> database.Database[_DocumentType]:
       1589     """Get a database by name.
       1590 
       1591     Raises :class:`~pymongo.errors.InvalidName` if an invalid
       (...)
       1595       - `name`: the name of the database to get
       1596     """
    -> 1597     return database.Database(self, name)


    File ~/miniconda3/envs/py312/lib/python3.12/site-packages/pymongo/database.py:137, in Database.__init__(self, client, name, codec_options, read_preference, write_concern, read_concern)
        129 super().__init__(
        130     codec_options or client.codec_options,
        131     read_preference or client.read_preference,
        132     write_concern or client.write_concern,
        133     read_concern or client.read_concern,
        134 )
        136 if not isinstance(name, str):
    --> 137     raise TypeError("name must be an instance of str")
        139 if name != "$external":
        140     _check_name(name)


    TypeError: name must be an instance of str



```python

```


---
**Score: 0**