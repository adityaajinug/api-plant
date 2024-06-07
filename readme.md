# Rules

## Status Response

```
{
    status : "200"
},
{
    status : "404"
},
{
    status : "500"
},
```

## Default message base response

```
{
    message : "success"
},
{
    message : "failed"
},
{
    message : "error server"
},
```

## Default data array or object

```
{
    data : []
},
{
    data : {}
},
{
    data : {
        "title": "Product 1",
        "size": [
            {
                id: 1,
                label: "S"
            }
        ],
        "price": 15000,
        "category_id": 1
    }
},
```
