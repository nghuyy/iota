#### Tài liệu sử dụng cho IOTA - Sandbox - Virtual IO
`Version 1.0`

```
  + Mọi kí tự ' sẽ được chuyển thành \". Để gởi 1 cấu trúc JSON
    từ IO không hỗ trợ " có thể dùng ' để thay thế ví dụ:
     "{\"data\":1}" tương đương với "{'data':1}
  + Để báo lỗi hay cập nhật tài liệu, sử dụng tính năng của Github
```
* Xóa màn hình tin nhắn
```text
out=':cls'
```
* Ghép tham số và đầu vào (Dùng cho Virtual IO)
```text
  Khi quy định tham số đầu vào, dữ liệu gọi tiếp theo sẽ kết hợp với tham số. Ví dụ khi user gõ ok, sẽ nhận lại id_ok
out=':fx,id'
```
* Gởi 1 liên kết đến người dùng, khi gởi 1 tin nhắn kèm link (http,https) link đó sẽ tự được phát hiện và user có thể click vào đó để mở, ví dụ:
```
out='Google https://google.com.vn'
```
