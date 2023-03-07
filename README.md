## Kubernetes Dashboard

Kubernetes Dashboard là một giao diện web để quản lý các tài nguyên Kubernetes một cách trực quan. Nó cung cấp cho người dùng một cách tiện lợi để xem và quản lý các ứng dụng và tài nguyên của Kubernetes mà không cần phải sử dụng các câu lệnh dòng lệnh phức tạp. Với Kubernetes Dashboard, người dùng có thể xem và quản lý các Pod, ReplicaSet, Service, Deployment và nhiều tài nguyên khác của Kubernetes. Nó được cài đặt bằng cách triển khai một Deployment trong Kubernetes cluster và sử dụng một Service để truy cập giao diện. Kubernetes Dashboard cũng hỗ trợ tính năng tìm kiếm và lọc tài nguyên để giúp người dùng dễ dàng tìm kiếm các tài nguyên một cách nhanh chóng.

<figure><img src="https://i.imgur.com/oPHagei.png" alt=""><figcaption></figcaption></figure>

### Cách cài đặt

```
git clone https://github.com/beta21s/kubernetes-dashboard.git
cd kubernetes-dashboard

kubectl apply -f recommended.yaml
kubectl apply -f dashboard-admin.yaml
kubectl apply -f components.yaml
kubectl apply -f dashboard-admin-bind-cluster-role.yaml
```

### Cách lấy tolken

``` 
kubectl -n kubernetes-dashboard create token admin-user --duration=488h
```

Kết quả nhận được như bên dưới
```
root@master:/home/ubuntu/dashboard#  kubectl -n kubernetes-dashboard create token admin-user --duration=488h
eyJhbGciOiJSUzI1NiIsImtpZCI6Ik9JVjl2c3pGTWFZNjJaNTJna3JQRkdqUm1YNENuTmtJcjNkN1RRMVhnQmMifQ.eyJhdWQiOlsiaHR0cHM6Ly9rdWJlcm5ldGVzLmRlZmF1bHQuc3ZjLmNsdXN0ZXIubG9jYWwiXSwiZXhwIjoxNjc5ODc3OTM5LCJpYXQiOjE2NzgxMjExMzksImlzcyI6Imh0dHBzOi8va3ViZXJuZXRlcy5kZWZhdWx0LnN2Yy5jbHVzdGVyLmxvY2FsIiwia3ViZXJuZXRlcy5pbyI6eyJuYW1lc3BhY2UiOiJrdWJlcm5ldGVzLWRhc2hib2FyZCIsInNlcnZpY2VhY2NvdW50Ijp7Im5hbWUiOiJhZG1pbi11c2VyIiwidWlkIjoiNmEyNjQ5ODItOTk1Mi00OTdmLTg4NDMtYTBlYzg1Y2RjNmFjIn19LCJuYmYiOjE2NzgxMjExMzksInN1YiI6InN5c3RlbTpzZXJ2aWNlYWNjb3VudDprdWJlcm5ldGVzLWRhc2hib2FyZDphZG1pbi11c2VyIn0.U0bcDvB4Z0GugF7VFWrOUvF6t9UxkxoJbXhTQwxxtGNWvBvpv7etuCu8VO_uWTwLqy8vlLo2kD4qHN0AsVfnxAJ6Pwkg32g78w9SEj5Te3AihrDdOlg__L7FWDTOUgSBbxVZwa786ZXDlVNV5JwjdxibxKOWCibYD6wdhnVKujy8w400Kv75uJ6xTed6Xf1SWbdmXn9jH7gryWwYruOWM0xcPqTIBn7tmSkbUOmM_eQyjc8SZbEMAAHQ-3a2zlgnmDepAIkfsYLzLuw3toeR3xKcD5b-Jew0EOQ0zEHJBFaNJhn8-OrXAJCkAJOcMNmORNt-6mbkH--Jr3T89EcMcA
```

<figure><img src="https://i.imgur.com/5YEmj5F.png" alt=""><figcaption></figcaption></figure>
