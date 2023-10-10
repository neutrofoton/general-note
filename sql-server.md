
# Tips
- Cannot drop database because it is currently in use

    ```sql
    use master
    alter database [DB_NAME] set single_user with rollback immediate

    drop database [DB_NAME]
    ```

# Reference
- https://stackoverflow.com/questions/1711840/how-do-i-specify-close-existing-connections-in-sql-script