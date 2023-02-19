# redis-workers 🎉
A tool that simplifies Redis usage for repeating tasks

## Installation

	pip install redis-workers

# Usage
`docker-compose up` to start Redis server

Give rd.cache() a key, callable and arguments.

````
    from redis_workers import redisWorker
    
    rd = redisWorker()

    games = rd.cache('games', db_app.get_table, 'games', ['game_id', 'appid'])
```
