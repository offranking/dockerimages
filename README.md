# dockerimages
Working with docker images

### Begin the process by logging into the AWS Management Console, navigating to your EC2 instance, and connecting to it via SSH using your local terminal.
<img width="1433" height="401" alt="Screenshot 2025-08-06 at 5 00 07 am" src="https://github.com/user-attachments/assets/e2637b1f-5daa-4a7f-b19d-ae13e9ace482" />

### Now it's time to pull the Docker image you need using the following command: "docker pull"
<img width="842" height="119" alt="Screenshot 2025-08-06 at 5 14 03 am" src="https://github.com/user-attachments/assets/e2833fe6-a71c-464c-98ea-8f76100f413e" />

### On your local terminal, run the following command to search for Ubuntu-related images on Docker Hub: "docker search ubuntu"
<img width="1041" height="538" alt="Screenshot 2025-08-06 at 5 14 42 am" src="https://github.com/user-attachments/assets/7915847b-6149-4e2e-bb57-6a946f60ff1c" />

### Now we need to download the official Ubuntu image by running the following command: docker pull ubuntu
<img width="834" height="145" alt="Screenshot 2025-08-06 at 5 18 22 am" src="https://github.com/user-attachments/assets/48b25a59-ea64-4cc3-b513-73cef441b670" />

### To view the images that have been downloaded to your system, run the following command in your terminal and This will list all locally available Docker images, including their repository names, tags, image IDs, creation dates, and sizes "docker images"
<img width="961" height="140" alt="Screenshot 2025-08-06 at 5 20 31 am" src="https://github.com/user-attachments/assets/a0c6f744-0bfa-4ac4-9539-6072ed845594" />

### In this step, you need to create a Dockerfile. and index.html and let paste in some text. run the commmand 
"touch dockerfile" on the local terminal and "touch index.html"

<img width="728" height="143" alt="Screenshot 2025-08-06 at 5 37 41 am" src="https://github.com/user-attachments/assets/32eb1d4b-5025-4f68-b0d1-3fe6cb5f8ebf" />

### open the text and paste in some code 
to open the file run the command "vim dockerfile" and "vim index.html"



<img width="749" height="900" alt="Screenshot 2025-08-06 at 5 34 07 am" src="https://github.com/user-attachments/assets/ded0efbe-747b-42e1-9105-6bd648f7f2a3" />

### And 

<img width="338" height="900" alt="Screenshot 2025-08-06 at 5 36 18 am" src="https://github.com/user-attachments/assets/e7ef2b1f-5e99-40ac-853f-7f2f31b26953" />


### To build the Docker image from your Dockerfile, run the following command in your terminal from the directory where the Dockerfile is located
run command "docker build -t dockerfile"

<img width="1440" height="690" alt="Screenshot 2025-08-06 at 5 41 29 am" src="https://github.com/user-attachments/assets/b68b8d9d-f4c7-4775-bd2e-b0b707e9f10d" />

### run docker images to see the images and the id

<img width="910" height="160" alt="Screenshot 2025-08-06 at 5 44 27 am" src="https://github.com/user-attachments/assets/d23c6934-937a-4be2-89a7-f3cf3982f19f" />

### To run a container based on the NGINX image you created using your Dockerfile, use the following command "docker run -p 8080:80 dockerfile"

<img width="951" height="432" alt="Screenshot 2025-08-06 at 5 47 02 am" src="https://github.com/user-attachments/assets/c56016e8-67f0-4280-bfce-16ce1cb26826" />

### On this step, you need to access your EC2 instance’s security group to configure inbound rules:


<img width="1245" height="264" alt="Screenshot 2025-08-06 at 5 48 52 am" src="https://github.com/user-attachments/assets/ca057b09-6721-49ee-9a0e-bb986242b70f" />

### Edit inbound rules.



<img width="1437" height="451" alt="Screenshot 2025-08-06 at 5 52 10 am" src="https://github.com/user-attachments/assets/6c69cd19-1c39-4040-832d-fa50e5428e7a" />

### Add the new rule

<img width="1413" height="453" alt="Screenshot 2025-08-06 at 5 54 13 am" src="https://github.com/user-attachments/assets/da6123ca-1275-42e9-a49e-25007b5c5a9f" />


### To list all available containers "docker ps -a"

<img width="1256" height="142" alt="Screenshot 2025-08-06 at 5 57 05 am" src="https://github.com/user-attachments/assets/8cac5dec-452d-4bd2-aef5-d50fe7c59216" />

### to check the containers run docker start with the containers ID "docker start"
<img width="1282" height="62" alt="Screenshot 2025-08-06 at 5 59 40 am" src="https://github.com/user-attachments/assets/e701f19c-7f88-4cd3-922c-55ef7f123c57" />


### after that run docker ps -a


<img width="1425" height="139" alt="Screenshot 2025-08-06 at 6 02 04 am" src="https://github.com/user-attachments/assets/f75e0bce-c417-4446-9fa1-a3980909e4e0" />

### now we need to gain access to out web browser by using the public iP http://3.85.162.93:8080




<img width="1440" height="856" alt="Screenshot 2025-08-06 at 6 04 50 am" src="https://github.com/user-attachments/assets/6dbf23a2-83bb-42c0-b1c2-f1377f7c0aee" />

### Now, you need to create a repository on Docker Hub to store and share your Docker images.



<img width="1180" height="600" alt="Screenshot 2025-08-06 at 7 32 24 am" src="https://github.com/user-attachments/assets/8be94a6a-4f77-475f-8bea-7e83b61a8727" />

### now we have to tag the repository on docker hub

<img width="1021" height="59" alt="Screenshot 2025-08-06 at 6 19 10 am" src="https://github.com/user-attachments/assets/47647452-a4e1-4425-803c-048ba3b1994f" />
<img width="1437" height="705" alt="Screenshot 2025-08-06 at 6 26 11 am" src="https://github.com/user-attachments/assets/ff719e29-a2c6-4774-b1fa-ff8128f82b33" />



<img width="1177" height="519" alt="Screenshot 2025-08-06 at 6 17 09 am" src="https://github.com/user-attachments/assets/c7d23624-67c5-40c8-bc3a-7d30410dc43f" />


now we have to push the container in to docker hub

<img width="1175" height="268" alt="Screenshot 2025-08-06 at 6 22 22 am" src="https://github.com/user-attachments/assets/19afabcd-40b2-452f-9695-e65e59daac71" />

 






