
## Redis Server & Redis Client on macOS


### Download - Redis Server
	https://redis.io/download


### Installation - Redis Server
	
	To tar downloaded redis package
	-------------------------------
	$ tar xzf redis-5.0.7.tar.gz
	$ cd redis-5.0.7
	
	To compile binaries
	-------------------
	$ make
	
	Note: For 32 bit
	$ make 32bit
	
	To test compiled binaries
	-------------------------
	$ make test

### Start - Redis Server
	$ ./src/redis-server
	
### To test Redis Server connection
	$ ./src/redis-cli ping
	
	Note: Open new shell tab/windows
	
### Redis CLI built-in Client to interact with Redis Server
	$ ./src/redis-cli
	
### Set a Key & Value Pair into Redis Server through Redis CLI Client
	
	To test Redis Server connection
	127.0.0.1:6379> PING
	
	To set a value with an associated key
	127.0.0.1:6379> set dev_name "Rahamath S"
	
	To get a value with an already associated key
	127.0.0.1:6379> get dev_name
	
	
## Refer following GitHub project for Java Client to connect with Redis Server

	https://github.com/rahamath18/Redis-Java-Client-Example
	