# CRUD on Attendances #
*Authorized Requests => Need Token Representation of Yourself* 

## *Create Attendance* ##
*To create an attendance =>  POST /attendances*
```json
{ 
    user_id: "ID of user attendance object belongs to",
    event_in: "Timestamp of User's entering",
    event: "String description representing whether user is entering or leaving",
    beacon_id: "ID of beacon attendance object belongs to"
}
```

## Collection of Attendances ##
*To see all available attendances for given user =>  GET /attendances*
```json
[
    {   
    user_id: 1,
    event_in: "0:00:00",
    event_out: "1:11:11"
    beacon_id: 1,
    created_at: "0:00:00",
    updated_at: "0:00:00"
},
{   
    user_id: 1,
    event_in: "0:00:00",
    event_out: "1:11:11"
    beacon_id: 2,
    created_at: "0:00:00",
    updated_at: "0:00:00"
},
{   
    user_id: 1,
    event_in: "0:00:00",
    event_out: "1:11:11"
    beacon_id: 3,
    created_at: "0:00:00",
    updated_at: "0:00:00"
}
]
```


## Index Specific Attendance ##
*Fetch a specific attendance object /attendances/:id*
> RETURNS 
```json
{   
    user_id: 1,
    event_in: "0:00:00",
    event_out: "1:11:11"
    beacon_id: 1,
    created_at: "0:00:00",
    updated_at: "0:00:00"
}
```

## Updates Specfic Attendance ##
*Updates an existing attendance object /attendances/:id*
> Pass in updated attributes through PUT/PATCH body
```json
{   
    user_id: 1,
    event_in: "0:00:00",
    event_out: "1:11:11"
    beacon_id: 1,
    created_at: "0:00:00",
    updated_at: "0:00:00"
}
```

> RETURNS Updated Attendance Object
```json
{   
    user_id: 1,
    event_in: "0:00:00",
    event_out: "1:11:11"
    beacon_id: 1,
    created_at: "0:00:00",
    updated_at: "0:00:00"
}
```

## Delete Specific Attendance ##
*Deletes an existing attendance object /attendances/:id*
> RETURNS Beacon Object Deleted
```json
{   
    user_id: 1,
    event_in: "0:00:00",
    event_out: "1:11:11"
    beacon_id: 1,
    created_at: "0:00:00",
    updated_at: "0:00:00"
}
```