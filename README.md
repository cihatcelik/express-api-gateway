# express-api-gateway
My Express Gateway Template
<br>Express Gateway is a microservices API Gateway built on Express.js.

Endpoints : 
 <br>/cars endpoints get all cars and cars with id from cars fake api (https://myfakeapi.com/api)
 <br>/* call for endpoints fake api (https://dummyjson.com)

Examples : 
>>  ###### http://localhost:8080/cars (gets all cars from myfakeapi.com)
>> ###### http://localhost:8080/cars/5 (gets id=5 car from myfakeapi.com)
>
>>  ###### http://localhost:8080/products (gets all product from dummyjson.com)
>>  ###### http://localhost:8080/products?skip=10&limit=1 (gets product with filter from dummyjson.com)
>>  ###### http://localhost:8080/users (gets users from dummyjson.com)
>>  ###### http://localhost:8080/users?skip=10&limit=1 (get users with filter from dummyjson.com)
  
Rate Limiting
Example : Max 200 request in 120000 ms
```
 - rate-limit:
          - action:
              max: 200
              windowMs: 120000
              rateLimitBy: "${req.hostname}"
              message : "Too Many Request"
```

  
## Run Project

Clone Project

```bash
  git clone https://github.com/cihatcelik/express-api-gateway
```

Go to Folder

```bash
  cd express-api-gateway
```

Install Packages

```bash
  npm install
```

Run

```bash
  npm start
```

  
