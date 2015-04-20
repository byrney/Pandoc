
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


