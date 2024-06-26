---
title : "24-06-2024"
date :  "`r Sys.Date()`" 
weight : 1 
chapter : false
pre : " <b>  </b> "
---
# Sovico lab

## VPC Fundamentals

Tạo VPC

![Sovico](/images/24-6-2024/1-24-6.png)

Setting VPC, Click chọn Enable DNS hostnames

![Sovico](/images/24-6-2024/2-24-6.png)

Tạo subnets

![Sovico](/images/24-6-2024/3-24-6.png)

Chọn VPC A vừa tạo VPC ID

![Sovico](/images/24-6-2024/4-24-6.png)

Setting subnet như sau 

![Sovico](/images/24-6-2024/5-24-6.png)

Tạo xong sẽ có 1 subnets ở Subnets list

![Sovico](/images/24-6-2024/6-24-6.png)

Lần lượt tạo thêm 3 Subnets nữa (mỗi AZ có 1 Subnet public và 1 Subnet private )

![Sovico](/images/24-6-2024/7-24-6.png)

Select Network ACL

![Sovico](/images/24-6-2024/8-24-6.png)

Create Network ACL

![Sovico](/images/24-6-2024/9-24-6.png)

Chọn Subnet associations và click Edit

![Sovico](/images/24-6-2024/10-24-6.png)

Chọn 4 Subnets vừa tạo 

![Sovico](/images/24-6-2024/11-24-6.png)

Ngoài trang Network ACLs, select inbound rules và chọn edit

![Sovico](/images/24-6-2024/12-24-6.png)

Edit inbound rules

![Sovico](/images/24-6-2024/13-24-6.png)

Ngoài trang Network ACLs, select outbound rules và chọn edit

![Sovico](/images/24-6-2024/14-24-6.png)

Edit outbound rules

![Sovico](/images/24-6-2024/15-24-6.png)

Tạo route table

![Sovico](/images/24-6-2024/16-24-6.png)

Select Subnet Associations và chọn edit

![Sovico](/images/24-6-2024/17-24-6.png)

Chọn 2 subnet pulics

![Sovico](/images/24-6-2024/18-24-6.png)

![Sovico](/images/24-6-2024/19-24-6.png)

Tạo thêm 1 route table private

![Sovico](/images/24-6-2024/20-24-6.png)

Edit Subnet associations và chọn 2 subnet private

![Sovico](/images/24-6-2024/21-24-6.png)

![Sovico](/images/24-6-2024/22-24-6.png)

Tạo Internets gateways

![Sovico](/images/24-6-2024/23-24-6.png)

![Sovico](/images/24-6-2024/24-24-6.png)

Attach to vpc

![Sovico](/images/24-6-2024/25-24-6.png)

![Sovico](/images/24-6-2024/26-24-6.png)

Update route tables, select Routes chọn edit routes

![Sovico](/images/24-6-2024/27-24-6.png)

Edit Routes

![Sovico](/images/24-6-2024/28-24-6.png)

Create Nat gateways

![Sovico](/images/24-6-2024/29-24-6.png)

![Sovico](/images/24-6-2024/30-24-6.png)

Update Private Route tables, Vào Route tables, select private route table và chọn route, sau đó edit routes

![Sovico](/images/24-6-2024/31-24-6.png)

![Sovico](/images/24-6-2024/32-24-6.png)

Create endpoints

![Sovico](/images/24-6-2024/33-24-6.png)

![Sovico](/images/24-6-2024/34-24-6.png)

![Sovico](/images/24-6-2024/35-24-6.png)

![Sovico](/images/24-6-2024/36-24-6.png)

Create another endpoint

![Sovico](/images/24-6-2024/37-24-6.png)

![Sovico](/images/24-6-2024/38-24-6.png)

![Sovico](/images/24-6-2024/39-24-6.png)

Launch an EC2 instance

![Sovico](/images/24-6-2024/40-24-6.png)

![Sovico](/images/24-6-2024/41-24-6.png)

![Sovico](/images/24-6-2024/42-24-6.png)

![Sovico](/images/24-6-2024/43-24-6.png)

![Sovico](/images/24-6-2024/44-24-6.png)

Lauch another

![Sovico](/images/24-6-2024/45-24-6.png)

![Sovico](/images/24-6-2024/46-24-6.png)

Test connect

![Sovico](/images/24-6-2024/47-24-6.png)

![Sovico](/images/24-6-2024/48-24-6.png)

![Sovico](/images/24-6-2024/49-24-6.png)

![Sovico](/images/24-6-2024/50-24-6.png)

![Sovico](/images/24-6-2024/51-24-6.png)

## Multiples VPCS

VPC peering 

![Sovico](/images/24-6-2024/52-24-6.png)

Transit gateway

![Sovico](/images/24-6-2024/53-24-6.png)

![Sovico](/images/24-6-2024/54-24-6.png)

![Sovico](/images/24-6-2024/55-24-6.png)

## Security controls

Network acls

![Sovico](/images/24-6-2024/56-24-6.png)

![Sovico](/images/24-6-2024/57-24-6.png)

Endpoint policy

![Sovcio](/images/24-6-2024/endpointpolicy.png)

## Connecting to on-premises

Etablish vpn connection

![Sovcio](/images/24-6-2024/59-24-6.png)

![Sovico](/images/24-6-2024/60-24-6.png)

![Sovico](/images/24-6-2024/61-24-6.png)

![Sovico](/images/24-6-2024/62-24-6.png)