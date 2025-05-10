User Service
Base URL: /
POST /register
Registers a new user and returns a JWT token.
Request:
{
  "username": "john",
  "password": "secret"
}
Response:
{
  "access_token": "..."
}
GET /profile
Returns user profile (JWT required).
Headers:
Authorization: Bearer <access_token>
Response:
{
  "msg": "Welcome to your profile!"
}# UserService
Handles user registration, login, profile management
