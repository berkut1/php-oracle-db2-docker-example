## Setting up Test Environment for OCI8 or ibm_db2 with PHP8

I spent over 3 days configuring the test environment for oci8 and ibm_db2 (the experience with db2 was particularly painful). I hope that my solution for PHP8 will help those who want to repeat this setup. This repository includes only PHP8 CLI, but if needed, you should have no trouble integrating it with Apache/nginx or FPM.

### IBM db2 important Note

After starting the container, you need to wait around 5 minutes before you can connect to DB2.

### Symfony Connection Example

```dotenv
#Oracle
DATABASE_URL="oci8://app_user:password@example-oracle:1521/FREEPDB1?serverVersion=23.3&charset=AL32UTF8&service=true"
#IBM DB2
DATABASE_URL="db2://db2inst1:password@example-db2:50000/app_db?serverVersion=11.5.0.0"
```
