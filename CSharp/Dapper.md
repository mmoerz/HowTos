# Dapper


## Hidden Loaf of Evil

If tables utilize other string types than nvarchar, not using DbString will
lead to a massiv performance penalty.

So to counter this problem you must use DbString.

Usage example:
```
employee = db.QueryFirst<Employee>(
        "select * from employeeDetails 
         With (nolock) where empID = @empID ", 
        new { @empID = new DbString { Value = "1", IsFixedLength = false, IsAnsi = true, Length = 15 } });
```
Read the [article](https://jithilmt.medium.com/sql-server-hidden-load-evil-performance-issue-with-dapper-465a08f922f6)
for more information about the problem.

## Resources
https://www.learndapper.com/

https://dapper-tutorial.net/

(vids)
https://www.jetbrains.com/dotnet/guide/tutorials/dotnet-days-online-2020/better-object-mapping-in-net-with-dapper/
