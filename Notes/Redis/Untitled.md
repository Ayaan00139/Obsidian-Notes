1. It Redis Is a type of no sql data base but is diff from other no sql data base, it is diff entirely diff from mongo db or my sql.

2. Stores Data In Key Value Pair 

	![[Pasted image 20261020175118.png]]


3. Not Good At storing structured data but is good at storing individual key value pair 

4. Redis works on memory / ram unlike other databases which run on disk/storage

5. It is not used as a actual persistent database cause you might lose everything in redis unless we are backing it up consistently that is why it is used for caching.

6. Redis is built on the top of a persistent database like mongo db.

7. To install use homebrew on mac, package manager on linux and using windows subsystem/wsl to run linux on windows.

8. To actually use redis we have to type redis-server in one terminal and redis-cli to another to use it

9. To actually enter the data in the databse we use "Set {key} {value}" and the value/key is always stored as a string, to check if a key exist, use EXISTS {key}

10. To see all the keys use: Keys *  , To del all use: FLUSHALL

11. TTL Stands for time to live which is basically a countdown when a key expires, normal kyes live forever but key with "expire name 10" or "setex name 10 ayaan" will expire after 10 secs

	![[Pasted image 20261020202019.png]]
	

12. Get and set basically works for strings, if we have to make an array we use LPUSH- "will basically add a item to the left of the array" or RPUSH-"will add a item to the right of the array".

	![[Pasted image 20261020202310.png]]


13. Can use lpop and r pop to basically remove a item from the array, lpop will remove left and rpop with remove right

	![[Pasted image 20261020202436.png]]

14. SETS:

	![[Pasted image 20261020202705.png]]


15. HASHES: we can set multiple key values for one key by hashes 

	![[Pasted image 20261020204844.png]]

16. after importing redis, it basically becomes a class that we can use;