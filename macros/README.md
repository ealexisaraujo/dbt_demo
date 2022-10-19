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

<!-- insert images in markdown-->

![macro_hello_world_1]
