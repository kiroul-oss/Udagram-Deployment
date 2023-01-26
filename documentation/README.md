## pipeline process

- I create `package.json` file in the root of project and added all scripts for installing, building, testing and deploying for frontend and backend to make it easy to automate the scripts 
- I create new Repo in github `udacity-deployment` and connected it to my account in circleci
- I did not put any hard coded enviroment variables but I add them to circleci
- I create `.circleci/config.yml` and put all configrations:


## Inside CircleCI

### in .circleci/config.yml file
- I put all orbs we need for setting up the server we need in orbs (node.js, AWS, EB).so, I put them
- setting up  all software used in our pipeline process which are `(node.js, yarn, checkout, aws-cli, EB)`
- I added the jobs in it for installing, building, testing and deploying for both frontend and backend by calling the corresponding scripts in `package.json` file in the root of project
- I also added the `workflow` section to make the pipeline process only triggered when I push to the main branch in Github Repo

## I put screenshots for my circleci account in the same directory showing that is pass all jobs successfully

## and also added the pipeline diagram 