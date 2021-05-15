Databases <br>
RDS has two features.
* Multi AZ for disaster recovery. Consist primary and secondary databases
* Read Replicas for performance. Consist primary and read replica

<br>
Read replicas can be helpful in creating reports every day without touching primary databases.

<br>
Automated Backups <br>
enabled by default, The data is stored in s3 and you get free storage space equal to the size of your database. So , if you have RDS instance of 10 gb, you will get 10Gb worth of storage. Backups are taken within defined window. During  the backup window, storage I/O may be suspended while your data is being backed up and you may experience elevated latency.

