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
https://acceptable-blisse-dian-nuswantoro-university-920e3c70.koyeb.app/payment-method
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
      "label": "Rumah",
      "client_name": "Adit",
      "address": "Jl. Kebon Jeruk No. 1, Jakarta Barat",
      "kelurahan": "Kebon Jeruk",
      "kecamatan": "Kebon Jeruk",
      "kota": "Jakarta Barat",
      "provinsi": "DKI Jakarta",
      "kode_pos": "11530",
      "phone": "08123456789"
    },
    {
      "id": "2",
      "label": "Rumah",
      "client_name": "Adit",
      "address": "Jl. Kebon Jeruk No. 1, Jakarta Barat",
      "kelurahan": "Kebon Jeruk",
      "kecamatan": "Kebon Jeruk",
      "kota": "Jakarta Barat",
      "provinsi": "DKI Jakarta",
      "kode_pos": "11530",
      "phone": "08123456789"
    }
  ]
}

```