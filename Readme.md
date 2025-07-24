## Introduction 
This project demostrates using GitHub Action as continuous integration and continuous delivery (CI/CD) platform to automate build, test, and deployment pipeline to test Rest Api using Postman. <br>
![screenshot](/img/github-actions-cicd-postman-test.drawio.png)

### Postman
exported from postman <br>
Postman collection test - ReqResApiTest.postman_collection.json <br>
Postman environment file - reqres.postman_environment.json <br>

### Pipeline workflow
.github\workflows <br>

Workflow Tigger by push event or by manual trigger on Github action tab "run workflow" button
- GitHub-hosted runners: Linux ubuntu
- Check out the code from the current repository.
- Install Nodejs for dependencies installations
- Install Newman
- Install Newman htmlextra reporter
- Running the collection
- Upload Newman report into the directory