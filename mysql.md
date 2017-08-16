# MySQL

## Update
Update selected fields based on `WHERE` clause.
```
    UPDATE <table_name> SET field1=value1,field2=value2 WHERE <clause>;
```

## Show columns but exclude everything except the field names
```MySQL

    SELECT column_name
    FROM information_schema.columns
    WHERE  table_name = 'your_table' AND table_schema = 'database_name'
```

## References
* [Show columns but exclude everything except the field names](https://stackoverflow.com/a/5525990)
