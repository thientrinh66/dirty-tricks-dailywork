# Tình huống:
- Công ty chặn truy cập các trang share host (Google Drive, OneDrive,...)
- Công ty giới hạn truy cập tất cả các trang có thể tải phần mềm
[...]

# Yêu cầu:
- Cần gửi 1 phần mềm portable (.exe) vào máy công ty để phục vụ công việc

# Tricks:
- Nén file exe thành các file zip dung lượng 20MB (Gmail cho phép đính kèm trực tiếp qua mail với file từ 20MB trở xuống)
- Các file zip từ 002 trở về sau sẽ gửi được bình thường qua gmail. File 001 không gửi được do vi phạm chính sách bảo mật của google.
- Cần làm: sử dụng cmd để encode file 001 này về dạng txt, sau đó sẽ gửi được qua gmail. Sau khi đã nhận được các file, tiến hành decode và unzip các file
   + Sender: trong cmd: certutil -encode file-cần-gửi.001 file-cần-gửi.001.txt
   + Reciever: trong cmd: certutil -encode file-cần-gửi.001.txt file-cần-gửi.001