### For the colors lab in COP4331

### Includes:
A log in page 

A user dashboard page which allows adding and searching for colors

Server endpoints (expected request and response json)

### Technology used:
Digital ocean LAMP (linux, apache, mysql, php) droplet. 

Regular html css js for the frontend

### Set up instructions (how to run and access application)
Create a digital ocean account and create a billing account.

Then create a LAMP droplet and allocate as many resouces as you need

### limitations
Currently on every search color server endpoint, it only requires the userId and search term, should also include a password or use a jwt.

### Add_color:

request:

{

  color: string,

  userId: int,

}

response:

{

  error: string

}

### login:

request:

{

  login: string,

  password: string,

}

response: 

{

  id: int,

  firstName: string,

  lastName: string,

  error: string,

}

### search color:

request:

{

  search: string,

  userId: int,

}

response:

{

  results: string[],

  error: string,

}
