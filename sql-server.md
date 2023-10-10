
# Tips
- Cannot drop database because it is currently in use

    ```sql
    use master
    alter database [DB_NAME] set single_user with rollback immediate

    drop database [DB_NAME]
    ```
- Create schema if not exist

    ```sql
    IF NOT EXISTS (SELECT * FROM sys.schemas WHERE name = 'master')
    BEGIN
        EXEC ('CREATE SCHEMA master;');
    END;
    ```
# Reference
- https://stackoverflow.com/questions/1711840/how-do-i-specify-close-existing-connections-in-sql-script
- https://stackoverflow.com/questions/18697578/cant-create-schema-inside-begin-block