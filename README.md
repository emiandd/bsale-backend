### bsale-backend
bsale backend for deploy

# Bsale Store Api

# Obtener todos los productos

### Request

`GET /products`

    https://bsale--back.herokuapp.com/products

### Response

    HTTP/1.1 200 Ok

    [{
      "id": 5,
      "name": "ENERGETICA MR BIG",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/misterbig3308256.jpg",
      "price": 1490,
      "discount": 20,
      "category": 1
    }, 
    {
      "id": 6,
      "name": "ENERGETICA RED BULL",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/redbull8381.jpg",
      "price": 1490,
      "discount": 0,
      "category": 1
    }, 
    {
      "id": 7,
      "name": "ENERGETICA SCORE",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/logo7698.png",
      "price": 1290,
      "discount": 0,
      "category": 1
    }]
    
# Obtener productos por nombre

### Request

const { search } = req.query;

`GET /products?search=name`

    https://bsale--back.herokuapp.com/products?search=coca

### Response
    
     HTTP/1.1 200 Ok

    [{
      "id": 37,
      "name": "COCA COLA ZERO DESECHABLE",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/cocazero9766.jpg",
      "price": 1490,
      "discount": 0,
      "category": 4
    }, {
      "id": 57,
      "name": "COCA COLA NORMAL DESECHABLE 1500cc",
      "url_image": null,
      "price": 1500,
      "discount": 0,
      "category": 4
    }, {
      "id": 58,
      "name": "COCA COLA LIGHT DESECHABLE",
      "url_image": null,
      "price": 1500,
      "discount": 0,
      "category": 4
    }]
    
# Obtener todas las categorias

### Request

`GET /categories`

    https://bsale--back.herokuapp.com/categories

### Response 

   HTTP/1.1 200 Ok

    [{
      "id": 1,
      "name": "bebida energetica"
    }, {
      "id": 2,
      "name": "pisco"
    }, {
      "id": 3,
      "name": "ron"
    }, {
      "id": 4,
      "name": "bebida"
    }, {
      "id": 5,
      "name": "snack"
    }, {
      "id": 6,
      "name": "cerveza"
    }, {
      "id": 7,
      "name": "vodka"
    }]
    
# Obtener productos por categoría

### Request

`GET /products/:category`

    https://bsale--back.herokuapp.com/products/5

### Response 

   HTTP/1.1 200 Ok

    [{
      "id": 47,
      "name": "Maní salado",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/manisaladomp4415.jpg",
      "price": 600,
      "discount": 0,
      "category": 5
    }, {
      "id": 53,
      "name": "Mani Sin Sal",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/manisinsalmp6988.jpg",
      "price": 500,
      "discount": 0,
      "category": 5
    }, {
      "id": 54,
      "name": "Papas Fritas Lisas Bolsa Grande",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/papaslisasgrande7128.jpg",
      "price": 1490,
      "discount": 0,
      "category": 5
    }, {
      "id": 55,
      "name": "Papas Fritas Bolsa Pequeña",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/papaslisas7271.jpg",
      "price": 500,
      "discount": 0,
      "category": 5
    }, {
      "id": 56,
      "name": "Papas Fritas Tarro",
      "url_image": "https://dojiw2m9tvv09.cloudfront.net/11132/product/78028005335657432.jpg",
      "price": 1990,
      "discount": 0,
      "category": 5
    }]
