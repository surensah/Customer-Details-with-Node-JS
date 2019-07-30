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

Application "Hello World" Endpoint: https://skilled-curve-247615.appspot.com/

API endpoints:

/allCustomers endpoint: https://skilled-curve-247615.appspot.com/allCustomers

/customer?id=value endpoint with sample customer id's:

Customer with id: https://skilled-curve-247615.appspot.com/customer?id=103

Customer with id: https://skilled-curve-247615.appspot.com/customer?id=110

To Add New Customer into Datastore using Postman:

/customer endpoint: https://skilled-curve-247615.appspot.com/customer

sample input for add new customer {	"customerId":"106",	"name":"James",	"email":"james@bcci.com",	"phoneNumber":"+789219087" }
