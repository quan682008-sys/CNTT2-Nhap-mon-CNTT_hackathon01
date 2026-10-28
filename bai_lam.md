# BÀI LÀM – HACKATHON 01

- **Mã đề:** 18
- **Họ tên: Nguyen Minh Quan** 
- **Lớp:CNTT2** 
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):Windows** 

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
PS E:\> cd E:\noi-that-website\starter-kit\"Noi That Website FINAL"
PS E:\noi-that-website\starter-kit\Noi That Website FINAL> Get-ChildItem -force
PS E:\noi-that-website\starter-kit\Noi That Website FINAL> Move-Item .\kich_thuoc.txt .\docs\
PS E:\noi-that-website\starter-kit\Noi That Website FINAL> Move-Item .\Logo_Noi_That.PNG .\media\
PS E:\noi-that-website\starter-kit\Noi That Website FINAL> Copy-Item .\media .\backup -Recurse
PS E:\noi-that-website\starter-kit\Noi That Website FINAL> rm temp_267.tmp
PS E:\noi-that-website\starter-kit\Noi That Website FINAL> cd ..
PS E:\noi-that-website\starter-kit> cd ..
PS E:\noi-that-website> cd logs
PS E:\noi-that-website\logs> Get-Content *.log
PS E:\noi-that-website\logs> cd ..
```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
PS E:\noi-that-website> Get-ChildItem -Recurse -Force


    Directory: E:\noi-that-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/28/2026   1:44 PM                data
d-----        10/28/2026   1:41 PM                docs
d-----        10/28/2026   1:44 PM                logs
d-----        10/28/2026   1:41 PM                media
d-----        10/28/2026   1:47 PM                starter-kit
-a----        10/27/2026   1:32 AM           2226 bai_lam.md


    Directory: E:\noi-that-website\data


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/27/2026   1:32 AM           6121 don_noi_that_quy_1.xlsx


    Directory: E:\noi-that-website\logs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----        10/27/2026   1:32 AM           1028 Furniture.log


    Directory: E:\noi-that-website\starter-kit


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/28/2026   2:05 PM                Noi That Website FINAL
------        10/27/2026   1:32 AM           2226 bai_lam.md


    Directory: E:\noi-that-website\starter-kit\Noi That Website FINAL


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
------        10/27/2026   1:32 AM             68 .env
-a----        10/27/2026   1:32 AM           4403 backup
-a----        10/27/2026   1:32 AM             53 docs
-a----        10/27/2026   1:32 AM           4403 media

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
PS E:\noi-that-website\logs> Get-Content Furniture.log | Select-String "ERROR"
```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
2026-01-28 07:35:33 [ERROR] Dat coc bi tu choi
2026-01-28 07:47:33 [ERROR] Dat coc bi tu choi

```

## 4.4. Thao tác với tài liệu Markdown (README.md)

> README.md được chấm trực tiếp trên file `README.md` ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [x] Heading 1: tên dự án
- [x] Mô tả ngắn có cả **in đậm** và *in nghiêng*
- [x] Bảng `Thư mục | Nội dung`, ít nhất 3 dòng dữ liệu
- [ ] Code block chứa lệnh PowerShell/Terminal liệt kê nội dung dự án
-[x]task list ít nhất 2 công việc, có ít nhất 1 mục đã hoàn thành
- [ ] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# Ghi lệnh vào đây (xoá dòng này)

```

### Kết quả hiển thị

```text
(Dán kết quả vào đây – xoá dòng này)

```
  PS E:\noi-that-website> Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass                                     

PS E:\noi-that-website> .\auto_report.ps1                                                                              
                                   
## 4.6. Đếm số dòng lỗi

### Lệnh

```shell

PS E:\noi-that-website\logs> (Get-Content Furniture.log | Select-String "ERROR" | Measure-Object).Count
7
```

### Kết quả đếm (Windows: giá trị Count; macOS: con số in ra)

```text
7
```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng (xoá dòng này)

```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây – xoá dòng này)

```

## 4.8. Excel

> Phần Excel được chấm trực tiếp trên file `data/don_noi_that_quy_1.xlsx`, không cần ghi vào đây.
