# Valid Requests To Registrations #


## *Post Request To /registrations* ##
> Credentials are sent through the headers
```json
{ 
    email: "example.com",
    password: "*****"
}
```

## *Facebook Users* ##
> Credentials are sent through the headers
> Cookie is obtained from successful request to "https://www.makeschool.com/users/auth/facebook"
> Taking the cookie value for _makschool_session=
```json
{
    Cookie: "_makeschool_session=*******",
    email: "example.com"
}
```

