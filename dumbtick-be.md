# LOGIN IMPLEMENTATION

## A. Requirements

**url** = {your_host}/api/v1/login
**mehtod** = POST
**request body** =

```json
{
    "email": "iis@gmail.com",
    "password": "lovespiderman"
}
```

**response body** =

```json
{
    "status": "success",
    "data": {
        "user": {
            "email": "iis@gmail.com",
            "token": "0sdnOJIoinsdo9878IJNBIniiuinINiuYIUY"
        }
    }
}
```

## B. Instructions

- When you finish this task, move it to "test" list. Then don't forget to push your job on `https://github.com/[your_name]`-dumbtick-be

- Create branch `1.Login-API`.

```
    git checkout -b 1.Login-API
```

- Push to branch `1.Login-API`.

```
    git add .
    git commit -m "add Login-API"
    git push origin 1.Login-API
```

<br/>

==============================

<br/>

# REGISTER IMPLEMENTATION

## A. Requirements

**url** = {your_host}/api/v1/register
**mehtod** = POST
**request body** =

```json
{
    "email": "iis@gmail.com",
    "password": "lovespiderman",
    "fullName": "Iis Dahlia",
    "role": "user"
}
```

**response body** =

```json
{
    "status": "success",
    "data": {
        "user": {
            "email": "iis@gmail.com",
            "token": "0sdnOJIoinsdo9878IJNBInii.uinINiuYIUxcvx.zhjsdga89asjadsaY"
        }
    }
}
```

## B. Instructions

- When you finish this task, move it to "test" list. Then don't forget to push your job on `https://github.com/[your_name]`-dumbtick-be

- Create branch `2.Register-API`.

```
    git checkout -b 2.Register-API
```

- Push to branch `2.Register-API`.

```
    git add .
    git commit -m "add Register API"
    git push origin 2.Register-API
```

<br/>

==============================

<br/>

# USER IMPLEMENTATION

## A. Requirements

**url** = {your_host}/api/v1/users
**mehtod** = GET
**response body** =

```json
{
    "status": "success",
    "data": {
        "users": [
            {
                "id": 1,
                "fullName": "spiderman",
                "email": "spiderman@gmail.com"
            },
            {
                "id": 2,
                "fullName": "Haris",
                "email": "haris@gmail.com"
            },
            {
                "id": 3,
                "fullName": "surti",
                "email": "surti@gmail.com"
            }
        ]
    }
}
```

### 2. Delete Users

**url** = {your_host}/api/v1/user/{id_user}
**method** = DELETE
**response body** =

```json
{
    "status": "success",
    "data": {
        "id": 1
    }
}
```

## B. Instructions

- When you finish this task, move it to "test" list. Then don't forget to push your job on `https://github.com/[your_name]`-dumbtick-be

- Create branch `3.Users`.

```
    git checkout -b 3.Users
```

- Push to branch `3.Users`.

```
    git add .
    git commit -m "add Users"
    git push origin 3.Users
```

<br/>

==============================

<br/>

# TICKET IMPLEMENTATION

## A. Requirements

### 1. Get Tickets

> **url** = {your_host}/api/v1/tickets
> **mehtod** = GET
> **response body** =

```json
{
    "status": "success",
    "data": {
        "books": [
            {
                "id": 1,
                "title": "Raisa Live In Concert",
                "category": "Music",
                "startDate": "13 Dec 2019 18:00",
                "endDate": "13 Dec 2019 22:00",
                "price": 300000,
                "address": "Jl. Pintu Satu Senayan, Gelora, Kecamatan Tanah Abang, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10270",
                "urlMap": "https://maps.google.com/xxxxxxxxxxxx",
                "phone": "+6287739320015",
                "email": "isbos@juniconcert.co.id",
                "description": "Raisa Live In Concert..."
            },
            {
                "id": 2,
                "title": "Eco Living Fun Bike",
                "category": "Sport",
                "startDate": "12 Dec 2019 07:00",
                "endDate": "12 Dec 2019 12:00",
                "price": 300000,
                "address": "Jl. Pintu Satu Senayan, Gelora, Kecamatan Tanah Abang, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10270",
                "urlMap": "https://maps.google.com/xxxxxxxxxxxx",
                "phone": "+6287739320015",
                "email": "isbos@juniconcert.co.id",
                "description": "Looking at its layout. The point..."
            },
            {
                "id": 3,
                "title": "Bootcamp Dumbways",
                "category": "Education",
                "startDate": "12 Dec 2019 08:00",
                "endDate": "12 Dec 2019 13:00",
                "price": 300000,
                "address": "Jl. Elang IV, Sawah Lama, Ciputat, Bintaro, Kota Tangerang Selatan",
                "urlMap": "https://maps.google.com/xxxxxxxxxxxx",
                "phone": "+6287739320015",
                "email": "help@dumbways.id",
                "description": "Coding Bootcamp..."
            }
        ]
    }
}
```

### 2. Get Detail Book

**url** = {your_host}/api/v1/ticket/{ticketId}
**method** = GET
**response body** =

```json
{
    "status": "success",
    "data": {
        "ticket": {
            "id": 1,
            "title": "Raisa Live In Concert",
            "category": "Music",
            "startDate": "13 Dec 2019 18:00",
            "endDate": "13 Dec 2019 22:00",
            "price": 300000,
            "address": "Jl. Pintu Satu Senayan, Gelora, Kecamatan Tanah Abang, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10270",
            "urlMap": "https://maps.google.com/xxxxxxxxxxxx",
            "phone": "+6287739320015",
            "email": "isbos@juniconcert.co.id",
            "description": "Raisa Live In Concert..."
        }
    }
}
```

### 3. Add Book

**url** = {your_host}/api/v1/ticket
**recruitments** = For epub file upload it using multer
**method** = POST
**request header** =

```json
{
    "Authorization": "Bearer {token}"
}
```

**request body** =

```json
{
    "id": 1,
    "title": "Raisa Live In Concert",
    "category": "Music",
    "startDate": "13 Dec 2019 18:00",
    "endDate": "13 Dec 2019 22:00",
    "price": 300000,
    "address": "Jl. Pintu Satu Senayan, Gelora, Kecamatan Tanah Abang, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10270",
    "urlMap": "https://maps.google.com/xxxxxxxxxxxx",
    "phone": "+6287739320015",
    "email": "isbos@juniconcert.co.id",
    "description": "Raisa Live In Concert..."
}
```

**response body** =

```json
{
    "status": "success",
    "data": {
        "ticket": {
            "id": 1,
            "title": "Raisa Live In Concert",
            "category": "Music",
            "startDate": "13 Dec 2019 18:00",
            "endDate": "13 Dec 2019 22:00",
            "price": 300000,
            "address": "Jl. Pintu Satu Senayan, Gelora, Kecamatan Tanah Abang, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10270",
            "urlMap": "https://maps.google.com/xxxxxxxxxxxx",
            "phone": "+6287739320015",
            "email": "isbos@juniconcert.co.id",
            "description": "Raisa Live In Concert..."
        }
    }
}
```

### 4. Edit Book

**url** = {your_host}/api/v1/ticket/{ticketId}
**method** = PUT / PATCH
**request header** =

```json
{
  "Authorization": "Bearer {token}"
}
```

**request body** =

```json
{
    "title": "Tess On Road Updated",
}
```

**response body** =

```json
{
    "status": "success",
    "data": {
        "book": {
            "id": 1,
            "title": "Tess On Road Updated",
            "category": "Music",
            "startDate": "13 Dec 2019 18:00",
            "endDate": "13 Dec 2019 22:00",
            "price": 300000,
            "address": "Jl. Pintu Satu Senayan, Gelora, Kecamatan Tanah Abang, Kota Jakarta Pusat, Daerah Khusus Ibukota Jakarta 10270",
            "urlMap": "https://maps.google.com/xxxxxxxxxxxx",
            "phone": "+6287739320015",
            "email": "isbos@juniconcert.co.id",
            "description": "Raisa Live In Concert..."
        }
    }
}
```

### 5. Delete Product

**url** = {your_host}/api/v1/ticket/{ticketId}
**method** = DELETE
**request header** =

```json
{
    "Authorization": "Bearer {token}"
}
```

**response body** =

```json
{
    "status": "success",
    "data": {
        "id": 1
    }
}
```

## B. Instructions

- When you finish this task, move it to "test" list. Then don't forget to push your job on `https://github.com/[your_name]`-dumbtick-be

- Create branch `4.Ticket`.

```bash
    git checkout -b 4.Ticket
```

- Push to branch `4.Ticket`.

```bash
    git add .
    git commit -m "add Ticket "
    git push origin 4.Ticket
```
