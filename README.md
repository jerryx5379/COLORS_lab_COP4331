For the colors lab in COP4331

Includes:
A log in page 
A user dashboard page which allows adding and searching for colors

Server endpoints (expected request and response json)
Add_color:
request:
{
  color: string,
  userId: int,
}
response:
{
  error: string
}

login:
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

search color:
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
