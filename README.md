Fitness App SignUp will allow user to

    •	Register
    •	Login
    •	Get all employee details
    •	Get a particular employee detail
    •	Update password of an employee
    •	Delete an employee
    
Requirements
    Prerequisites
        You should have at least a basic understanding of Node, Express, MongoDB
        
    Install
        Lastly, make sure you have the following installed.
        
          •	Latest version of Node.js
          •	Latest version of NPM (Node Package Manage)
          •	Latest version of MongoDB 
          •	Azure Cosmos DB 
          •	Latest version of git (This is optional. It requires only if you choose to clone project)
          •	https://github.com/navindian/fitnessapp.git
          
       Set the path variables for mongoDB and npm
        
Getting Started

    1.	Either you can clone or download repository from GitHub.
    
              Clone with HTTPS (required git installed in your system)
                 git clone https://github.com/navindian/fitnessapp.git

              Clone with SSH (required git installed in your system)
                 git clone git@github.com: navindian/fitnessapp.git

              Download Zip
          
    2.	Navigate to project directory in the terminal or command prompt.
          
            cd fitnessapp
          
    3.	Install project dependencies
           
             npm i
           
    4.	Attach Database Account in Azure cosmos Db
         
            Set the connection string for the database as mongodb://127.0.0.1:27017
   
    5.	Run the backend server
          
            Node app.js

    6.	Project server is running at:
        	
            Backend server is running at http://localhost:4000
          
          
Backend APIs

    1.	Register
        Endpoint - http://localhost:4000/employee
        HTTP Method - POST
        Payload
        {
          “staffId”:"100003",
          “firstName”:”Helen”,
          “lastName”:”Paul”,
          “password”:”Abcd1234”
        }
      
    2.	Login
        Endpoint - http://localhost:4000/employee/verify 
        HTTP Method - POST
        Payload
        {
          “staffId”:"100003",
          “password”:”Abcd1234”
        }
      
    3.	Get All Employees
        Endpoint - http://localhost:4000/employee
    	  HTTP Method - GET
        
    4.	Get an Employee Detail based on ID
            Endpoint - http://localhost:4000/employee/id/:id
            HTTP Method - GET
            Parameter-id:100003

    5.	Update Password
            Endpoint - http://localhost:4000/employee
            HTTP Method - PUT
            Payload
            {
          “staffId”:"100003",
          “password”: ”Mnop5678”
        }

    6.	Delete an Employee
            Endpoint - http://localhost:4000/employee/:id
            HTTP Method - DELETE
          Parameter-id:100003


Contributing
1.	Fork it ( https://github.com/ navindian/fitnessapp/fork )
2.	Create your feature branch (git checkout -b my-new-feature)
3.	Commit your changes (git commit -am 'Add some feature')
4.	Push to the branch (git push origin my-new-feature)
5.	Create a new pull request.



