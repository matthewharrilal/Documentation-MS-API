# CRUD on Beacons #
*Authorized Requests => Need Token Representation of Yourself* 

## *Post Request made to /beacons* ##
```json
{ 
    hardware_id: "Integer Value Representing the Beacon's Hardware ID",
    title: "Title of The Corresponding Beacon"
}
```

## Collection of Beacons ##
*To see all available beacons =>  GET /beacons*
```json
[
    {   
    id: 1,
    hardware_id: "1",
    title: "Beacon Title",
    created_at: "0:00:00",
    updated_at: "0:00:00"
},
{   
    id: 2,
    hardware_id: "2",
    title: "Beacon Title",
    created_at: "0:00:00",
    updated_at: "0:00:00"
},
{   
    id: 2,
    hardware_id: "2",
    title: "Beacon Title",
    created_at: "0:00:00",
    updated_at: "0:00:00"
}
]
```


## Specific Beacon ##
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

## Delete Beacon ##
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