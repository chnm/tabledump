= TABLEDUMP

Dump only the database tables with a given prefix from a MySQL database.

This is useful if you have a database with a large number of different WordPress, Omeka, or other type applications installed. Each of those installs would have a different table prefix (like wp_, or omeka_). This will do a mysqldump for just those tables, rather than needing to dump the whole database.
