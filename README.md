```
D CREATE OR REPLACE TABLE rep AS SELECT 3 AS s;

D CREATE OR REPLACE TABLE R AS SELECT 1 AS A, 2 AS s;

D ALTER TABLE R ADD COLUMN B INTEGER DEFAULT 10;
Hello! The query is: ALTER TABLE R ADD COLUMN B INTEGER DEFAULT 10;
Specialized Alter for Table R
fact table column size: 2
rep table column size: 1
idx is: 1
fact row group size: 1
rep row group size: 1
fact row group row_start: 0
rep row group row_start: 0
fact tree number of nodes: 1
rep tree number of nodes: 1
factCol->column_index: 1
factCol->info.table: rep

D SELECT * FROM R;
Hello! The query is: SELECT * FROM R;
┌───────┬───────┐
│   A   │   s   │
│ int32 │ int32 │
├───────┼───────┤
│     1 │     3 │
└───────┴───────┘
D SELECT * FROM rep;
```
