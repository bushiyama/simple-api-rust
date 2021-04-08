# simple-api-rust

```bash
$ cargo run
```

```bash
$ curl http://localhost:8080/todos/123
{"id":123,"content":"やること","done":false}

$ curl --location --request POST 'localhost:8080/todos' \
> --header 'Content-Type: application/json' \
> --data-raw '{
>     "content": "なにかやる",
>     "done": false
> }'
ok

# cargo run's console out
post_todo
Json: Todo { id: None, content: "なにかやる", done: false }
```
