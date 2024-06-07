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

## List Product

### Url

```
https://acceptable-blisse-dian-nuswantoro-university-920e3c70.koyeb.app/products
```

### Response

````
{
  "status": "200",
  "message": "success",
  "data": [
    {
      "id": 1,
      "title": "Sansiviera",
      "images": "https://unsplash.com/img.jpg",
      "price": 15000,
      "price_discount": 10000,
      "category": 1
    },
    {
      "id": 2,
      "title": "Sansiviera",
      "images": "https://unsplash.com/img.jpg",
      "price": 25000,
      "price_discount": 20000,
      "category": 2
    }
  ]
}

```
````
