# kubernetes-dashboard

Kubernetes Dashboard là một giao diện web để quản lý các tài nguyên Kubernetes một cách trực quan. Nó cung cấp cho người dùng một cách tiện lợi để xem và quản lý các ứng dụng và tài nguyên của Kubernetes mà không cần phải sử dụng các câu lệnh dòng lệnh phức tạp. Với Kubernetes Dashboard, người dùng có thể xem và quản lý các Pod, ReplicaSet, Service, Deployment và nhiều tài nguyên khác của Kubernetes. Nó được cài đặt bằng cách triển khai một Deployment trong Kubernetes cluster và sử dụng một Service để truy cập giao diện. Kubernetes Dashboard cũng hỗ trợ tính năng tìm kiếm và lọc tài nguyên để giúp người dùng dễ dàng tìm kiếm các tài nguyên một cách nhanh chóng.


```
kubectl apply -f recommended.yaml
kubectl apply -f dashboard-admin.yaml
kubectl apply -f components.yaml
kubectl apply -f dashboard-admin-bind-cluster-role.yaml
```
