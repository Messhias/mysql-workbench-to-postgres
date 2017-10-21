# mysql-workbench-to-postgres

Converts a MySQL Workbench SQL export into a PostgreSQL compatible SQL script.

> Copyright (C) 2011 by Aevum Softwares LTDA ME under GNU General Public License

> Original source code from https://code.google.com/p/mysql-workbench-to-postgres/

> Some corrections by Oscar Fonts, 2015

> Some more corrections by Gus Antoniassi, 2017

## Usage

* Use the MySQL Workbench "File" > "Export" > "Forward Engineer SQL CREATE script..." option to generate a MySQL SQL script.
* Run the exporter command to translate the SQL script to a PostgreSQL compatible one, like this:

```
    ./exporter.py input.sql [output.sql]
```
* If you omit the output file, a file with `_postgre` will be created
* You can change the schema name using `-s` or `--schema`, like this:
```
    ./exporter.py input.sql --schema public
```

## Disclaimer

This project is not thoroughly tested, contributions are welcome.

Last tested on MySQL Workbench v.6.2 (Oct 2015).
