Add the column:

```
./gh-ost --user="root" --password="password" --host=localhost --database="school" --table="students" --verbose --alter="alter table students add column phone varchar(15);" --hooks-path=./hooks --allow-on-master
```

Remove the column:

```
./gh-ost --user="root" --password="password" --host=localhost --database="school" --table="students" --verbose --alter="alter table students drop phone;" --hooks-path=./hooks --allow-on-master
```

Make hooks executable with `chmod a+x ./hooks/gh-ost-on-hook`