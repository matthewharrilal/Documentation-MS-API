# CRUD on Beacons #

## *Post Request made to /beacons* ##
```json
{ 
    hardware_id: "Integer Value Representing the Beacon's Hardware ID",
    title: "Title of The Corresponding Beacon"
}
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