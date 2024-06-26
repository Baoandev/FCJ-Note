---
title : "20-06-2024"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b>  </b> "
---

**AWS Well-Architected Framework**

Sáu trụ cột

- Operational Excellence Pillar (Trụ cột vận hành xuất sắc)
- Security Pillar (Trụ cột bảo mật)
- Reliability Pillar (Trụ cột độ tin cậy)
- Pillars of productivity efficiency (Trụ cột hiệu quả năng suất)
- Cost optimization pillar (Trụ cột tối ưu hóa chi phí)
- Sustainability Pillar (Trụ cột tính bền vững)
  
**Operational Excellence Pillar**

There are five design principles (5 nguyên tắc) for operational excellence in the cloud:

• Perform operations as code

- **Giải thích:** Thay vì thực hiện các tác vụ quản lý và vận hành hệ thống một cách thủ công, hãy tự động hóa chúng bằng cách sử dụng mã. Điều này bao gồm việc sử dụng các công cụ như AWS CloudFormation hoặc Terraform để triển khai và quản lý cơ sở hạ tầng, hay sử dụng các script để thực hiện các công việc định kỳ.
- **Lợi ích:** Tăng cường tính nhất quán, giảm thiểu lỗi do con người gây ra, và dễ dàng kiểm soát các thay đổi.

• Make frequent, small, reversible changes ( Thực hiện những thay đổi nhỏ và có thể đảo ngược nếu gặp sự cố )

- **Giải thích:** Thực hiện các thay đổi nhỏ và thường xuyên trong hệ thống thay vì thực hiện các thay đổi lớn và hiếm hoi. Mỗi thay đổi nhỏ cần phải dễ dàng đảo ngược nếu gặp phải sự cố.
- **Lợi ích:** Giảm thiểu rủi ro khi thay đổi hệ thống, dễ dàng phát hiện và khắc phục sự cố, và tăng khả năng phản ứng nhanh với các yêu cầu mới.

• Refine operations procedures frequently (Tinh chỉnh các quy trình hoạt động thường xuyên)

- **Giải thích:** Liên tục đánh giá và cải thiện các quy trình hoạt động để đảm bảo chúng luôn hiệu quả và phù hợp với nhu cầu hiện tại. Điều này bao gồm việc kiểm tra và cập nhật các quy trình vận hành, đào tạo nhân viên và áp dụng các phương pháp mới.
- **Lợi ích:** Tăng cường hiệu suất hoạt động, giảm thiểu rủi ro và lỗi, và đảm bảo hệ thống luôn sẵn sàng và hiệu quả.

• Anticipate failure ( Dự đoán sự cố )

- **Giải thích:** Luôn giả định rằng các sự cố sẽ xảy ra và chuẩn bị sẵn các kế hoạch để xử lý chúng. Điều này bao gồm việc xây dựng các cơ chế tự động phát hiện và khắc phục sự cố, cũng như thực hiện các bài kiểm tra dự phòng thường xuyên.
- **Lợi ích:** Tăng cường khả năng phục hồi của hệ thống, giảm thiểu thời gian gián đoạn và đảm bảo tính liên tục của dịch vụ.

• Learn from all operational failures ( Học hỏi từ tất cả các sự cố vận hành )

- **Giải thích:** Mỗi khi có sự cố xảy ra, hãy phân tích nguyên nhân gốc rễ và tìm ra các biện pháp khắc phục để ngăn ngừa sự cố tương tự trong tương lai. Điều này bao gồm việc thu thập dữ liệu, phân tích sự cố và chia sẻ kiến thức trong toàn bộ tổ chức.
- **Lợi ích:** Liên tục cải thiện hệ thống, nâng cao kiến thức và kỹ năng của nhân viên, và giảm thiểu các sự cố tương tự trong tương lai.


**Security Pillar**

There are seven design principles for security in the cloud ( 7 nguyên tắc )

• Implement a strong identity foundation (Xây dựng nền tảng nhận dạng mạnh mẽ)

- **Giải thích:** Sử dụng các phương pháp quản lý danh tính và quyền truy cập mạnh mẽ để kiểm soát ai có thể truy cập vào các tài nguyên và hành động gì họ có thể thực hiện. Điều này bao gồm việc sử dụng các nguyên tắc như quyền truy cập tối thiểu, xác thực đa yếu tố (MFA) và quản lý vai trò (IAM roles).
- **Lợi ích:** Đảm bảo rằng chỉ những người dùng và dịch vụ được ủy quyền mới có thể truy cập và thao tác trên các tài nguyên, giảm thiểu rủi ro từ các truy cập trái phép.

• Enable traceability (Kích hoạt khả năng theo dõi)

- **Giải thích:** Ghi lại và theo dõi tất cả các hoạt động trong hệ thống để có thể phân tích và điều tra khi cần. Sử dụng các dịch vụ như AWS CloudTrail, AWS Config, và Amazon CloudWatch để thu thập và phân tích dữ liệu nhật ký.
- **Lợi ích:** Cung cấp khả năng phát hiện và phản ứng nhanh chóng với các sự cố bảo mật, cũng như tuân thủ các yêu cầu pháp lý và quy định.

• Apply security at all layers (Áp dụng bảo mật ở tất cả các lớp)

- **Giải thích:** Bảo mật nên được tích hợp vào mọi lớp của hệ thống, bao gồm lớp mạng, hệ điều hành, ứng dụng và dữ liệu. Sử dụng các công cụ và dịch vụ bảo mật như tường lửa, mã hóa và kiểm tra lỗ hổng.
- **Lợi ích:** Tăng cường khả năng bảo vệ toàn diện, giảm thiểu các điểm yếu và tạo ra nhiều lớp phòng thủ chống lại các mối đe dọa.

• Automate security best practices (Tự động hóa các phương pháp bảo mật tốt nhất)

- **Giải thích:** Tự động hóa các tác vụ bảo mật thông qua việc sử dụng mã và các công cụ tự động. Ví dụ: sử dụng AWS Lambda để thực hiện các kiểm tra bảo mật tự động hoặc AWS Security Hub để tập trung và tự động hóa quản lý bảo mật.
- **Lợi ích:** Giảm thiểu lỗi do con người gây ra, tăng cường tính nhất quán và cho phép phản ứng nhanh chóng với các sự cố bảo mật.

• Protect data in transit and at rest (Bảo vệ dữ liệu khi truyền và khi lưu trữ)

- **Giải thích:** Sử dụng các phương pháp mã hóa để bảo vệ dữ liệu khi nó đang được truyền qua mạng và khi nó được lưu trữ. Sử dụng các dịch vụ như AWS Key Management Service (KMS) và SSL/TLS để mã hóa dữ liệu.
- **Lợi ích:** Đảm bảo tính bảo mật và toàn vẹn của dữ liệu, ngăn chặn các truy cập trái phép và bảo vệ dữ liệu khỏi các mối đe dọa.

• Keep people away from data (Giữ người dùng khỏi dữ liệu)

- **Giải thích:** Giảm thiểu việc người dùng trực tiếp truy cập vào dữ liệu và hệ thống bằng cách sử dụng các công cụ tự động và các cơ chế kiểm soát truy cập. Ví dụ: sử dụng các công cụ quản lý và tự động hóa thay vì cho phép truy cập trực tiếp vào cơ sở dữ liệu.
- **Lợi ích:** Giảm thiểu rủi ro do lỗi con người hoặc các hoạt động trái phép, và bảo vệ dữ liệu nhạy cảm.

• Prepare for security events (Chuẩn bị cho các sự cố bảo mật)

- **Giải thích:** Xây dựng và thực hiện các kế hoạch phản ứng sự cố bảo mật, bao gồm việc phát hiện, phản ứng, và khắc phục. Điều này bao gồm việc thử nghiệm và cập nhật các kế hoạch này thường xuyên.
- **Lợi ích:** Tăng cường khả năng phản ứng nhanh chóng và hiệu quả với các sự cố bảo mật, giảm thiểu tác động và thời gian gián đoạn.


**Reliability Pillar**

There are five design principles for reliability in the cloud:

• Automatically recover from failure (Tự động khôi phục từ sự cố)

- **Giải thích:** Hệ thống phải có khả năng tự động phát hiện và khắc phục các sự cố mà không cần sự can thiệp của con người. Sử dụng các dịch vụ và cơ chế tự động để thay thế hoặc khắc phục các thành phần bị hỏng.
- **Lợi ích:** Giảm thiểu thời gian gián đoạn dịch vụ, tăng cường tính sẵn sàng của hệ thống và đảm bảo dịch vụ liên tục cho người dùng.

• Test recovery procedures (Kiểm tra các quy trình khôi phục)

- **Giải thích:** Thường xuyên kiểm tra và đánh giá các quy trình khôi phục để đảm bảo chúng hoạt động hiệu quả khi cần. Điều này bao gồm việc thực hiện các bài kiểm tra dự phòng và kịch bản sự cố.
- **Lợi ích:** Xác định và khắc phục các điểm yếu trong quy trình khôi phục, đảm bảo hệ thống có thể phục hồi nhanh chóng từ các sự cố và tăng cường khả năng sẵn sàng.

• Scale horizontally to increase aggregate workload availability (Mở rộng ngang để tăng khả năng chịu tải tổng hợp)

- **Giải thích:** Thay vì tăng cường năng lực của một thành phần duy nhất (mở rộng dọc), hãy thêm nhiều thành phần tương tự (mở rộng ngang) để phân phối tải công việc. Sử dụng các cơ chế cân bằng tải và các cụm máy chủ để đảm bảo khả năng mở rộng.
- **Lợi ích:** Tăng khả năng chịu tải của hệ thống, giảm nguy cơ điểm đơn lẻ thất bại (single point of failure) và cải thiện hiệu suất.

• Stop guessing capacity (Ngừng đoán dung lượng)

- **Giải thích:** Sử dụng các công cụ và dịch vụ tự động để quản lý và dự đoán nhu cầu dung lượng thay vì dựa vào ước lượng thủ công. Sử dụng các dịch vụ như Auto Scaling để tự động điều chỉnh tài nguyên dựa trên nhu cầu thực tế.
- **Lợi ích:** Đảm bảo hệ thống luôn có đủ tài nguyên để đáp ứng nhu cầu mà không bị quá tải hoặc lãng phí tài nguyên, tăng hiệu quả sử dụng tài nguyên và giảm chi phí.

• Manage change in automation (Quản lý thay đổi bằng tự động hóa)

- **Giải thích:** Tự động hóa quy trình quản lý thay đổi để đảm bảo các thay đổi được triển khai nhất quán và an toàn. Sử dụng các công cụ như AWS CloudFormation hoặc AWS CodePipeline để tự động hóa việc triển khai và quản lý các thay đổi.
- **Lợi ích:** Giảm thiểu lỗi do con người gây ra, tăng tính nhất quán và tốc độ triển khai thay đổi, và đảm bảo rằng các thay đổi không làm ảnh hưởng tiêu cực đến tính sẵn sàng của hệ thống.

**Pillars of productivity efficiency**

There are five design principles 

• Democratize advanced technologies (Dân chủ hóa các công nghệ tiên tiến)

- **Giải thích:** Sử dụng các dịch vụ đám mây để dễ dàng truy cập và triển khai các công nghệ tiên tiến mà trước đây chỉ có các tổ chức lớn mới có thể tiếp cận. AWS cung cấp nhiều dịch vụ tiên tiến như machine learning, phân tích dữ liệu lớn, và Internet of Things (IoT).
- **Lợi ích:** Tăng cường khả năng sáng tạo và cạnh tranh, giảm chi phí và thời gian triển khai các giải pháp tiên tiến, và cho phép các tổ chức nhỏ và trung bình tiếp cận các công nghệ hàng đầu.

• Go global in minutes  (Triển khai toàn cầu trong vài phút)

- **Giải thích:** Sử dụng cơ sở hạ tầng đám mây để mở rộng hệ thống và dịch vụ ra toàn cầu một cách nhanh chóng. AWS cung cấp các khu vực và khu vực khả dụng (availability zones) trên toàn thế giới, cho phép bạn triển khai ứng dụng gần với người dùng cuối.
- **Lợi ích:** Cải thiện hiệu suất và độ trễ cho người dùng toàn cầu, dễ dàng đáp ứng các yêu cầu pháp lý và quy định địa phương, và tăng cường tính linh hoạt và khả năng phục hồi của hệ thống.

• Use serverless architectures (Sử dụng kiến trúc không máy chủ)

- **Giải thích:** Tận dụng các dịch vụ không máy chủ (serverless) như AWS Lambda để chạy mã mà không cần quản lý cơ sở hạ tầng máy chủ. Serverless cho phép bạn tập trung vào logic kinh doanh và tự động quản lý việc mở rộng và tối ưu hóa tài nguyên.
- **Lợi ích:** Giảm chi phí vận hành và quản lý cơ sở hạ tầng, tăng cường khả năng mở rộng và phản ứng nhanh với các thay đổi về nhu cầu, và đơn giản hóa việc triển khai và bảo trì ứng dụng.

• Experiment more often (Thử nghiệm thường xuyên hơn)

- **Giải thích:** Sử dụng môi trường đám mây để dễ dàng và nhanh chóng thử nghiệm các ý tưởng mới. AWS cung cấp các dịch vụ có thể được triển khai và điều chỉnh linh hoạt, cho phép bạn tạo và kiểm tra các giả thuyết một cách nhanh chóng.
- **Lợi ích:** Tăng cường khả năng đổi mới và cải tiến liên tục, giảm rủi ro và chi phí liên quan đến việc thử nghiệm, và cải thiện chất lượng sản phẩm và dịch vụ thông qua thử nghiệm và học hỏi.

• Consider mechanical sympathy (Cân nhắc về sự đồng cảm cơ học)

- **Giải thích:** Hiểu rõ cách thức hoạt động của các tài nguyên cơ bản và thiết kế hệ thống để tận dụng tối đa các đặc điểm của chúng. Ví dụ, tối ưu hóa việc sử dụng CPU, bộ nhớ, và băng thông để đạt hiệu suất tối đa.
- **Lợi ích:** Tăng hiệu suất và hiệu quả sử dụng tài nguyên, giảm thiểu lãng phí và chi phí, và đảm bảo rằng hệ thống hoạt động một cách tối ưu với các tài nguyên hiện có.




