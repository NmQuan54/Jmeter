# Jmeter

## Mục tiêu:
Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://www.simplilearn.com/
Chạy kịch bản kiểm tra và ghi lại kết quả.
Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.
Kịch bản kiểm tra:
Thread Group:
Số lượng thread: 100
Thời gian chạy: 60 giây
Ramp-up period: 10 giây
HTTP Request:
URL: https://www.simplilearn.com/
Method: GET
Content encoding: UTF-8
Listeners:
View Results Tree
Aggregate Report
Kết quả kiểm tra:
image

![Screenshot 2024-05-30 112111](https://github.com/NmQuan54/Jmeter/assets/96828932/c0a52bc5-3b09-4075-9869-e4dbb3c73675)

Hình ảnh tổng quát
![Screenshot 2024-05-30 112259](https://github.com/NmQuan54/Jmeter/assets/96828932/a581699d-dfa7-4fd2-8f41-485dff7020a8)

Kiểm tra hiệu năng API
Mục tiêu:
Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập API thời tiết https://openweathermap.org/current.
Chạy kịch bản kiểm tra và ghi lại kết quả.
Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.
Kịch bản kiểm tra:
Thread Group:
Số lượng thread: 100
Thời gian chạy: 60 giây
Ramp-up period: 10 giây
HTTP Request:
URL: https://openweathermap.org/current
Method: GET
Content encoding: UTF-8
Listeners:
View Results Tree
Aggregate Report
Kết quả kiểm tra:
![Screenshot 2024-05-30 112356](https://github.com/NmQuan54/Jmeter/assets/96828932/e3516774-100a-4f63-b5ee-3bddd9d9f3c3)

Phân tích kết quả kiểm tra:
Số lượng yêu cầu thành công: 996/1000 = 99,6%
Số lượng yêu cầu thất bại: 4/1000 = 0,4%
Thời gian phản hồi trung bình: 10
