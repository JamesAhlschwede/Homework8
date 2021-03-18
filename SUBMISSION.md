
[DockerFile](Dockerfile)

Your running docker instance as shown by a ps command.
(running-instance.png?raw=true)

[Homepage](homepage.png?raw=true)

The output from docker-compose up

Creating network "spring-petclinic_default" with the default driver
Pulling mysql (mysql:5.7)...
5.7: Pulling from library/mysql
6f28985ad184: Pull complete
e7cd18945cf6: Pull complete
ee91068b9313: Pull complete
b4efa1a4f93b: Pull complete
f220edfa5893: Pull complete
74a27d3460f8: Pull complete
2e11e23b7542: Pull complete
39ac93d44c47: Pull complete
dfd9db50d4ea: Pull complete
a0699264f539: Pull complete
eaf3d09f5acb: Pull complete
Digest: sha256:bb536013c16d12152ebc956cac9ef26cde46fb8f2ca2af488629161b7bed678b
Status: Downloaded newer image for mysql:5.7
Creating spring-petclinic_mysql_1 ... done
Attaching to spring-petclinic_mysql_1
mysql_1  | 2021-03-18 01:39:57+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.33-1debian10 started.
mysql_1  | 2021-03-18 01:39:57+00:00 [Note] [Entrypoint]: Switching to dedicated user 'mysql'
mysql_1  | 2021-03-18 01:39:57+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.33-1debian10 started.
mysql_1  | 2021-03-18 01:39:57+00:00 [Note] [Entrypoint]: Initializing database files
mysql_1  | 2021-03-18T01:39:57.871566Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
mysql_1  | 2021-03-18T01:39:57.882216Z 0 [Warning] Setting lower_case_table_names=2 because file system for /var/lib/mysql/ is case insensitive
mysql_1  | 2021-03-18T01:39:59.724427Z 0 [Warning] InnoDB: New log files created, LSN=45790
mysql_1  | 2021-03-18T01:40:00.125874Z 0 [Warning] InnoDB: Creating foreign key constraint system tables.
mysql_1  | 2021-03-18T01:40:00.166930Z 0 [Warning] No existing UUID has been found, so we assume that this is the first time that this server has been started. Generating a new UUID: da3e0a1d-878a-11eb-8e15-0242ac120002.
mysql_1  | 2021-03-18T01:40:00.185563Z 0 [Warning] Gtid table is not ready to be used. Table 'mysql.gtid_executed' cannot be opened.
mysql_1  | 2021-03-18T01:40:01.154275Z 0 [Warning] CA certificate ca.pem is self signed.
mysql_1  | 2021-03-18T01:40:01.321992Z 1 [Warning] root@localhost is created with an empty password ! Please consider switching off the --initialize-insecure option.
mysql_1  | 2021-03-18 01:40:14+00:00 [Note] [Entrypoint]: Database files initialized
mysql_1  | 2021-03-18 01:40:14+00:00 [Note] [Entrypoint]: Starting temporary server
mysql_1  | 2021-03-18 01:40:14+00:00 [Note] [Entrypoint]: Waiting for server startup
mysql_1  | 2021-03-18T01:40:14.245616Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
mysql_1  | 2021-03-18T01:40:14.255645Z 0 [Note] mysqld (mysqld 5.7.33) starting as process 78 ...
mysql_1  | 2021-03-18T01:40:14.264185Z 0 [Warning] Setting lower_case_table_names=2 because file system for /var/lib/mysql/ is case insensitive
mysql_1  | 2021-03-18T01:40:14.265895Z 0 [Note] InnoDB: PUNCH HOLE support available
mysql_1  | 2021-03-18T01:40:14.265924Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
mysql_1  | 2021-03-18T01:40:14.265937Z 0 [Note] InnoDB: Uses event mutexes
mysql_1  | 2021-03-18T01:40:14.265950Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
mysql_1  | 2021-03-18T01:40:14.265963Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
mysql_1  | 2021-03-18T01:40:14.266156Z 0 [Note] InnoDB: Number of pools: 1
mysql_1  | 2021-03-18T01:40:14.266261Z 0 [Note] InnoDB: Using CPU crc32 instructions
mysql_1  | 2021-03-18T01:40:14.267436Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
mysql_1  | 2021-03-18T01:40:14.275563Z 0 [Note] InnoDB: Completed initialization of buffer pool
mysql_1  | 2021-03-18T01:40:14.279895Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
mysql_1  | 2021-03-18T01:40:14.361144Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
mysql_1  | 2021-03-18T01:40:14.530299Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
mysql_1  | 2021-03-18T01:40:14.534834Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
mysql_1  | 2021-03-18T01:40:14.690121Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
mysql_1  | 2021-03-18T01:40:14.708668Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
mysql_1  | 2021-03-18T01:40:14.708718Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
mysql_1  | 2021-03-18T01:40:14.709415Z 0 [Note] InnoDB: Waiting for purge to start
mysql_1  | 2021-03-18T01:40:14.759811Z 0 [Note] InnoDB: 5.7.33 started; log sequence number 2747895
mysql_1  | 2021-03-18T01:40:14.760260Z 0 [Note] Plugin 'FEDERATED' is disabled.
mysql_1  | 2021-03-18T01:40:14.760497Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
mysql_1  | 2021-03-18T01:40:14.866906Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
mysql_1  | 2021-03-18T01:40:14.866945Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
mysql_1  | 2021-03-18T01:40:14.882184Z 0 [Warning] CA certificate ca.pem is self signed.
mysql_1  | 2021-03-18T01:40:14.882264Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
mysql_1  | 2021-03-18T01:40:14.892045Z 0 [Note] InnoDB: Buffer pool(s) load completed at 210318  1:40:14
mysql_1  | 2021-03-18T01:40:14.895728Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
mysql_1  | 2021-03-18T01:40:15.414289Z 0 [Note] Event Scheduler: Loaded 0 events
mysql_1  | 2021-03-18T01:40:15.414766Z 0 [Note] mysqld: ready for connections.
mysql_1  | Version: '5.7.33'  socket: '/var/run/mysqld/mysqld.sock'  port: 0  MySQL Community Server (GPL)
mysql_1  | 2021-03-18 01:40:15+00:00 [Note] [Entrypoint]: Temporary server started.
mysql_1  | Warning: Unable to load '/usr/share/zoneinfo/iso3166.tab' as time zone. Skipping it.
mysql_1  | Warning: Unable to load '/usr/share/zoneinfo/leap-seconds.list' as time zone. Skipping it.
mysql_1  | Warning: Unable to load '/usr/share/zoneinfo/zone.tab' as time zone. Skipping it.
mysql_1  | Warning: Unable to load '/usr/share/zoneinfo/zone1970.tab' as time zone. Skipping it.
mysql_1  | 2021-03-18 01:40:19+00:00 [Note] [Entrypoint]: Creating database petclinic
mysql_1  | 2021-03-18 01:40:19+00:00 [Note] [Entrypoint]: Creating user petclinic
mysql_1  | 2021-03-18 01:40:19+00:00 [Note] [Entrypoint]: Giving user petclinic access to schema petclinic
mysql_1  | 
mysql_1  | 2021-03-18 01:40:20+00:00 [Note] [Entrypoint]: Stopping temporary server
mysql_1  | 2021-03-18T01:40:20.020787Z 0 [Note] Giving 0 client threads a chance to die gracefully
mysql_1  | 2021-03-18T01:40:20.021514Z 0 [Note] Shutting down slave threads
mysql_1  | 2021-03-18T01:40:20.021974Z 0 [Note] Forcefully disconnecting 0 remaining clients
mysql_1  | 2021-03-18T01:40:20.022385Z 0 [Note] Event Scheduler: Purging the queue. 0 events
mysql_1  | 2021-03-18T01:40:20.022867Z 0 [Note] Binlog end
mysql_1  | 2021-03-18T01:40:20.032687Z 0 [Note] Shutting down plugin 'ngram'
mysql_1  | 2021-03-18T01:40:20.032719Z 0 [Note] Shutting down plugin 'partition'
mysql_1  | 2021-03-18T01:40:20.032731Z 0 [Note] Shutting down plugin 'BLACKHOLE'
mysql_1  | 2021-03-18T01:40:20.032739Z 0 [Note] Shutting down plugin 'ARCHIVE'
mysql_1  | 2021-03-18T01:40:20.032760Z 0 [Note] Shutting down plugin 'PERFORMANCE_SCHEMA'
mysql_1  | 2021-03-18T01:40:20.032789Z 0 [Note] Shutting down plugin 'MRG_MYISAM'
mysql_1  | 2021-03-18T01:40:20.032801Z 0 [Note] Shutting down plugin 'MyISAM'
mysql_1  | 2021-03-18T01:40:20.032811Z 0 [Note] Shutting down plugin 'INNODB_SYS_VIRTUAL'
mysql_1  | 2021-03-18T01:40:20.032834Z 0 [Note] Shutting down plugin 'INNODB_SYS_DATAFILES'
mysql_1  | 2021-03-18T01:40:20.032843Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLESPACES'
mysql_1  | 2021-03-18T01:40:20.032850Z 0 [Note] Shutting down plugin 'INNODB_SYS_FOREIGN_COLS'
mysql_1  | 2021-03-18T01:40:20.032860Z 0 [Note] Shutting down plugin 'INNODB_SYS_FOREIGN'
mysql_1  | 2021-03-18T01:40:20.032880Z 0 [Note] Shutting down plugin 'INNODB_SYS_FIELDS'
mysql_1  | 2021-03-18T01:40:20.032915Z 0 [Note] Shutting down plugin 'INNODB_SYS_COLUMNS'
mysql_1  | 2021-03-18T01:40:20.032929Z 0 [Note] Shutting down plugin 'INNODB_SYS_INDEXES'
mysql_1  | 2021-03-18T01:40:20.033018Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLESTATS'
mysql_1  | 2021-03-18T01:40:20.033029Z 0 [Note] Shutting down plugin 'INNODB_SYS_TABLES'
mysql_1  | 2021-03-18T01:40:20.033048Z 0 [Note] Shutting down plugin 'INNODB_FT_INDEX_TABLE'
mysql_1  | 2021-03-18T01:40:20.033055Z 0 [Note] Shutting down plugin 'INNODB_FT_INDEX_CACHE'
mysql_1  | 2021-03-18T01:40:20.033062Z 0 [Note] Shutting down plugin 'INNODB_FT_CONFIG'
mysql_1  | 2021-03-18T01:40:20.033068Z 0 [Note] Shutting down plugin 'INNODB_FT_BEING_DELETED'
mysql_1  | 2021-03-18T01:40:20.033084Z 0 [Note] Shutting down plugin 'INNODB_FT_DELETED'
mysql_1  | 2021-03-18T01:40:20.033172Z 0 [Note] Shutting down plugin 'INNODB_FT_DEFAULT_STOPWORD'
mysql_1  | 2021-03-18T01:40:20.033190Z 0 [Note] Shutting down plugin 'INNODB_METRICS'
mysql_1  | 2021-03-18T01:40:20.033197Z 0 [Note] Shutting down plugin 'INNODB_TEMP_TABLE_INFO'
mysql_1  | 2021-03-18T01:40:20.033203Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_POOL_STATS'
mysql_1  | 2021-03-18T01:40:20.033211Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_PAGE_LRU'
mysql_1  | 2021-03-18T01:40:20.033218Z 0 [Note] Shutting down plugin 'INNODB_BUFFER_PAGE'
mysql_1  | 2021-03-18T01:40:20.033226Z 0 [Note] Shutting down plugin 'INNODB_CMP_PER_INDEX_RESET'
mysql_1  | 2021-03-18T01:40:20.033329Z 0 [Note] Shutting down plugin 'INNODB_CMP_PER_INDEX'
mysql_1  | 2021-03-18T01:40:20.033340Z 0 [Note] Shutting down plugin 'INNODB_CMPMEM_RESET'
mysql_1  | 2021-03-18T01:40:20.033350Z 0 [Note] Shutting down plugin 'INNODB_CMPMEM'
mysql_1  | 2021-03-18T01:40:20.033361Z 0 [Note] Shutting down plugin 'INNODB_CMP_RESET'
mysql_1  | 2021-03-18T01:40:20.033372Z 0 [Note] Shutting down plugin 'INNODB_CMP'
mysql_1  | 2021-03-18T01:40:20.033382Z 0 [Note] Shutting down plugin 'INNODB_LOCK_WAITS'
mysql_1  | 2021-03-18T01:40:20.033390Z 0 [Note] Shutting down plugin 'INNODB_LOCKS'
mysql_1  | 2021-03-18T01:40:20.033470Z 0 [Note] Shutting down plugin 'INNODB_TRX'
mysql_1  | 2021-03-18T01:40:20.033486Z 0 [Note] Shutting down plugin 'InnoDB'
mysql_1  | 2021-03-18T01:40:20.033659Z 0 [Note] InnoDB: FTS optimize thread exiting.
mysql_1  | 2021-03-18T01:40:20.033930Z 0 [Note] InnoDB: Starting shutdown...
mysql_1  | 2021-03-18T01:40:20.136013Z 0 [Note] InnoDB: Dumping buffer pool(s) to /var/lib/mysql/ib_buffer_pool
mysql_1  | 2021-03-18T01:40:20.143193Z 0 [Note] InnoDB: Buffer pool(s) dump completed at 210318  1:40:20
mysql_1  | 2021-03-18T01:40:21.562502Z 0 [Note] InnoDB: Shutdown completed; log sequence number 12665509
mysql_1  | 2021-03-18T01:40:21.566955Z 0 [Note] InnoDB: Removed temporary tablespace data file: "ibtmp1"
mysql_1  | 2021-03-18T01:40:21.567011Z 0 [Note] Shutting down plugin 'MEMORY'
mysql_1  | 2021-03-18T01:40:21.567024Z 0 [Note] Shutting down plugin 'CSV'
mysql_1  | 2021-03-18T01:40:21.567035Z 0 [Note] Shutting down plugin 'sha256_password'
mysql_1  | 2021-03-18T01:40:21.567043Z 0 [Note] Shutting down plugin 'mysql_native_password'
mysql_1  | 2021-03-18T01:40:21.567200Z 0 [Note] Shutting down plugin 'binlog'
mysql_1  | 2021-03-18T01:40:21.570841Z 0 [Note] mysqld: Shutdown complete
mysql_1  | 
mysql_1  | 2021-03-18 01:40:22+00:00 [Note] [Entrypoint]: Temporary server stopped
mysql_1  | 
mysql_1  | 2021-03-18 01:40:22+00:00 [Note] [Entrypoint]: MySQL init process done. Ready for start up.
mysql_1  | 
mysql_1  | 2021-03-18T01:40:22.200274Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
mysql_1  | 2021-03-18T01:40:22.209484Z 0 [Note] mysqld (mysqld 5.7.33) starting as process 1 ...
mysql_1  | 2021-03-18T01:40:22.218435Z 0 [Warning] Setting lower_case_table_names=2 because file system for /var/lib/mysql/ is case insensitive
mysql_1  | 2021-03-18T01:40:22.220325Z 0 [Note] InnoDB: PUNCH HOLE support available
mysql_1  | 2021-03-18T01:40:22.220371Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
mysql_1  | 2021-03-18T01:40:22.220378Z 0 [Note] InnoDB: Uses event mutexes
mysql_1  | 2021-03-18T01:40:22.220384Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
mysql_1  | 2021-03-18T01:40:22.220392Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
mysql_1  | 2021-03-18T01:40:22.220674Z 0 [Note] InnoDB: Number of pools: 1
mysql_1  | 2021-03-18T01:40:22.220804Z 0 [Note] InnoDB: Using CPU crc32 instructions
mysql_1  | 2021-03-18T01:40:22.223040Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
mysql_1  | 2021-03-18T01:40:22.231533Z 0 [Note] InnoDB: Completed initialization of buffer pool
mysql_1  | 2021-03-18T01:40:22.234747Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
mysql_1  | 2021-03-18T01:40:22.317899Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
mysql_1  | 2021-03-18T01:40:22.440975Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
mysql_1  | 2021-03-18T01:40:22.444984Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
mysql_1  | 2021-03-18T01:40:22.638116Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
mysql_1  | 2021-03-18T01:40:22.643720Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
mysql_1  | 2021-03-18T01:40:22.643892Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
mysql_1  | 2021-03-18T01:40:22.644752Z 0 [Note] InnoDB: Waiting for purge to start
mysql_1  | 2021-03-18T01:40:22.695271Z 0 [Note] InnoDB: 5.7.33 started; log sequence number 12665509
mysql_1  | 2021-03-18T01:40:22.695743Z 0 [Note] Plugin 'FEDERATED' is disabled.
mysql_1  | 2021-03-18T01:40:22.695965Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
mysql_1  | 2021-03-18T01:40:22.738585Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
mysql_1  | 2021-03-18T01:40:22.738615Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
mysql_1  | 2021-03-18T01:40:22.747112Z 0 [Warning] CA certificate ca.pem is self signed.
mysql_1  | 2021-03-18T01:40:22.747211Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
mysql_1  | 2021-03-18T01:40:22.752449Z 0 [Note] Server hostname (bind-address): '*'; port: 3306
mysql_1  | 2021-03-18T01:40:22.752690Z 0 [Note] IPv6 is available.
mysql_1  | 2021-03-18T01:40:22.752736Z 0 [Note]   - '::' resolves to '::';
mysql_1  | 2021-03-18T01:40:22.752840Z 0 [Note] Server socket created on IP: '::'.
mysql_1  | 2021-03-18T01:40:22.755993Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
mysql_1  | 2021-03-18T01:40:22.880105Z 0 [Note] InnoDB: Buffer pool(s) load completed at 210318  1:40:22
mysql_1  | 2021-03-18T01:40:23.174177Z 0 [Note] Event Scheduler: Loaded 0 events
mysql_1  | 2021-03-18T01:40:23.174749Z 0 [Note] mysqld: ready for connections.
mysql_1  | Version: '5.7.33'  socket: '/var/run/mysqld/mysqld.sock'  port: 3306  MySQL Community Server (GPL)

Image of Veternarians running locally
![Vets](vets.png?raw=true "Local")

[docker-compose.yml](docker-compose.yml)

[application-mysql.properties](application-mysql.properties)


Output from Docker Compoose Up

(base) james@Jamess-iMac spring-petclinic % docker-compose up
Starting spring-petclinic_mysql_1 ... done
Attaching to spring-petclinic_mysql_1
mysql_1  | 2021-03-18 01:51:49+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.33-1debian10 started.
mysql_1  | 2021-03-18 01:51:53+00:00 [Note] [Entrypoint]: Switching to dedicated user 'mysql'
mysql_1  | 2021-03-18 01:51:53+00:00 [Note] [Entrypoint]: Entrypoint script for MySQL Server 5.7.33-1debian10 started.
mysql_1  | 2021-03-18T01:51:54.260518Z 0 [Warning] TIMESTAMP with implicit DEFAULT value is deprecated. Please use --explicit_defaults_for_timestamp server option (see documentation for more details).
mysql_1  | 2021-03-18T01:51:54.280568Z 0 [Note] mysqld (mysqld 5.7.33) starting as process 1 ...
mysql_1  | 2021-03-18T01:51:54.311408Z 0 [Warning] Setting lower_case_table_names=2 because file system for /var/lib/mysql/ is case insensitive
mysql_1  | 2021-03-18T01:51:54.316082Z 0 [Note] InnoDB: PUNCH HOLE support available
mysql_1  | 2021-03-18T01:51:54.316123Z 0 [Note] InnoDB: Mutexes and rw_locks use GCC atomic builtins
mysql_1  | 2021-03-18T01:51:54.316136Z 0 [Note] InnoDB: Uses event mutexes
mysql_1  | 2021-03-18T01:51:54.316148Z 0 [Note] InnoDB: GCC builtin __atomic_thread_fence() is used for memory barrier
mysql_1  | 2021-03-18T01:51:54.316161Z 0 [Note] InnoDB: Compressed tables use zlib 1.2.11
mysql_1  | 2021-03-18T01:51:54.316354Z 0 [Note] InnoDB: Number of pools: 1
mysql_1  | 2021-03-18T01:51:54.316528Z 0 [Note] InnoDB: Using CPU crc32 instructions
mysql_1  | 2021-03-18T01:51:54.318460Z 0 [Note] InnoDB: Initializing buffer pool, total size = 128M, instances = 1, chunk size = 128M
mysql_1  | 2021-03-18T01:51:54.335943Z 0 [Note] InnoDB: Completed initialization of buffer pool
mysql_1  | 2021-03-18T01:51:54.340892Z 0 [Note] InnoDB: If the mysqld execution user is authorized, page cleaner thread priority can be changed. See the man page of setpriority().
mysql_1  | 2021-03-18T01:51:54.507737Z 0 [Note] InnoDB: Highest supported file format is Barracuda.
mysql_1  | 2021-03-18T01:51:54.685724Z 0 [Note] InnoDB: Creating shared tablespace for temporary tables
mysql_1  | 2021-03-18T01:51:54.690428Z 0 [Note] InnoDB: Setting file './ibtmp1' size to 12 MB. Physically writing the file full; Please wait ...
mysql_1  | 2021-03-18T01:51:54.922581Z 0 [Note] InnoDB: File './ibtmp1' size is now 12 MB.
mysql_1  | 2021-03-18T01:51:54.935573Z 0 [Note] InnoDB: 96 redo rollback segment(s) found. 96 redo rollback segment(s) are active.
mysql_1  | 2021-03-18T01:51:54.935599Z 0 [Note] InnoDB: 32 non-redo rollback segment(s) are active.
mysql_1  | 2021-03-18T01:51:54.940426Z 0 [Note] InnoDB: 5.7.33 started; log sequence number 12665537
mysql_1  | 2021-03-18T01:51:54.941579Z 0 [Note] Plugin 'FEDERATED' is disabled.
mysql_1  | 2021-03-18T01:51:54.943840Z 0 [Note] InnoDB: Loading buffer pool(s) from /var/lib/mysql/ib_buffer_pool
mysql_1  | 2021-03-18T01:51:55.144635Z 0 [Note] Found ca.pem, server-cert.pem and server-key.pem in data directory. Trying to enable SSL support using them.
mysql_1  | 2021-03-18T01:51:55.144663Z 0 [Note] Skipping generation of SSL certificates as certificate files are present in data directory.
mysql_1  | 2021-03-18T01:51:55.196304Z 0 [Warning] CA certificate ca.pem is self signed.
mysql_1  | 2021-03-18T01:51:55.196389Z 0 [Note] Skipping generation of RSA key pair as key files are present in data directory.
mysql_1  | 2021-03-18T01:51:55.218395Z 0 [Note] Server hostname (bind-address): '*'; port: 3306
mysql_1  | 2021-03-18T01:51:55.218448Z 0 [Note] IPv6 is available.
mysql_1  | 2021-03-18T01:51:55.218465Z 0 [Note]   - '::' resolves to '::';
mysql_1  | 2021-03-18T01:51:55.218485Z 0 [Note] Server socket created on IP: '::'.
mysql_1  | 2021-03-18T01:51:55.254639Z 0 [Note] InnoDB: Buffer pool(s) load completed at 210318  1:51:55
mysql_1  | 2021-03-18T01:51:55.271411Z 0 [Warning] Insecure configuration for --pid-file: Location '/var/run/mysqld' in the path is accessible to all OS users. Consider choosing a different directory.
mysql_1  | 2021-03-18T01:51:56.140311Z 0 [Note] Event Scheduler: Loaded 0 events
mysql_1  | 2021-03-18T01:51:56.140688Z 0 [Note] mysqld: ready for connections.
mysql_1  | Version: '5.7.33'  socket: '/var/run/mysqld/mysqld.sock'  port: 3306  MySQL Community Server (GPL)
^CGracefully stopping... (press Ctrl+C again to force)
Stopping spring-petclinic_mysql_1 ... done
(base) james@Jamess-iMac spring-petclinic % docker-compose up
Pulling webapp (se441/spring-petclinic:both)...
ERROR: The image for the service you're trying to recreate has been removed. If you continue, volume data could be lost. Consider backing up your data before continuing.

Continue with the new image? [yN]N
ERROR: pull access denied for se441/spring-petclinic, repository does not exist or may require 'docker login': denied: requested access to the resource is denied



