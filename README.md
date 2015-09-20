https://pythonhosted.org/Flask-JWT/

POST /auth
Content-Type: application/json

{
    "username": "joe",
    "password": "pass"
}

HTTP/1.1 200 OK
Content-Type: application/json

{
  "token": "<jwt-token>"
}


GET /protected
Authorization: Bearer <jwt-token>

HTTP/1.1 200 OK

Success!