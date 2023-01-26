## In the application

* I install all dependancies and run the scripts for building, testing and added the script for deploy in both the frontend and backend

* I initiate the eb cli in the project by `eb init` and put all credintiles

## In AWS 

* first of all I create IAM credintiles to access the aws from cli commands

* I create an instance from RDS postgres database its name is `database-3` where its endpoint is `database-3.cmq6iq7khhix.us-east-1.rds.amazonaws.com`

* I also create new application in elastic beanstalk its name is `post-posts` and put all enviroment properties in it and it send requests to our RDS database and then retrive data from it and it return response to front end in S3 bucket and this is its link `(http://post-posts.s3-website-us-east-1.amazonaws.com)` where the backend server is running on.
`
* I also create S3 bucket and put all frontend files which it host the frontend and the user an send requests for the server in elasticbeanstalk and get back the response as HTML pages for user and I make it public access so we can run it from anywhere and put the sutaible bucket policy and enable Static website hosting where its endpoint to access it is:(http://post-posts.s3-website-us-east-1.amazonaws.com/)

### the Architecture diagram is added in the same directory which showing the infrastructure and also I added screenshots from AWS console for each sevices
