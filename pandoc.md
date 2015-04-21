
A Table
=======

| VersionRoot            | Versioned         | VersionRelated      |
| :--------------------- | :---------------- | :------------------ |
| `latest_version int`   | `version int`     | `version_from int`  |
|                        | `valid_from date` | `version_to int`    |
|                        | `valid_to date`   |                     |


Some code Syntax
=========


```sqlpostgresql
    create table Assets (
        asset_id    text
        asset_type  text
    ) inherits VersionRoot
```

A List
======

* Top level
    - Nested 1
    - Nested 2
* Another top
    #. Numbered
    #. Numbered

Some text with a footnote[^blah] in the middle



[^blah]: Footnotes have nice names


Explanation List
---------------

There are several options

(@a) Option A
(@b) Option A
(@c) Option A
(@d) Option A
(@e) Option A


My favourite is option @b.


---------------------------------------------------------------------
Layer            Description
---------------- ----------------------------------------------------
Logging          Log basic information about request using
(server)         Standard logging

Authentication   Use Windows auth to authenticate the connected user.
(server)         Check that user is peermitted to connect on behalf of
                 Client

Encoding         Compress response according to callers Accept header
(server)         gzip/deflate etc

Routing          Extract URL components and dispatch
(server)

Engine           Database Access
(server)

PG-Pool          Distribute database calls to appropriate server/schema
(Pg-pool)

PG               Postgres Database, sharded based on client
(database)
---------------------------------------------------------------------


Position Calculations
---------------------

---------------------------------------------------------------------
trade_date      version_from    version_to      position
----------      -----------     ----------      --------
x               y               z               77
---------------------------------------------------------------------

