# Automated-Code-Quality-Workflows-GitHub-Actions-and-SonarQube-on-Azure-Cloud
Ensure that all code changes are automatically tested for quality and security issues before they are deployed to production. You decide to use SonarQube for static code analysis and GitHub Actions to automate the workflow, all of which are deployed on an Azure VM using Docker.

# Technologies Used
1. SonarQube: A tool for continuous code quality inspection that performs automatic code reviews using static analysis to find bugs, code smells, and security issues.
2. GitHub Actions: A CI/CD service that allows you to automate tasks within your software development lifecycle, such as building, testing, and deploying code.
3. Azure Cloud: A comprehensive set of cloud services that developers and IT professionals use to build, deploy, and manage applications through Microsoft’s global network of data centers.
4. Docker: A platform that allows developers to build, share, and run programs in containers, ensuring a consistent environment across development and production.

<hr style="border:2px solid gray">

🔸Docker Installation Commands:

```
sudo apt-get update
sudo apt-get install -y docker.io
sudo systemctl start docker
sudo systemctl enable docker
```

🔸Verify the docker is installed and active:
```
sudo systemctl status docker
```


🔸Create a Docker Container for SonarQube:
````
sudo docker run -d --name sonarqube -p 9000:9000 sonarqube:latest
````

🔸Access SonarQube: 
```
Open your browser and navigate to http://<vm_ip>:9000 to access the SonarQube interface.
```



