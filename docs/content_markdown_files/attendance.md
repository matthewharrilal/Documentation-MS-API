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


## Index Specific Beacon ##
*Fetch a specific beacon /beacons/:id*
> RETURNS 
```json
{   
    id: 1,
    hardware_id: "1",
    title: "Beacon Title",
    created_at: "0:00:00",
    updated_at: "0:00:00"
}
```

## Updates Specfic Beacon ##
*Updates a specific beacon /beacons/:id*
> Pass in updated attributes through PUT/PATCH body
```json
{   
    id: 1,
    hardware_id: "6",
    title: "Updated Beacon Id",
    created_at: "0:00:01",
    updated_at: "0:00:01"
}
```

> RETURNS Updated Beacon Object
```json
{   
    id: 1,
    hardware_id: "6",
    title: "Updated Beacon Id",
    created_at: "0:00:01",
    updated_at: "0:00:01"
}
```

## Delete Specific Beacon ##
*Deletes a specific beacon /beacons/:id*
> RETURNS Beacon Object Deleted
```json
{   
    id: 1,
    hardware_id: "1",
    title: "Beacon Title",
    created_at: "0:00:00",
    updated_at: "0:00:00"
}
```