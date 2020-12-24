#### Tài liệu sử dụng cho IOTA - Virtual IO
` Có thể sử dụng sanbox tương tự VTIO với dữ liệu tương ứng là chuỗi`

##### Hiển thị ảnh và tiêu đề:
`Hiển thị ảnh trên từng tin nhắn:`

![](https://github.com/nghuyy/iota/blob/main/src/src11.png?raw=true|124)

```
    Đẩu ra: 
      {'src':'url ảnh','p': "độ padding", 'w': "chiều rộng" , 'h': "chiều cao" , 't': 'Tiêu đề', 'l' : "nội dung gọi lại iota hoặc website khác" } 
```
Mẫu: 
```
    io.send,{'src':'https://live.staticflickr.com/65535/50381112368_f0afc44dbc_o_d.jpg','p': 10, 'w': 124 , 'h': 164 , 't': 'Ảnh 1', 'l' : 'iota://anh1' }   
    io.send,{'src':'https://live.staticflickr.com/65535/50381112368_f0afc44dbc_o_d.jpg','p': 10, 'w': 124 , 'h': 164 , 't': 'Ảnh 2', 'l' : 'iota://anh2' }  
```
```text
    Ví dụ: 
    Nhiều ảnh: https://test-box.vsys.vn/dashb/botedit/5fe3fa2ac3d69007f54c878e
    1 ảnh: https://test-box.vsys.vn/dashb/botedit/5fe41188c3d69007f54c878f
```
`Hiển thị ảnh theo hàng ngang với thanh cuộn:`
![](https://github.com/nghuyy/iota/blob/main/src/src12.png?raw=true|124)
```
    Đẩu ra: 
      { 'iolist':[
             {'src':'url ảnh','p': "độ padding", 'w': "chiều rộng" , 'h': "chiều cao" , 't': 'Tiêu đề', 'l' : "nội dung gọi lại iota hoặc website khác"},
            {'src':'url ảnh','p': "độ padding", 'w': "chiều rộng" , 'h': "chiều cao" , 't': 'Tiêu đề', 'l' : "nội dung gọi lại iota hoặc website khác"},
          ],
        'n':' Tiêu đề chính' 
      } 
```

Ví dụ:[IOTA TEST](https://test-box.vsys.vn/dashb/botedit/5fe44455c3d69007f54c8790)
