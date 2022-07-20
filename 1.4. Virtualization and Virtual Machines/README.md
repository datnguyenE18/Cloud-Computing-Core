# **Virtualization and Virtual Machines**


- **Virtualization** is the process of creating a software based or virtual version of something whether that be compute, storage, networking, servers, or applications and what makes virtualization feasible, is something called the hypervisor. 

  Ảo hóa là quá trình tạo ra một bản sao ảo của một thực thể nào đó. Ảo trong trường hợp này có nghĩa là một cái gì đó rất giống với bản gốc, giống đến nỗi mà hầu như không thể phân biệt được nó với bản gốc.

  Trong CNTT thì ảo hóa là một công nghệ được thiết kế để tạo ra tầng trung gian giữa hệ thống phần cứng máy tính và phần mềm chạy trên nó. 
  Ý tưởng của công nghệ ảo hóa máy chủ là từ một máy vật lý đơn lẻ có thể tạo thành nhiều máy ảo độc lập. Mỗi một máy ảo đều có một thiết lập nguồn hệ thống riêng rẽ, hệ điều hành riêng và các ứng dụng riêng. 
  Ảo hóa có nguồn gốc từ việc phân chia ổ đĩa, chúng phân chia một máy chủ thực thành nhiều máy chủ logic. Một khi máy chủ thực được chia, mỗi máy chủ logic có thể chạy một hệ điều hành và các ứng dụng độc lập



- **Hypervisor**'s simply a piece of software that runs above the physical server, or host. 
 
- **2 types of hypervisors:**
  - Type 1: A hypervisor that is installed directly on top of the physical server. They're also called bare-metal hypervisors. (these are the most frequently typed of use hypervisors and they're most secure, they lower the latency)
 
  - Type 2: there is a layer of host OS that sits between the physical server and the hypervisor. By that nature they are also called, Hosted (These are a lot less frequent. They're mostly used for end-user virtualization. They're a lot less frequent. They have a higher latency than a Type 1 hypervisor)



- **A VM** is simply a software based computer. They're run like a physical computer. They have an operating system and applications, and they're completely independent of one another, but you can run multiple of them on a hypervisor and the hypervisor manages the resources that are allocated to these virtual environments from the physical server. Because they're independent you can run different operating systems on different virtual machines
 
  Máy ảo là một chương trình đóng vai trò như một máy vi tính ảo. Nó chạy trên hệ điều hành hiện tại - hệ điều hành chủ và cung cấp phần cứng ảo tới hệ điều hành khách. Các hệ điều hành khách chạy trên các cửa sổ của hệ điều hành chủ, giống như bất kỳ chương trình nào khác của máy. Đối với những hệ điều hành khách, máy ảo lại hiện diện như một cỗ máy vật lý thực sự.
  
  Các máy ảo cung cấp phần cứng ảo, bao gồm CPU ảo, RAM ảo, ổ đĩa cứng, giao diện mạng và những thiết bị khác. Các thiết bị phần cứng ảo được cung cấp bởi máy ảo và được ánh xạ tới phần cứng thực trên máy thật. Ví dụ như, ổ đĩa cứng ảo lại được lưu trong một file đặt trên ổ đĩa cứng thực.
