# Address Api Spec

## Create Address

Endpoint : POST /api/contacts/:contactId/addresses

Headers : 
- Authorization: token

Request Body :
```json
{
  "street": "Jalan", // optional
  "city": "Kota", // optional
  "province": "Provinsi", // optional
  "country": "Negara",
  "postal_code": "12345"
}
```

Response Body :
```json
{
  "data": {
    "street": "Jalan", // optional
    "city": "Kota", // optional
    "province": "Provinsi", // optional
    "country": "Negara",
    "postal_code": "12345"
  }
}
```

## Get Address

Endpoint : GET /api/contacts/:contactId/addresses/:addressId

Headers : 
- Authorization: token

Response Body :
```json
{
  "data": {
    "street": "Jalan", // optional
    "city": "Kota", // optional
    "province": "Provinsi", // optional
    "country": "Negara",
    "postal_code": "12345"
  }
}
```

## Update Address

Endpoint : PUT /api/contacts/:contactId/addresses/:addressId

Headers : 
- Authorization: token

Response Body :
```json
{
  "data": {
    "street": "Jalan", // optional
    "city": "Kota", // optional
    "province": "Provinsi", // optional
    "country": "Negara",
    "postal_code": "12345"
  }
}
```

## Remove Address

Endpoint : DELETE /api/contacts/:contactId/addresses/:addressId

Headers : 
- Authorization: token

Response Body :
```json
{
  "data": true
}
```

## List Addresses

Endpoint : GET /api/contacts/:contactId/addresses

Headers : 
- Authorization: token

Response Body :
```json
{
  "data": [
    {
      "id": 1,
      "street": "Jalan", // optional
      "city": "Kota", // optional
      "province": "Provinsi", // optional
      "country": "Negara",
      "postal_code": "12345"
    },
    {
      "id": 2,
      "street": "Jalan", // optional
      "city": "Kota", // optional
      "province": "Provinsi", // optional
      "country": "Negara",
      "postal_code": "12345"
    }
  ]
}
```