# **Secure Networking in Cloud**

- The notion of building a cloud network is not much different from deploying a network in an on-premises data center
 
- We use logical instances of networking elements as opposed to physical devices. For example, Network Interface Controllers (NICs) would be represented by vNICs in cloud environments
 
- To create a network in the cloud, one starts by defining the size of the network, or the IP address range that establishes the boundaries or the cloud network
 
- Logically segmented cloud networks are private carveout of the cloud that offer customers the security of private clouds and the scalability of public clouds
 
- Cloud resources, such as VMs or Virtual Server Instances (VSIs), storage, network connectivity and load balancers are deployed into subnets. 
 
- Subnets ( part of a logically segmented cloud network ) is the main area where security is implemented
 
- **Private Cloud**
 
  Private cloud có thể được đặt tại các data center của khách hàng hoặc co-location tại nhà cung cấp dịch vụ. Workload của khách hàng chạy trên các máy chủ vật lý riêng biệt, kho lưu trữ vật lý riêng biệt và vào level của các thiết bị kết nối vật lý riêng biệt, được tổng hợp lại thành một shared network, có thể là một backbone local area network hoặc shared Internet. Khách hàng có thể chọn để kết nối với Internet, kết nối mạng private cho truy cập từ bên ngoài hoặc kết nối với cả hai.


- **Public Cloud**
 
  Public Cloud được đặt tại các data center của nhà cung cấp dịch vụ và được đặt tại nhiều vị trí địa lý khác nhau. Workload của khách hàng chạy trên các máy chủ vật lý như các khách hàng khác, kho lưu trữ vật lý được chia sẻ giữa các khách hàng và kết nối vật lý cũng được chia sẻ. Tuy nhiên, ngay cả với mức độ về chia sẻ vật lý, điều này không có nghĩa là một khách hàng có thể truy cập vào hệ thống của khách hàng khác.
  
  Ở cấp độ máy chủ, hypervisor được sử dụng để tạo ra các máy chủ logic trên các máy chủ vật lý. Những máy chủ logic này được gọi là máy ảo (VM – virtual machine) được cô lập và đặt trên Virtual Local Area Networks (VLANs) của khách hàng. Kho lưu trữ được ngăn cách bởi zone và data store hoặc logical unit cho mỗi máy ảo. Theo mặc định, các máy ảo và VLAN không cho phép các máy ảo giao tiếp với bất cứ điều gì. Điều này sẽ không tạo ra giá trị nếu các máy ảo hoàn toàn bị cô lập, vì vậy khách hàng – client (chứ không phải là nhà cung cấp – provider), bao gồm cả security team, xác định VLAN mà mỗi VM nên giao tiếp và quy định các quy tắc cho các giao thức (protocol), port và tường lửa (firewall) có thể được sử dụng.
  
  Nhà cung cấp dịch vụ thiết lập các mức truy cập quản trị điển hình thông qua NIC card riêng biệt và các VM được chỉ định cho việc quản trị. Nhưng việc truy cập đến các dịch vụ cần thiết của các nhà cung cấp dịch vụ sẽ bị hạn chế. IBM Cloud Managed Services cung cấp các nhiệm vụ riêng lẻ cho các admin để đảm bảo công tác bảo mật của đội ngũ hỗ trợ hypervisor, operating system, network.


- **Hybrid Cloud**
 
  Hybrid cloud chỉ đơn giản một phần trong cơ sở hạ tầng của khách hàng, nằm giữa private cloud và public cloud. IBM Cloud Managed Services bao gồm việc đặt các máy ảo trên một phần mở rộng của network, được gọi là extended premises (EP) network. Nhiều khách hàng kết nối với EP network đã trở lại IT infrastructure truyền thống hoặc data center private cloud, và khách hàng có toàn quyền kiểm soát bất kỳ quy tắc firewall mà họ muốn thiết lập cho public cloud VM.
