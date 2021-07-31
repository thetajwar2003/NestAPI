# NeStore

An e-commerce API built using Nest.js

## API Reference

#### Get All Items

```http
  GET /products
```

Output

```
[
    {
        "id": String,
        "title": String,
        "description": String,
        "price": Number
    },
]

```

#### Get Specific Item

```http
  GET /products/:id
```

Output

```
Success:
{
    "id": String,
    "title": String,
    "description": String,
    "price": Number
},

Error:
{
    "statusCode": Number,
    "error": String,
    "message": String
}

```

#### Post Item

```http
  POST /products
```

Input

```
{
    "title": String,
    "description": String,
    "price": Number
}
```

Output

```
{
    "id": String
}
```

#### Update item

```http
  PATCH /products/:id
```

Input

```
{
    "title": String,
    "description": String,
    "price": Number
}
```

Output

```
Success:
    *Nothing*

Error:
{
    "statusCode": Number,
    "error": String,
    "message": String
}
```

#### Delete item

```http
  DELETE /products/:id
```

Output

```
Success:
    *Nothing*

Error:
{
    "statusCode": Number,
    "error": String,
    "message": String
}
```
