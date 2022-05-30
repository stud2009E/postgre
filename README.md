# postgre
cli psql

1) Connect to PostgreSQL database
local:
psql -d database -p port -U user
remote:
psql -h host -d database -p port -U user

2) Switch connection to a new database
\c dbname username

3) List available databases
\l

4) List available tables
\dt

5) Describe a table
\d table_name

6) List available schema
\dn

7) List available functions
\df

8) List available views
\dv

9) List users and their roles
\du

10) Execute the previous command
SELECT version();

11) Command history
\s

12) Get help on psql commands
\?

13)To get help on specific PostgreSQL statement, you use the \h command.
\h ALTER TABLE

14) Turn on query execution time
dvdrental=# \timing
Timing is on.
dvdrental=# select count(*) from film;
 count
-------
  1000
(1 row)

Time: 1.495 ms
dvdrental=#

15) Edit command in your own editor
\e
\ef [function name]

16) Switch output options
 \a command switches from aligned to non-aligned column output.
 \H command formats the output to HTML format.
 
 17) Quit psql
\q
