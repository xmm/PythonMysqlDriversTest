PythonMysqlDriversTest
======================

Python Mysql Drivers Benchmark

##  Compare python mysql drivers
* Python version: 2.7.5+ (default, Feb 27 2014, 19:37:08) 
[GCC 4.8.1] 
* Platform: Linux-3.11.0-18-generic-x86_64-with-Ubuntu-13.10-saucy 
* Database: https://launchpad.net/test-db 1.0.6
* MySQLdb version: 1.2.5 url:https://github.com/farcepest/MySQLdb1
* mysql.connector version: 1.1.6 url:http://dev.mysql.com/downloads/connector/python/
* oursql version: 0.9.3.1 url:https://launchpad.net/oursql
* pymysql version: 0.6.1.None url:https://github.com/petehunt/PyMySQL
* sqlalchemy version: 0.9.3 url:http://www.sqlalchemy.org

###  Simple Select 1 record 10000x 
*  0.57119011879 MySQLdb
*  0.751263856888 oursql
*  1.3060708046 mysql.connector
*  1.68229007721 pymysql
*  1.33858585358 sqlalchemy raw

###  Select 500 rows 1000x
*  1.87236404419 MySQLdb
*  1.8126680851 oursql
*  7.15665388107 mysql.connector
*  7.47649288177 pymysql
*  2.05442595482 sqlalchemy raw

###  Select 500 rows with 500 args 1000x
*  1.25386977196 MySQLdb
*  1.20354008675 oursql
*  2.38949418068 mysql.connector
*  4.17395281792 pymysql
*  1.34546685219 sqlalchemy raw

###  Select 300k id  5x
*  0.690109014511 MySQLdb
*  0.721325874329 oursql
*  6.18549704552 mysql.connector
*  6.2363421917 pymysql
*  1.34703087807 sqlalchemy raw

###  Simple Select 1M3 id  1x
*  6.14506411552 MySQLdb
*  9.71714186668 oursql
*  58.2201230526 mysql.connector
*  59.2201881409 pymysql
*  11.5915169716 sqlalchemy raw
