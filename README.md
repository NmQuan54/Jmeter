# Jmeter

## Mục tiêu:
Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập trang web https://www.simplilearn.com/
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của trang web.
## Kịch bản kiểm tra:
- Thread Group:
- Số lượng thread: 100
- Thời gian chạy: 60 giây
- Ramp-up period: 10 giây
* HTTP Request: URL: https://www.simplilearn.com/
- Method: GET
- Content encoding: UTF-8
* Listeners:
- View Results Tree
- Aggregate Report
Kết quả kiểm tra:
# 1. Simpli
- Average: 54 ms - Thời gian phản hồi trung bình là 54 mili giây.
- Median: 10 ms - Thời gian phản hồi trung vị là 10 mili giây.
- 90% Line: 839 ms - 90% các yêu cầu hoàn thành trong vòng 839 mili giây.
- Min: 114.9 ms - Thời gian phản hồi ngắn nhất là 114.9 mili giây.
- Max: 0.0 ms - Đây có thể là một lỗi hoặc vấn đề trong việc thu thập dữ liệu.
- Error %: 23.81% - Tỷ lệ lỗi là 23.81%, khá cao và cần được xem xét kỹ lưỡng.
- Throughput: 8860.25 requests/sec - Số lượng yêu cầu được xử lý mỗi giây.
- Received KB/sec: 5.77 KB/sec - Lượng dữ liệu nhận được mỗi giây.
- Sent KB/sec: 381061.46 KB/sec - Lượng dữ liệu gửi đi mỗi giây, giá trị này có vẻ không hợp lý và có thể cần kiểm tra lại.
# 2. Resources
- Average: 38 ms - Thời gian phản hồi trung bình là 38 mili giây.
- Median: 11 ms - Thời gian phản hồi trung vị là 11 mili giây.
- 90% Line: 718 ms - 90% các yêu cầu hoàn thành trong vòng 718 mili giây.
- Min: 76.88 ms - Thời gian phản hồi ngắn nhất là 76.88 mili giây.
- Max: 0.0 ms - Đây có thể là một lỗi hoặc vấn đề trong việc thu thập dữ liệu.
- Error %: 24.35% - Tỷ lệ lỗi là 24.35%, cũng khá cao.
- Throughput: 5557.92 requests/sec - Số lượng yêu cầu được xử lý mỗi giây.
- Received KB/sec: 9.53 KB/sec - Lượng dữ liệu nhận được mỗi giây.
- Sent KB/sec: 233742.0 KB/sec - Lượng dữ liệu gửi đi mỗi giây, giá trị này có vẻ không hợp lý và có thể cần kiểm tra lại.
# 3. Business
- Average: 157 ms - Thời gian phản hồi trung bình là 157 mili giây.
- Median: 29 ms - Thời gian phản hồi trung vị là 29 mili giây.
- 90% Line: 1563 ms - 90% các yêu cầu hoàn thành trong vòng 1563 mili giây.
- Min: 239.88 ms - Thời gian phản hồi ngắn nhất là 239.88 mili giây.
 -Max: 0.0 ms - Đây có thể là một lỗi hoặc vấn đề trong việc thu thập dữ liệu.
 -Error %: 23.23% - Tỷ lệ lỗi là 23.23%.
 -Throughput: 35613.86 requests/sec - Số lượng yêu cầu được xử lý mỗi giây.
- Received KB/sec: 9.03 KB/sec - Lượng dữ liệu nhận được mỗi giây.
- Sent KB/sec: 1569973.05 KB/sec - Lượng dữ liệu gửi đi mỗi giây, giá trị này có vẻ không hợp lý và có thể cần kiểm tra lại.
# 4. TOTAL
- Average: 83 ms - Thời gian phản hồi trung bình là 83 mili giây.
-  Median: 10 ms - Thời gian phản hồi trung vị là 10 mili giây.
- 90% Line: 1563 ms - 90% các yêu cầu hoàn thành trong vòng 1563 mili giây.
- Min: 168.30 ms - Thời gian phản hồi ngắn nhất là 168.30 mili giây.
- Max: 0.0 ms - Đây có thể là một lỗi hoặc vấn đề trong việc thu thập dữ liệu.
- Error %: 66.93% - Tỷ lệ lỗi là 66.93%, rất cao và cần được kiểm tra ngay.
- Throughput: 47603.10 requests/sec - Số lượng yêu cầu được xử lý mỗi giây.
-  Received KB/sec: 22.81 KB/sec - Lượng dữ liệu nhận được mỗi giây.
- Sent KB/sec: 728258.84 KB/sec - Lượng dữ liệu gửi đi mỗi giây, giá trị này có vẻ không hợp lý và có thể cần kiểm tra lại.
# Kết Luận:
- Tỷ lệ lỗi cao: Tỷ lệ lỗi trong các nhóm và tổng thể đều cao, đặc biệt là giá trị tổng thể lên tới 66.93%. Điều này cho thấy có nhiều yêu cầu không thành công, có thể do lỗi máy chủ hoặc vấn đề mạng.
- Thời gian phản hồi: Thời gian phản hồi trung bình và 90% line khá tốt, nhưng vẫn cần giảm tỷ lệ lỗi.
- Throughput cao: Throughput cao, nhưng cần kiểm tra lại giá trị dữ liệu gửi đi, vì có vẻ không hợp lý.
- Cần điều tra: Cần kiểm tra lại giá trị Max và dữ liệu gửi đi để đảm bảo không có lỗi trong việc thu thập dữ liệu hoặc cấu hình JMeter.

image
![Screenshot 2024-05-30 113403](https://github.com/NmQuan54/Jmeter/assets/96828932/462f7c1b-8874-4e20-85a3-dc7b1be048a3)


Hình ảnh tổng quát
![Screenshot 2024-05-30 112259](https://github.com/NmQuan54/Jmeter/assets/96828932/a581699d-dfa7-4fd2-8f41-485dff7020a8)

# Kiểm tra hiệu năng API
## Mục tiêu:
- Sử dụng jMeter để tạo một kịch bản kiểm tra mô phỏng người dùng truy cập API thời tiết https://openweathermap.org/current.
- Chạy kịch bản kiểm tra và ghi lại kết quả.
- Phân tích kết quả kiểm tra, bao gồm thời gian phản hồi, số lượng yêu cầu thành công, số lượng yêu cầu thất bại, v.v.
- Dựa trên kết quả phân tích, đưa ra kết luận về hiệu năng của API.
* Kịch bản kiểm tra:
- Thread Group:
- Số lượng thread: 100
- Thời gian chạy: 60 giây
- Ramp-up period: 10 giây
- HTTP Request: URL: https://openweathermap.org/current
- Method: GET
- Content encoding: UTF-8
* Listeners:
- View Results Tree
- Aggregate Report
- Kết quả kiểm tra:
![Screenshot 2024-05-30 112356](https://github.com/NmQuan54/Jmeter/assets/96828932/e3516774-100a-4f63-b5ee-3bddd9d9f3c3)

Phân tích kết quả kiểm tra:
- Số lượng yêu cầu thành công: 996/1000 = 99,6%
- Số lượng yêu cầu thất bại: 4/1000 = 0,4%
- Thời gian phản hồi trung bình: 10
