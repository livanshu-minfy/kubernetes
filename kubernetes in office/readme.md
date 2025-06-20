# readme.md file of kubernetes in office work

in this assignment I am deploying my first NGINX pod.

first I created a pod.yaml file and applied the manifest to the cluster using "kubectl apply -f pod.yaml"
![Screenshot 2025-06-19 173628](https://github.com/user-attachments/assets/72b166ce-46e2-4546-99be-86e8a283ac93)

then i checked the status using "kubectl get pods" and to get more details i used "kubectl get pods -o wide"
after that to view the application logs i used "kubectl logs nginx-pod"
![Screenshot 2025-06-19 173659](https://github.com/user-attachments/assets/f8642605-c7ba-4046-899f-1e5d904d249d)

it was written in the notion file that to get detailed information and events for troubleshooting purposes i can use "kubectl describe pod nginx-pod"
command , so I tried that too
![Screenshot 2025-06-19 173730](https://github.com/user-attachments/assets/503cce53-39af-46db-9aa6-aa8e7b96e433)
![Screenshot 2025-06-19 173741](https://github.com/user-attachments/assets/747d0175-dacb-4cce-ab71-536e9eb0df8f)


**----------------------------------------------------------**

then in second file to witness auto-healing and scaling, the first step was to create a file named "deployment.yaml"
after creating it i applied using "kubectl apply -f deployment.yaml"
i have also applies "kubectl get deployment", "kubectl get replicaset" and "kubectl get pods"

![Screenshot 2025-06-19 174144](https://github.com/user-attachments/assets/53675331-338d-4e48-b3da-2188caeeb4c8)

after doing this task i cleaned up carefully and stopped the minikube
