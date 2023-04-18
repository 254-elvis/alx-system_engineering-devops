Project Description.
Learn what is the main role of a database. What is a database replica. What is the purpose of a database replica. Why database backups need to be stored in different physical locations. What operation should you regularly perform to make sure that your database backup strategy actually works.

0. Install MySQL - Install mySQL on both your web-01 and web-02 servers. MySQL distribution must be 5.7.x.
1. Let us in! - Create a user and password for both MySQL databases which will allow the checker access to them.
2. If only you could see what I've seen with your eyes - In order for you to set up replication, you’ll need to have a database with at least one table and one row in your primary MySQL server (web-01) to replicate from.
3. Quite an experience to live in fear, isn't it? - On your primary MySQL server (web-01), create a new user for the replica server.
4. Setup a Primary-Replica infrastructure using MySQL - Primary must be hosted on web-01 - do not use the bind-address, just comment out this parameter. MySQL replica must be hosted on web-02.
5. MySQL backup - Write a Bash script that generates a MySQL dump and creates a compressed archive out of it. - 5-mysql_backup.
