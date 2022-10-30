# 数据存储加密

iOS的app的本地端，一般都会涉及到存储很多数据，其中有些可能是敏感数据。

其中一种增加iOS的app的安全的做法是：把本地保存的数据加密。

* iOS端本地的数据库
  * 常用：SQLite
    * SQLite加密：增加破解难度
      * SQLCipher
        * https://github.com/sqlcipher/sqlcipher
