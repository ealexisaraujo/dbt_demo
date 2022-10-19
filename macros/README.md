# Lab 4a: Macros 101

Are you new to dbt's macro and Jinja? This lab covers a series of macro examples that aims to help you understand a specific piece of Jinja code by running a sample macro and relating the Jinja code to its output.

## Steps

1. Create file macro_hello_world.sql, under demo_project/macros, containing macro examples.

   Run provided curl command to download precreated macro_hello_world.sql into the right location.

```bash
curl 'https://static.us-east-1.prod.workshops.aws/public/ba38c170-1f4d-4335-b8ce-bdbd4d76abff/static/lab_4a/code/macro_hello_world.sql' --output ~/environment/demo_project/macros/macro_hello_world.sql
```

2. Run dbt run-operation macro_hello_world_1 to showcase log which is used to print a defined output.

```bash
dbt run-operation macro_hello_world_1
```

3. Run dbt run-operation macro_hello_world_2 to showcase set, [], and for which are used to create a variable, represent a list and loop a list respectively. It is interesting to note that when a variable defined outside of a loop is updated inside the loop, the variable retains its original value.

```bash
dbt run-operation macro_hello_world_2
```

4. Run dbt run-operation macro_hello_world_3 to showcase namespace() which is used to hold variables created outside of a loop that when updated inside a loop, reflects the updated value. Think of variables held in namespace as global variables.

```bash
dbt run-operation macro_hello_world_3
```

5. Run dbt run-operation macro_hello_world_4 to showcase if, elif, and else which are used to test conditions.

```bash
dbt run-operation macro_hello_world_4
```

6. Run dbt run-operation macro_hello_world_5 to showcase run_query which sends a direct query to Amazon Redshift for processing.

```bash
dbt run-operation macro_hello_world_5
```

7. Run dbt run-operation macro_hello_world_6 --args "{'input': 'ABC'}" to showcase the defining and passing of an input.

```bash
dbt run-operation macro_hello_world_6 --args "{'input': 'ABC'}"
```

8. Run dbt run-operation macro_hello_world_7 to showcase the usage of dictionary data structure.

```bash
dbt run-operation macro_hello_world_7
```
