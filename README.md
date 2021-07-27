# Pro-MERN-Stack-IssueTracker-API-Deploy

### Changes for Heroku
* /server.js: Change in Environment Variable Name for Server Port.
* api/sample.env: Change in Variable Name for Server Port.
* /api_handler.js: Enable GraphQL Playground in Production.
* /package.json: Engine Specification for Heroku.

### Connected to MongoDB
* use Atlas
* whitelist my IP address
* connect to my app with MongoDB by setting heroku config
* initialize could database with init.mongo.js and generate_data_mongo.js.

### Command
* $ heroku create tracker-api-sophiafan
* $ heroku config:set \
DB_URL=$DB_URL \  (mongodb+srv://<username>:<password>@cluster0.yh6ey.mongodb.net/myFirstDatabase?retryWrites=true&w=majority)
JWT_SECRET=YOUR_SPECIAL_SECRET \
COOKIE_DOMAIN=herokuapp.com
* $ git push heroku main
* $ heroku logs (to troubleshoot)

### skip non-proxy deployment