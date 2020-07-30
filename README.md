# AWS-UniversityInformator
Implemented CRUD operation along with paginated search using Elastic Search, Lambda, API gateway in AWS

Steps followed to create this application:-

  1.Created domain for Elastic search and generated ES endpoint URL and Kibana URL
  2.Created and tested Elastic Search using Kibana 
  3.Connected Elastic Search with Lambda and developed code in python 
  4.Connected Lamba with API gateway and generated output with API gateway
 
 Attached files of screenshots from APi gateway and Lambda file code.
 Also showed one output of URL posted through postman
 
 Attachhing sample data for each CRUD operations and API Endpoint URL to test using curl or Postman:-
 
 
 1. Create Information :- https://dnrselt37g.execute-api.us-east-1.amazonaws.com/Prod/createuniversityinformation
  {
  "alpha_two_code": "US",
  "country": "USA",
  "domain": "cu.us",
  "name": "Carolina University",
  "web_page": "http://www.cu.us/"
  }
  
  2. Update Information :- https://76exqqxzk4.execute-api.us-east-1.amazonaws.com/Prod/updateuniversityinformation
  {
  "_id": "3",
  "alpha_two_code": "US",
  "country": "USA",
  "domain": "cu.us",
  "name": "Carolina University",
  "web_page": "http://www.cu.us/"
  }
  
  3. Search Information (Implemented Search on name along with liter as domain value) :-https://xamggj6p8j.execute-api.us-east-1.amazonaws.com/Prod/getuniversityinfo 
  {
  "name": "Washington",
  "domain_value": "edu"
  }
  
  4. Delete Information :- https://lhq4ipbec7.execute-api.us-east-1.amazonaws.com/Prod/deleteuniversityinfo
  {
   "_id": "2"
  }
  
  

  

