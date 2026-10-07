**Bài 2 : Phân tích và xử lý lỗi thực thi trong Terminal** 

## 

**Phần 1:** Lỗi xảy ra vì sinh viên đang đứng tại `Desktop` trong khi file `deploy.ps1` nằm trong `Downloads\Project`

\-. Bước 1 dùng `Get-Location` để xác định thư mục hiện tại.

\- Bước 2 dùng `Get-ChildItem` để kiểm tra các file trong thư mục.

\- Bước 3 xác định file nằm trong `Downloads\Project` và dùng `.\deploy.ps1` để chỉ rõ script cần thực thi từ thư mục hiện tại. PowerShell yêu cầu tiền tố `.\` khi gọi script ở thư mục hiện tại nhằm tránh việc vô tình thực thi một script cùng tên từ nơi khác.

**Phần 2: sửa lại** 

 Get-Location  
 cd ..\\Downloads\\Project  
 Test-Path .\\deploy.ps1  
 .\\deploy.ps1

