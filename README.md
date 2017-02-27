#Money Tree APIs

##Datalayer

Note: this is a simple json server and does not applies any validations or security

####Using data layer

####Installation:
Install json-server globally using
npm install json-server -g

####Running:
Run npm start

####Usage

Get all users 
GET: http://localhost:3000/users

Get user by username and password
GET: http://localhost:3000/users?username=pkaus2&password=password2

Add new user
POST: http://localhost:3000/securities
with Content-Type: application/json and json data

Get all securities
GET: http://localhost:3000/securities

Search securities by security name
GET http://localhost:3000/securities?name_like=ro where ro is the part of name to be looked up

Search securities by security symbol
GET http://localhost:3000/securities?symbol_like=ro where ro is the part of name to be looked up

Add a new order
POST: http://localhost:3000/orders
This does not validates anything.
{
	"symbol": "INFY",
	"type": "MARKET",
	"side": "BUY",
	"limitPrice": 0,
	"stopPrice": 0,
	"quantity": 10
}

GET all orders
GET: http://localhost:3000/orders

Update orders block id
http://localhost:3000/orders/<orderID>
{
    blockID: 1
}





