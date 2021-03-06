
## Redis Server on macOS


What is Redis?

	Redis is an open source (BSD licensed), in-memory data structure store, 
	used as a database, cache and message broker. It supports data structures such as 
	strings, hashes, lists, sets, sorted sets with range queries, bitmaps, hyperloglogs, 
	geospatial indexes with radius queries and streams. Redis has built-in replication, 
	Lua scripting, LRU eviction, transactions and different levels of on-disk 
	persistence, and provides high availability via Redis Sentinel and automatic 
	partitioning with Redis Cluster. Learn more https://redis.io/topics/introduction


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
	
	
## Redis Desktop Manager as Client

### What is Redis Desktop Manager

	Redis Desktop Manager (aka RDM) — is a fast Redis database management application for Windows, Linux, MacOS and iPadOS.

### Download and Install Redis Desktop Manager

	Step 1: Download redis-desktop-manager-2019.5.181.dmg  from  https://redisdesktop.com/subscriptions
	
	Step 2: Install redis-desktop-manager-2019.5.181.dmg
	
	Step 3: After installation, open Redis Desktop Manager
	
	Step 4: Click on 'Connect to Redis Server'
	
	Step 5: Enter following Redis Server Connection Settings
			- Connection Name
			- Redis Server IP (default: 127.0.0.1)
			- Redis Server Port (default: 6379)
			- Enter SSL, SSL Tunnel and other necessary details
			
	Step 6: Test Connection and click 'OK'
	
	Step 7: Left side click on the 'Connection Name' to extend and check the Keys & Values
	

## Refer following GitHub project for Java Client to connect with Redis Server

	https://github.com/rahamath18/Redis-Jedis-Java-Client-Example


## Note:

The MSOpenTech-Redis project is no longer being actively maintained. If you are looking for a Windows version of Redis, you may want to check out Memurai. Please note that Microsoft is not officially endorsing this product in any way. More details in https://github.com/microsoftarchive/redis

To install & setup Redis Server on Windows 10 https://redislabs.com/blog/redis-on-windows-10

To install & setup Redis Server on macOS & Linux https://redis.io/download

Also, you may install & setup Redis Server on Linux via the package manager

For quick Redis Server Installation & Setup Guide for macOS https://github.com/rahamath18/Redis-on-MacOS
	
