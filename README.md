# Customer-Details-with-Node-JS

Initially created a datastore with (kind) "customer" with few attributes like customerId, email, name, phoneNumber

By using nodejs and express framework:

## Created 3 apis:
/allCustomers - api to fetch customers details from datastore
/customer?id-value - api to fetch specific customer detail from datastore
/customer - api to create new customer detail into datastore
Local Usage: Prerequisite: Node modules should be installed on local machine

npm init //It creates package.json file

For dependencies add

npm i --save module-name (express,body-parser)

npm install //to add all dependencies

npm start //command to run locally

GCloud SDK Usage: Initialized gcloud sdk before deploying application into app engine

$gcloud auth login

$gcloud config set project projectId

Used app engine "standard environment" to deploy the application for deploying use command

$gcloud app deploy(google sdk)

$gcloud app browse

Application "Hello World" Endpoint: https://earnest-crow-243811.appspot.com

API endpoints:

/allCustomers endpoint: https://nodejs-customer-243619.appspot.com/getCustomers

/customer?id=value endpoint with sample customer id's:

getCustomer with id:http://localhost:3000/customer?id=108

getCustomer with id:https://nodejs-customer-243619.appspot.com/getCustomer?id=153242

getCustomer with id:https://nodejs-customer-243619.appspot.com/getCustomer?id=153243

/postCustomer endpoint: https://nodejs-customer-243619.appspot.com/postCustomer

sample input for post customer { "custId":153244, "email":"chris.barnod@ikea.com", "firstName":"Chris", "lastName":"Barnod", "phone":"+46722222222" }
