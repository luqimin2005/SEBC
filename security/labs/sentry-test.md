The statement should return an empty set because no authorizations are in place:
```
[luqimin2005@ip-172-31-35-195 ~]$ beeline 
Beeline version 1.1.0-cdh5.9.2 by Apache Hive
beeline> !connect jdbc:hive2://ip-172-31-35-75:10000/default;principal=hive/ip-172-31-35-75@LUQIMIN2005.CN
scan complete in 3ms
Connecting to jdbc:hive2://ip-172-31-35-75:10000/default;principal=hive/ip-172-31-35-75@LUQIMIN2005.CN
Connected to: Apache Hive (version 1.1.0-cdh5.9.2)
Driver: Hive JDBC (version 1.1.0-cdh5.9.2)
Transaction isolation: TRANSACTION_REPEATABLE_READ
0: jdbc:hive2://ip-172-31-35-75:10000/default> show tables;
INFO  : Compiling command(queryId=hive_20170510102121_fbfa2401-074f-41b3-95ee-4aaff590c038): show tables
INFO  : Semantic Analysis Completed
INFO  : Returning Hive schema: Schema(fieldSchemas:[FieldSchema(name:tab_name, type:string, comment:from deserializer)], properties:null)
INFO  : Completed compiling command(queryId=hive_20170510102121_fbfa2401-074f-41b3-95ee-4aaff590c038); Time taken: 0.709 seconds
INFO  : Executing command(queryId=hive_20170510102121_fbfa2401-074f-41b3-95ee-4aaff590c038): show tables
INFO  : Starting task [Stage-0:DDL] in serial mode
INFO  : Completed executing command(queryId=hive_20170510102121_fbfa2401-074f-41b3-95ee-4aaff590c038); Time taken: 0.255 seconds
INFO  : OK
+-----------+--+
| tab_name  |
+-----------+--+
+-----------+--+
No rows selected (2.353 seconds)

```
