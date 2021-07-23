[![](https://img.shields.io/badge/dynamic/json?style=flat-square&logo=docker&label=Online&query=%24.version&url=https%3A%2F%2F.iotabot.app%2Frelease.json)](https://iotabot.app)
![](https://img.shields.io/badge/dynamic/json?logo=libreoffice&style=flat-square&label=Note&query=%24.release_note&url=https%3A%2F%2Fiotabot.app%2Frelease.json)

Chú ý
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
* IOTA API:
```
Inbox:
Content-Type: application/json

POST: https://iotabot.app/api
{"cmd":"inbox", "token":"<token>", "d":"<d>", "to":"<to>"}
token: "xxxx"
d: nội dung tin nhắn
to: SĐT IOTA
```
