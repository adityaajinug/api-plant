# Rules

## URL rules

```
Contoh Benar :
http://api.example.com/products
http://api.example.com/payment-method

Contoh Salah :
http://api.example.com/get-all-products
http://api.example.com/get-payment-method

http://api.example.com/getproducts
http://api.example.com/getpaymentmethod


Contoh Benar :
GET http://api.example.com/products/{productId}
POST http://api.example.com/products

Contoh Salah :

GET http://api.example.com/get-products-by-id/{productId}
POST http://api.example.com/create-product


```

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
https://acceptable-blisse-dian-nuswantoro-university-920e3c70.koyeb.app/product
```

### Response

```
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
## Detail Product
### URL
```
https://acceptable-blisse-dian-nuswantoro-university-920e3c70.koyeb.app/product/(uuid_product)
```
### Response
```
{
  "status": "200",
  "message": "success",
  "data": {
    "id": 1,
    "title": "string",
    "price": 0,
    "after_discount": 0,
    "size": [
      {
        "id": "uuid",
        "size": "string"
      },
      {
        "id": "uuid",
        "size": "string"
      }
    ],
    "image": ["url1", "url2"],
    "description": "string",
    "category": "string"
  }
}

```
## Detail Product Review
### URL
```
https://acceptable-blisse-dian-nuswantoro-university-920e3c70.koyeb.app/product/review?id=(uuid_product)
```
### Response
```
{
  "status": "200",
  "message": "success",
  "data": [
    {
      "fullname": "John Doe",
      "photo": "url",
      "comment": "This is a comment"
    },
    {
      "fullname": "Jane Doe",
      "photo": "url",
      "comment": "This is a comment"
    }
  ]
}

```
## Cart
### Response
```
{
  "status": "200",
  "message": "success",
  "data": [
    {
      "id": "1",
      "title": "Sansiviera",
      "images": "https://unsplash.com/img.jpg",
      "price": 25000,
      "price_discount": 20000,
      "size": "M",
      "quantity": 10
    },
    {
      "id": "1",
      "title": "Sansiviera",
      "images": "https://unsplash.com/img.jpg",
      "price": 25000,
      "price_discount": 20000,
      "size": "M",
      "quantity": 10
    }
  ]
}


```
## Payment Method

### Url

```
https://acceptable-blisse-dian-nuswantoro-university-920e3c70.koyeb.app/ref/payment-method
```

### Response
```
{
  "status": "200",
  "message": "success",
  "data": [
    {
      "id": "1",
      "bank_name": "BNI",
      "logo": "https://unsplash.com/img.jpg",
      "bank_number": "123456789"
    },
    {
      "id": "2",
      "bank_name": "BRI",
      "logo": "https://unsplash.com/img.jpg",
      "bank_number": "8765434567"
    }
  ]
}

```

## Address
### Url

```
https://acceptable-blisse-dian-nuswantoro-university-920e3c70.koyeb.app/shipping-address
```
### Response
```
{
  "status": "200",
  "message": "success",
  "data": [
    {
      "id": "1",
      "address_label": "Rumah",
      "recipient": "Adit",
      "address": "Jl. Kebon Jeruk No. 1, Jakarta Barat",
      "village": "Kebon Jeruk",
      "district": "Kebon Jeruk",
      "city": "Jakarta Barat",
      "province": "DKI Jakarta",
      "postal_code": "11530",
      "phone": "08123456789"
    }
  ]
}

```