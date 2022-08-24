# Tình huống:
- Có cả trăm video nhỏ
- Bạn cần phải xem hết tất cả để biết nội dung,... nhưng việc mở hàng trăm video lần lượt là quá mất thời gian
- Bạn muốn merge vào cùng 1 video lớn để xem cho nhanh
- Nhưng các phần mềm video làm việc này hơi lâu


# Tricks:
- Sử dụng format factory
- Video merge
- Chọn trong output setting mục Video encode là copy --> Để video merge giữ nguyên encode, không cần phải re-encode --> Sẽ nhanh hơn.

# Edit 220824: 
- Sử dụng format factory có vẻ không thực sự hoạt động nếu số lượng file lớn. Đã thử với 100 file, 50 file, thậm chí ít hơn nhưng bị lỗi can not mux audio
--> Sử dụng LosslessCut: https://mifi.github.io/lossless-cut/