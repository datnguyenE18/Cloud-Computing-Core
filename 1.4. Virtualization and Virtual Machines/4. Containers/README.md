# **Containers** 



- Containers are an executable unit of software in which application code is packaged, along with its libraries and dependencies, in common ways so that it can be run anywhere, whether it be on desktop, traditional IT, or the cloud.
 
- Containers are small, fast, and portable, and unlike virtual machines, they do not need to include a guest OS in every instance and can, instead, simply leverage the features and resources of the host OS



- Container là giải pháp để giải quyết vấn đề làm sao để chuyển giao phần mềm một cách đáng tin cậy (không phát sinh lỗi) giữa các môi trường máy tính khác nhau. Chẳng hạn như giữa máy tính của lập trình viên với máy của tester, giữa môi trường staging (hay còn được gọi là môi trường tiền thực tế) với môi trường thực tế hay thậm trí giữa máy chủ riêng đặt tại trung tâm dữ liệu với máy ảo trên Cloud 
 
- Container giải quyết vấn đề trên bằng cách tạo ra một môi trường bị cô lập (isolated) chứa mọi thứ mà phần mềm cần để có thể chạy được bao gồm mã nguồn, các thư viện runtime, các thư viện hệ thống, các công cụ hệ thống,… (gọi là sự phụ thuộc hoặc các phụ thuộc) mà không bị các yếu tố liên quan đến môi trường hệ thống làm ảnh hưởng tới cũng như không làm ảnh hưởng tới các phần còn lại của hệ thống.
 
- Whenever I mention containers, most people tend to default to something like Docker or even Kubernetes these days. But container technology has actually been around for quite some time
 
- Các Container sẽ ảo hóa ở cấp hệ điều hành. Trong đó nhiều Container chạy trực tiếp trên nhân hệ điều hành. Điều này có nghĩa là so với máy chủ ảo, các Container sẽ nhẹ hơn rất nhiều. Có được lợi ích này là do chúng chia sẻ nhân hệ điều hành dẫn đến việc khởi động nhanh hơn nhiều và sử dụng một phần nhỏ bộ nhớ so với khởi động toàn bộ hệ điều hành như máy chủ ảo thông thường

***

**Đặc điểm kỹ thuật** 

- Mô hình kiến trúc của container bao gồm các thành phần chính là Server (máy chủ vật lý hoặc máy ảo), host OS (hệ điều hành cài đặt trên server) và các container.



- Mỗi một ứng dụng (App A và App B) sẽ có những sự phụ thuộc riêng của nó bao gồm cả về phần mềm (các dịch vụ hay thư viện) lẫn cả về phần cứng (CPU, bộ nhớ, lưu trữ).



- Các ứng dụng này sẽ được Container Engine, một công cụ ảo hóa tinh gọn, được cài đặt trên host OS, nó sẽ cô lập sự phụ thuộc của các ứng dụng khác nhau bằng cách đóng gói chúng thành các container. Các tiến trình (process) trong một container bị cô lập với các tiến trình của các container khác trong cùng hệ thống tuy nhiên tất cả các container này đều chia sẻ kernel của host OS (dùng chung host OS).



- Với mô hình trên, sự phụ thuộc của ứng dụng vào tầng OS cũng như cơ sở hạ tầng được loại bỏ giúp việc triển khai phương pháp “deploy anywhere” (triển khai ở bất kỳ nơi đâu) của container được hiệu quả hơn. Thêm vào đó, do chia sẻ host OS nên container có thể được tạo gần như một cách tức thì, giúp việc scale-up & scale-down theo nhu cầu được thực hiện một cách nhanh chóng.

***

**Ưu điểm**

- **Môi trường nhất quán:** Container cung cấp cho các nhà phát triển khả năng tạo ra các môi trường có thể dự đoán được, tách biệt khỏi các ứng dụng khác. Container cũng có thể bao gồm các thành phần khác chẳng hạn như các thư viện phần mềm… điều này được đảm bảo nhất quán cho dù ứng dụng được triển khai ở bất cứ đâu
 
- **Tính phù hợp:** Các Container có thể chạy hầu như ở mọi nơi, giúp dễ dàng phát triển. Nó có thể chạy trên các hệ điều hành Linux, Windows và Mac. Hoặc trên máy ảo, trên máy của nhà phát triển hoặc trong các trung tâm dữ liệu. Và tất nhiên, trên cả các dịch vụ Public Cloud
 
- **Tính độc lập :** Các Container ảo hóa tài nguyên CPU, bộ nhớ, lưu trữ và mạng ở cấp hệ điều hành. Qua đó, nó cung cấp cho các nhà phát triển chế độ xem dưới dạng sandbox (hộp cát) về hệ điều hành được cô lập một cách hợp lý với các ứng dụng khác. Đây chính là điều mọi người hay nhầm lẫn với máy ảo khi tìm hiểu Container
