## To start the project locally 
```sh
npm install
node index.js repl
```

## Database Commands

#### using [database name]

Either loads a database from the directory you are currently in or creates a database with the specified name if none exists

Example: using test

#### create [table name] [columns names]

creates a new table in the database with the specified columns

Example:

```sh
create users username password
```

#### insert [table name] [columns values]

inserts a new document in the specified table with the values passed

Example:

```sh
insert users JohnDoe helloWorld
```

#### select [columns name or *] From [table name] [where?]

returns an array with the specified columsn from the database

Example:

```sh
select username from users
```

#### where [key] [operator] [value]

optional parameter for the select command, compares the values from the table with the ones informed using the informed operator

Example:

```sh
select username from users where name = JohnDoe
```
