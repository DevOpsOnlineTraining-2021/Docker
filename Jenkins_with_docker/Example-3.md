Step-1: Make sure jenkins and node configured - perform Step-1 to Step-3 from [Example-1](Example-1.md)


Step-2: Create a new pipeline job and add configure below Git repo URL.

      Git repo URL: https://github.com/venkatasykam/DevOpsWebApp.git
      Git Branch: containerized-build2
      Jenkinsfile: https://github.com/venkatasykam/DevOpsWebApp/blob/containerized-build2/Jenkinsfile
      Dockerfile: https://github.com/venkatasykam/DevOpsWebApp/blob/containerized-build2/Dockerfile

Step-3: Execute the job and observer the build console output.


![image](https://user-images.githubusercontent.com/24622526/133076494-9b16976f-9a5f-409b-9110-706c50ff95f9.png)


**On server (jenkins node)**:

![image](https://user-images.githubusercontent.com/24622526/133076769-437b69e1-047a-4e0a-b2f1-3343361c00e8.png)

