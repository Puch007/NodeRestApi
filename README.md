# BaseAPI

Description: Get all the cars from the database
Endpoint:http://localhost:3002/api/v1/car
GETParams: none
Request Payload: none
Response:
[
    {
        "id": 1,
        "make": "Nissan",
        "model": "Murano",
        "year": "2015",
        "user_id": 1,
        "active": true,
        "created_by": "SYS",
        "updated_by": "SYS",
        "created_at": "2021-04-30T04:35:50.077Z",
        "updated_at": "2021-04-30T04:39:31.684Z",
        "deleted_at": null,
        "mileage": null,
        "color": null
    },
    {
        "id": 2,
        "make": "Nissan",
        "model": "350z",
        "year": "2018",
        "user_id": 1,
        "active": true,
        "created_by": "SYS",
        "updated_by": null,
        "created_at": "2021-04-30T04:35:59.274Z",
        "updated_at": "2021-04-30T04:35:59.274Z",
        "deleted_at": null,
        "mileage": null,
        "color": null
    },
    {
        "id": 3,
        "make": "Nissan",
        "model": "Maxima",
        "year": "2018",
        "user_id": 2,
        "active": true,
        "created_by": "SYS",
        "updated_by": null,
        "created_at": "2021-04-30T04:36:30.495Z",
        "updated_at": "2021-04-30T04:36:30.495Z",
        "deleted_at": null,
        "mileage": null,
        "color": null
    },
    {
        "id": 4,
        "make": "nissan",
        "model": "350",
        "year": null,
        "user_id": null,
        "active": true,
        "created_by": "SYS",
        "updated_by": null,
        "created_at": "2021-05-01T07:26:57.142Z",
        "updated_at": "2021-05-01T07:26:57.142Z",
        "deleted_at": null,
        "mileage": null,
        "color": null
    },
    {
        "id": 5,
        "make": "Toyota",
        "model": "Celica",
        "year": null,
        "user_id": null,
        "active": true,
        "created_by": "SYS",
        "updated_by": null,
        "created_at": "2021-05-01T16:18:11.750Z",
        "updated_at": "2021-05-01T16:18:11.750Z",
        "deleted_at": null,
        "mileage": null,
        "color": "black"
    },
    {
        "id": 6,
        "make": "Toyota",
        "model": "Celica",
        "year": null,
        "user_id": null,
        "active": true,
        "created_by": "SYS",
        "updated_by": null,
        "created_at": "2021-05-01T16:19:04.843Z",
        "updated_at": "2021-05-01T16:19:04.843Z",
        "deleted_at": null,
        "mileage": null,
        "color": "Blue"
    },
    {
        "id": 7,
        "make": "Dodge",
        "model": "Ram",
        "year": null,
        "user_id": null,
        "active": true,
        "created_by": "SYS",
        "updated_by": "SYS",
        "created_at": "2021-05-01T16:19:09.561Z",
        "updated_at": "2021-05-01T16:27:21.298Z",
        "deleted_at": null,
        "mileage": null,
        "color": "Green"
    }
]

Description: Get a car by its ID from the database
Endpoint:http://localhost:3000/api/v1/car/id/1
GETParams: id - the car id
Request Payload: none
Response:{
        "id": 1,
        "make": "Nissan",
        "model": "Murano",
        "year": "2015",
        "user_id": 1,
        "active": true,
        "created_by": "SYS",
        "updated_by": "SYS",
        "created_at": "2021-04-30T04:35:50.077Z",
        "updated_at": "2021-04-30T04:39:31.684Z",
        "deleted_at": null,
        "mileage": null,
        "color": null
    }
    Description: Create a new car record
    Endpoint:http://localhost:3000/api/v1/car
    POSTParams: none
    Request Payload:
    {
        "id": 7,
        "make": "Dodge",
        "model": "Ram",
        "color": "Green"
    }
    Response:
    {
        "id": 7,
        "make": "Dodge",
        "model": "Ram",
        "year": null,
        "user_id": null,
        "active": true,
        "created_by": "SYS",
        "updated_by": "SYS",
        "created_at": "2021-05-01T16:19:09.561Z",
        "updated_at": "2021-05-01T16:27:21.298Z",
        "deleted_at": null,
        "mileage": null,
        "color": "Green"
    }
    Description: Update a car record
Endpoint:http://localhost:3000/api/v1/car/id/6
PUTParams: id - the id of the book
Request Payload: "id": 6,
        "make": "Toyota",
        "model": "Celica",
        "color": "Blue"
        
Response:
   {"id": 6,
        "make": "Toyota",
        "model": "Celica",
        "year": null,
        "user_id": null,
        "active": true,
        "created_by": "SYS",
        "updated_by": null,
        "created_at": "2021-05-01T16:19:04.843Z",
        "updated_at": "2021-05-01T16:19:04.843Z",
        "deleted_at": null,
        "mileage": null,
        "color": "Blue"}
        
       Description: Delete a book record
        Endpoint:http://localhost:3000/api/v1/carid/6
        DELETEParams: id - The id of the car
        Request Payload: None
        Response:
        {
    "data": [],
    "statusCode": 200,
    "message": "delete success"
}
        
