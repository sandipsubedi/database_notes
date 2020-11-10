## dump database:

- Excluding users.
```
pg_dump -h host.com -U postgres -W --exclude-table-data=users -F p postgres > dump_data.sql
```

- add `-v` at the end to see it progressing:
```
pg_dump -h host.com -U postgres -W --exclude-table-data=users -F p postgres > dump_data.sql -v
```


## shows the file with size:
```
 ls -lh dump_data.sql
```