### Learning with a REST API tutorial

#### Source:

`Build A REST API With Node.js, Express, & MongoDB - Quick`:  
https://www.youtube.com/watch?v=fgTGADljAeg&ab_channel=WebDevSimplified

#### Requirements:

MongoDB:

- Link for Ubuntu:  
  https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-ubuntu/

#### How to run:

- Check that mongod is running correctly:  
  ubuntu: `systemctl status mongod`

- Run API:
  `npm run devStart`

- Examples to run with `REST Client` VSCode plugin, use a `.rest` file extension
  - ids shown here are just placeholders

```json
GET http://localhost:3000/subscribers

###

GET http://localhost:3000/subscribers/65232fa1ff5667744c0ef7b6

###

POST http://localhost:3000/subscribers
Content-Type: application/json

{
  "name": "Some Person",
  "subscribedToChannel":"Web Dev Simplified"
}

###

DELETE http://localhost:3000/subscribers/65232fa1ff5667744c0ef7b6


###

PATCH http://localhost:3000/subscribers/6523e5a67fc49e3e90416c7c
Content-Type: application/json

{
  "name": "Some Person Different Name"
}
```
