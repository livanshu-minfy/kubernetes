# this is readme.md file of kubernetes take home assignment

in this assignment we are setting up mongoDB database backend
the first step is to generate Base64-Encoded credentials

![Screenshot 2025-06-20 190356](https://github.com/user-attachments/assets/dfb6ec47-5d3d-43bd-ad86-a37dc24edcae)

next I created livanshu-mongo-secret.yaml file and applied it using **"kubectl apply -f livanshu-mongo-secret.yaml"** and then
checked secret's creation using **"kubectl get secret"**.

![image](https://github.com/user-attachments/assets/1b9f51ff-56c3-4ad8-9988-93c9d75b5d04)

then i created livanshu-mongo-deployment.yaml file and applied the configuration using **"kubectl apply -f livanshu-mongo-deployment.yaml"**
and verified deployment using **"kubectl get all"**.

![image](https://github.com/user-attachments/assets/cd228838-0d69-4035-b151-56500fae9675)

then i created livanshu-mongo-configmap.yaml file and applied the configuration using **"kubectl apply -f livanshu-mongo-configmap.yaml"**
and applied configmap using **"kubectl get configmap"**.

![image](https://github.com/user-attachments/assets/a7b56ba5-c19c-4956-9f06-1ce40c4da5ce)

and then i created livanshu-mongo-express.yaml file and applied the configuration using **"kubectl apply -f livanshu-mongo-express.yaml"**
and verified using **"kubectl get all"** and added auto auth too.

![image](https://github.com/user-attachments/assets/69848a05-8774-4e80-aba6-53800e1149e7)

after that i got the service url using **"minikube service mongo-express-service"**.

![image](https://github.com/user-attachments/assets/29f1d3ec-bf13-452b-ad27-aba6b82a0d0b)

which opened this browser window

![image](https://github.com/user-attachments/assets/39f30397-5652-4408-b99b-5eec24f5226a)

and after filling the credentials i got mogo db

![image](https://github.com/user-attachments/assets/cea160d6-c236-4878-88d6-dbf8af01648e)

then I created a new database and a new collection to confirm that your my application is successfully communicating with the MongoDB backend.

![image](https://github.com/user-attachments/assets/82ae6615-ad50-4785-9bf5-818049790462)
![image](https://github.com/user-attachments/assets/7b23342f-61e1-469f-beff-842883536bc9)

after this last and final step i.e. **cleanup**

![image](https://github.com/user-attachments/assets/4f5bf424-bf33-4cae-be8b-81f40821519e)
