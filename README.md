# jenkins_nodejs_test
just for jenkins build testing
 
### build Error

    npm install
    node app error

### build Success

    npm install
    node app 

### build Success but test Error
    
    npm install
    node app
    mocha test/error.js

### build Success and test Success

    npm install
    node app
    mocha test/success.js
