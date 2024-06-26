---
title : "19-06-2024"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b>  </b> "
---
**Cloud Computing là gì** Điện toán đám mây là việc phân phối các tài nguyên CNTT theo nhu cầu qua internet với chính sách thanh toán theo mức sử dụng.

**Lợi ích của điện toán đám mây** 
- Sử dụng bao nhiêu tính tiền bấy nhiêu, cung cấp khả năng tối ưu hóa chi phí
- Tăng tốc độ phát triển nhờ tận dụng các tính năng tự động hóa và  quản trị bởi nhà cung cấp dịch vụ 
- Linh hoạt
- Mở rộng qui mô ứng dụng lên toàn cầu
- 
**AWS khác biệt?**
- Là nhà cung cấp hạ tầng cloud dẫn đầu trong 13 năm liên tiếp 
- Khác biệt về tầm nhìn và giá 
- Triết lý về giá của AWS: Khách hàng sẽ chi trả càng ngày càng ít tiền cho cùng 1 dịch vụ, tính năng, tài nguyên sử dụng
- Mang lại giá trị thực sự cho khách hàng lên hàng đầu trong tất cả các nguyên tắc lãnh đạo ( Leadership Principles )
![19-6](/images/19-6-2024/1-19-6.png)
**Trung tâm dữ liệu của AWS**

    1 trung tâm dữ liệu có thể chứa hàng chục ngàn máy chủ 

    Tất cả trung tâm dữ liệu của AWS đều sử dụng các thiết bị được tối ưu hóa dành riêng cho hoạt động của AWS

- Availability zone
![19-6](/images/19-6-2024/2-19-6.png)

    1 AZ bao gồm 1 hoặc nhiều trung tâm dữ liệu , các AZ được thiết kế để không xảy ra sự cố ảnh hưởng đồng thời 2 AZ một lúc ( Fault isolation ).

    Giữa 2 AZ là đường kết nối riêng có tốc độ cao.

    AWS khuyến nghị nên triển khai ứng dụng tối thiểu trên 2 AZ.

- Region
![19-6](/images/19-6-2024/3-19-6.png)

    Một AWS Region bao gồm tối thiểu 3 Availability Zone (AZ). Hiện tại có hơn 25 Region trên toàn cầu.

    Các Region được kết nối với nhau bởi mạng backbone của AWS.

    Mặc định dữ liệu và dịch vụ ở các Region độc lập với nhau.

- Edge Locations 

    Là mạng lưới trung tâm dữ liệu AWS được thiết kế để cung cấp dịch vụ với độ trễ thấp nhất có thể 

    Các dịch vụ AWS hoạt động tại Edge location (POP) bao gồm:

    CloudFront (CDN)

    Web Application Firewall (WAF)

    Route 53 (DNS Service)

**Công cụ quản lí AWS service**
- AWS CLI
    Cho phép tương tác với các dịch vụ AWS bằng các lệnh command
- AWS SDK
![19-6](/images/19-6-2024/4-19-6.png)   

AWS SDK đơn giản hóa việc sử dụng AWS Service cho ứng dụng bằng cách cung cấp một bộ thư viện nhất quán và quen thuộc cho đội ngũ phát triển ứng dụng

AWS SDK cung cấp hỗ trợ cho những công việc quản lí vòng đời của API tới AWS Service như quản lí thông tin xác thực (Manage Credentials ), thử lại (retry), sắp xếp dữ liệu ( data marshalling - chuẩn bị dữ liệu), tuần tự hóa ( Serialization chuyển object sang bytes stream) và giải mã hóa ( deserialization chuyển bytes stream về lại object )

**Tối ưu hóa chi phí trên AWS**

    Lựa chọn cấu hình tài nguyên tính toán và nơi lưu trữ dữ liệu phù hợp

    Tận dụng các phương thức thanh toán giảm giá như reserved instance, saving plan, spot 

    Xóa các tài nguyên không sử dụng, bật tắt tự động các tài nguyên không cần chạy 24/7 

    Tận dụng các dịch vụ serverless

    Thiết kế kiến trúc tối ưu giải quyết các yêu cầu đề ra

    Cài đặt và sử dụng AWS Budget

    Quản lí chi phí theo phòng ban / ứng dụng với cost allocation tag 

    Liên tục theo dõi và tối ưu hóa chi phí

**Công cụ tính toán chi phí** 

[AWS Pricing Calculator](https://calculator.aws/#/)

    Cho phép tạo các estimate các dịch vụ thông dụng 

    Có thể chia sẻ các estimate cho người khác 

    Chi phí sẽ khác biệt theo từng Region

**AWS Support**

- Basic ( Explore )
- Developer ( Test / dev )
- Business ( Production )
- Enterprise ( Large Enterprise )

**Lab 000007 - Create Budget**

**Cost Budget** cho phép bạn gửi cảnh báo khi tổng chi phí vượt qua ngưỡng chi phí trong ngân sách

**Usage Budget** cho phép bạn cảnh báo khi tổng mức sử dụng theo từng dịch vụ bạn lựa chọn vượt qua ngưỡng mức sử dụng trong ngân sách. VD: mức sử dụng theo số giờ chạy của EC2

**Reservation Instance** (RI) budget cho phép bạn gửi cảnh báo dựa trên mức sử dụng các dịch vụ trả trước ( reserve instance) của bạn.

**Saving plans budget** cho phép bạn gửi cảnh báo dựa trên mức sử dụng các dịch vụ đã được qui định trong saving plans

![19-6](/images/19-6-2024/5-19-6.png)   