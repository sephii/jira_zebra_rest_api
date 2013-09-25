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

_NA_

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
            carried_over": "9.5",
            done: "1153.25",
            target: "1171.2"
        },
        vacation: {
            balance": "97",
            carried_over": "49"
            available: "160",
            used": "112",
        },
        education_budget: [
            {
                name: "Techtalk",
                activity_id: 71,
                employment_rate_dependent: false,
                work_period_dependent: true,
                allocated: {
                    budget: 0,
                    hours: 16
                },
                used: {
                    budget: 0,
                    hours: 25
                },
                balance: {
                    budget: 0,
                    hours: -9
                }
            }
        ]
    }

### POST

_NA_

### DELETE

_NA_

## /reports/

### GET

Arguments

* start_date
* end_date
* user_id
* project_id
* activity_id

Response

    [{
        id: "218030",
        project: {
            id: 1521,
            name: "Further education (Weiterbildung) 2013"
        }
        activity: {
            id: 97,
            name: "Quartalsworkshop Team",
            rate: "0.00"
        },
        user: {
            id: 1,
            name: "john.doe",
            first_name: "John",
            last_name: "Doe",
        }
        date: "2013-09-24",
        time: "3.25",
    }]

### PUT

Arguments

* project_id
* activity_id
* hours
* description
* date

Response

    {
        id: 1500
    }

## /reports/id/

### GET

Response

    {
        id: "218030",
        project: {
            id: 1521,
            name: "Further education (Weiterbildung) 2013"
        }
        activity: {
            id: 97,
            name: "Quartalsworkshop Team",
            rate: "0.00"
        },
        user: {
            id: 1,
            name: "john.doe",
            first_name: "John",
            last_name: "Doe",
        }
        date: "2013-09-24",
        time: "3.25",
    }

### POST

Arguments

* project_id
* activity_id
* hours
* description
* date

### DELETE

## /contacts/

### GET

Arguments

* first_name
* last_name
* email

Response

    [{
        id: 1000,
        first_name: "Jane",
        last_name: "Doe",
        email: "jane.doe@janedoe.com",
        phone: {
            mobile: "079 123 45 67",
            home: "021 123 45 67"
        }
    }]

### PUT

_NA_

## /contacts/id/

### GET

Response

    {
        id: 1000,
        first_name: "Jane",
        last_name: "Doe",
        email: "jane.doe@janedoe.com",
        phone: {
            mobile: "079 123 45 67",
            home: "021 123 45 67"
        }
    }

### POST

_NA_

### DELETE

_NA_

## /projects/

### GET

Arguments

* project_name
* team_name

### PUT

_NA_

## /projects/id/

# Jira

TODO thx sitron
