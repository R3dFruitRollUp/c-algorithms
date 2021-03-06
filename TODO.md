# TODO

* Implement AES CTR mode
* Add algorithms: crypto: RSA, EC (see https://github.com/afiskon/c-elliptic-curves-crypto ), DH, Random/Entropy (see pgcrypto) + utils: crc32, adler32, crc64
* Add BSD/MIT-licensed compression algoritms, including pglz
* Refactor rbtree
	* Never override existing RB-tree nodes (see rbtree.c:593)
	* Write a test: make sure that changing walk direction from left-right to right-left works well
	* Implement search by part of the key: find\_by\_partial\_key\_march(rb, rb\_comparator, void\* arg)
* Add AVL trees
* Add skip lists, see:
	* https://github.com/begeekmyfriend/skiplist/blob/master/skiplist.h
	* https://github.com/antirez/redis/blob/unstable/src/t\_zset.c
* Add LRU/LFU cache examples, see http://antirez.com/news/109
* Add array-bases queue implementation (fifo)
* Add in-memory B-tree implementation (See tarantool?)
* Add scapegoat tree implementation https://github.com/delamonpansie/octopus/blob/master/third\_party/sptree.h#L331
* From time to time recheck code using Clang Static Analyzer, PVS-Studio, CppCheck, MemorySanitizer
