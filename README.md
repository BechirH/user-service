# user-service

API tests 
POST http://localhost:8080/api/auth/register
{
  "username": "test",
  "password": "test123" 
}

this will create user named test and assign default role "USER_ROLE" that has "USER_READ", "USER_UPDATE"  permessions 



POST http://localhost:8080/api/auth/login
{
  "username": "test",
  "password": "test123" 
}

get repond with your Bearer token 

GET http://localhost:8080/api/users  ( require "USER_READ" permession) 

will reply with list of users 


GET http://localhost:8080/api/roles  ( require "ROLE_READ" permession)

will reply with 403 message 

GET http://localhost:8080/api/permissions

 will reply with 403 message 
