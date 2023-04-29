# Fruits Web App

## objective

The objective of this project is to create a web app that allows users to view a list of fruits and add new fruits to the list.

## requirements

- [ ] The app should have a home page that displays a list of fruits.
- [ ] The app should have a form that allows users to add new fruits to the list.
- [ ] The app should show a fruits by specifying the fruit type in the URL.

## databsae structure

```json
{
    "grocery": {
        "1": {
            "name": "Apple",
            "quantity": 2,
            "price": 2.4,
            "type": "fruit"
        },
        "2": {
            "name": "Milk",
            "quantity": 1,
            "price": 2.5,
            "type": "dairy"
        },
        "4": {
            "name": "Bread",
            "quantity": 1,
            "price": 1.5,
            "type": "bakery"
        },
        "5": {
            "name": "Chicken",
            "quantity": 2,
            "price": 2.5,
            "type": "meat"
        },
        "6": {
            "name": "Coffee",
            "quantity": 2,
            "price": 2.5,
            "type": "grain"
        }
    }
}
```

## Grocery item properties

- [ ] `name` - the name of the fruit.
- [ ] `quantity` - the quantity of the fruit.
- [ ] `price` - the price of the fruit.
- [ ] `type` - the type of the fruit.

types of grocery items:

- `fruit`
- `dairy`
- `bakery`
- `meat`
- `grain`

## GroceryDB - database class

for this project we will use a database class to store our data. The database class will have the following methods:

- [ ] `__init__` - the constructor method that will initialize the database class.
- [ ] `add` - a method that will add a new item to the database.
- [ ] `all` - a method that will return all the items in the database.
- [ ] `get_by_type` - a method that will return all the items in the database that match the type specified in the URL.
- [ ] `get_by_name` - a method that will return all the items in the database that match the name specified in the URL.
- [ ] `get_by_price` - a method that will return all the items in the database that match the price specified in the URL.

## Endpoints

- [ ] GET `/grocery` - this endpoint will display a list of fruits.
- [ ] POST `/grocery/add` - this endpoint will display a form that allows users to add new fruits to the list.
- [ ] GET `/grocery/type/<type>` - this endpoint will display a list of fruits by specifying the fruit type in the URL.
- [ ] GET `/grocery/name/<name>` - this endpoint will display a list of fruits by specifying the fruit name in the URL.
- [ ] GET `/grocery/price/<price>` - this endpoint will display a list of fruits by specifying the fruit price in the URL.


## API documentation

1. GET `/grocery` - get all grocery from database.

response:

```json
[
    {
        "name": "Apple",
        "quantity": 2,
        "price": 2.4,
        "type": "fruit"
    }
]
```

| parameter | type | description |
| --- | --- | --- |
| `name` | `string` | the name of the fruit. |
| `quantity` | `int` | the quantity of the fruit. |
| `price` | `float` | the price of the fruit. |
| `type` | `string` | the type of the fruit. |
