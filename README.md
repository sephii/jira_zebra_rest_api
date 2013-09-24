# Zebra

## /users/

### GET

Arguments

* first_name
* last_name
* id


Response

    [
        {
            id: 1,
            username: "john.doe",
            firstname: "john",
            lastname: "doe",
            email: "john.doe@liip.ch",
            location: "Lausanne",
            birthdate: "1950-12-31"
        }
    ]


### PUT

NA

## /users/username/

### GET

Response

    {
        id: 1,
        username: "john.doe",
        firstname: "John",
        lastname: "Doe",
        email: "john.doe@liip.ch",
        birthdate: "1950-12-31",
        contact: {
            street: "Maple Street 12",
            zip: "1000",
            city: "Lausanne",
            phone: {
                mobile: "079 123 45 67",
                home: "021 123 45 67",
                company: "021 123 45 67"
            }
        },
        hours: {
            balance: "-8.45",
            legacy": "9.5",
            done: "1153.25",
            target: "1171.2"
        },
    }

### POST

NA

### DELETE

NA

## /reports/

### GET

Arguments

* start_date
* end_date
* user_id
* project_id
* activity_id

### PUT

NA

## /reports/id/

### GET
### POST
### DELETE

## /contacts/

### GET

Arguments

* first_name
* last_name

### PUT

NA

## /contacts/id/

### GET
### POST

NA

### DELETE

NA

## /projects/

### GET

Arguments

* project_name
* team_name

### PUT

NA

## /projects/id/

# Jira

TODO thx sitron
