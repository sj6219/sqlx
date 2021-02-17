set  DATABASE_URL=sqlite:C:\Users\sjpark\Documents\sqlx\todos.db
set  DATABASE_URL=sqlite:todos.db
cargo build --bin=sqlx-example-sqlite-todos --package=sqlx-example-sqlite-todos

# TODOs Example

## Setup

1. Declare the database URL

    ```
    export DATABASE_URL="sqlite:todos.db"
    ```

2. Create the database.

    ```
    $ sqlx db create
    ```

3. Run sql migrations

    ```
    $ sqlx migrate run
    ```

## Usage

Add a todo 

```
cargo run -- add "todo description"
```

Complete a todo.

```
cargo run -- done <todo id>
```

List all todos

```
cargo run
```
