# MeLiDev
App development based on MercadoLibre's API

Some useful links:

Example Item:
http://articulo.mercadolibre.com.ve/MLV-465468083-guitarra-electroacustica-antonio-hermosa-nylon-_JM

Item_id=MLV465468083


Base URL:
https://api.mercadolibre.com


Item info:
/items/{Item_id}
https://api.mercadolibre.com/items/MLV465468083/


*About visits
  List item visits in a given period of time:
/items/{item_id}/visits/?date_from={date_from}&date_to={date_to}
https://api.mercadolibre.com/items/MLV465468083/visits/?date_from=2016-05-28T00:00:00.000-03:00&date_to=2016-06-02T23:59:59.999


·

·

·



# MeliDev



https://api.mercadolibre.com/items/MLV465562200/

https://api.mercadolibre.com/sites/

https://api.mercadolibre.com/items/MLV465468083/visits/?date_from=2016-05-28T00:00:00.000-03:00&date_to=2016-06-02T23:59:59.999


https://api.mercadolibre.com/questions/search?seller_id={}

https://api.mercadolibre.com/questions/search?seller_id=91382784

https://api.mercadolibre.com/questions/search?item=MLV465562200

·

**Some test with this Item: MLV465562200**

"start_time": "2016-05-25T12:56:36.000Z"

·

## Informacion a obtener:
·

### VISITAS

* Numero de visitas de un articulo en un rango de tiempo:  
[https://api.mercadolibre.com/items/MLV465562200/visits?date_from=2017-02-14T00:00:00.000-04:00&date_to=2017-02-14T23:59:59.999-04:00](https://api.mercadolibre.com/items/MLV465562200/visits?date_from=2017-02-14T00:00:00.000-04:00&date_to=2017-02-14T23:59:59.999-04:00)


* Numero de visitas en los ultimos 2 dias:  
https://api.mercadolibre.com/items/MLV465562200/visits/time_window?last=2&unit=day&ending=2017-02-19

·
### COMPRAS
* Numero total de ventas de un articulo:  
[https://api.mercadolibre.com/items/MLV465562200/](https://api.mercadolibre.com/items/MLV465562200/)


	TODO: Obtener numero de compras en un rango de tiempo


·
### PREGUNTAS
* Numero total de preguntas de un articulo:  
[https://api.mercadolibre.com/questions/search?item=MLV465562200&limit=0](https://api.mercadolibre.com/questions/search?item=MLV465562200&limit=0)  
(Se usa "limit=0" para no pedir los detalles de las preguntas)


* SOLO mostrar el numero de preguntas:  
https://api.mercadolibre.com/questions/search?item=MLV465562200&limit=0&attributes=total


	TODO: Obtener numero de preguntas en un rango de tiempo

·

**PARA OBTENER SOLO "ATRIBUTOS" ESPECIFICOS:**

***	?attributes= ***

**Request:**

https://api.mercadolibre.com/items/MLV465562200/  
Devuelve todo los atributos

https://api.mercadolibre.com/items/MLV465562200/?attributes=sold_quantity,start_time :+1:

**Response:**

```json
{
  "sold_quantity": 4613,
  "start_time": "2016-05-25T12:56:36.000Z"
}
```
