# TABLEDUMP

Dump only the database tables with a given prefix from a MySQL database.

This is useful if you have a database with a large number of different WordPress, Omeka, or other type applications installed. Each of those installs would have a different table prefix (like wp_, or omeka_). This will do a mysqldump for just those tables, rather than needing to dump the whole database.

The port (DBPORT) and host (DBHOST) for the database are hard coded in the script, so change these as needed. The default uses settings for MAMP on Mac OSX.

Some common examples:

- MAMP on Mac OSX

  DBPORT=8889
  DBHOST=localhost

- Many default LAMP servers
  
  DBPORT=3306
  DBHOST=localhost


# How To Use

- Copy the script to any directory.
- Set the execute bit

  ```
  chmod u+x tabledump
  ```

- Edit the DBPORT and DBHOST variables if needed
- Run like so:
  
  ```
  ./tabledump
  ```

The script will prompt for the database name, the prefix, the database username and the password (twice).
