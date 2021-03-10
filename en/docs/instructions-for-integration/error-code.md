# Error Code

## Engine Errors     

| STT | Error Number | Constant name                        | Error description                    |
| --- | ------------ | ------------------------------------ | ------------------------------------ |
| 1   | 1            | ENGINE\_ERR\_CONNECT\_TIME\_OUT      | Engine connection timout             |
| 2   | 2            | ENGINE\_ERR\_INTERNAL\_SERVER\_ERROR | Lỗi hệ thống Engine                  |
| 3   | 3            | ENGINE\_ERR\_VALIDATE                | Lỗi validate dữ liệu Engine          |
| 4   | 4            | ENGINE\_ERR\_UNKNOWN                 | Lỗi Engine không xác định            |
| 5   | 5            | ENGINE\_ERR\_NOT\_SUPPORT            | Lỗi engine không hỗ trợ              |
| 6   | 6            | ENGINE\_ERR\_UNAUTHORIZE             | Lỗi Engine xác thực không thành công |
| 7   | 7            | ENGINE\_ERR\_VALID\_FILE             | Lỗi Engine khi thao tác với File     |

## Platform Errors

| STT | Error Number | Constant name                          | Error description                  |
| --- | ------------ | -------------------------------------- | ---------------------------------- |
| 1   | 21           | PLATFORM\_ERR\_CONNECT\_TIME\_OUT      | Lỗi kết nối hệ thống BIOID         |
| 2   | 22           | PLATFORM\_ERR\_INTERNAL\_SERVER\_ERROR | Lỗi hệ thống BIOID                 |
| 3   | 23           | PLATFORM\_ERR\_AUTHENTICATION          | Xác thực không thành công          |
| 4   | 24           | PLATFORM\_ERR\_UNKNOWN                 | Lỗi hệ thống không xác định        |
| 5   | 25           | PLATFORM\_ERR\_AUTHORIZATION           | Không được phép truy cập           |
| 6   | 26           | PLATFORM\_ERR\_QUOTA\_EXCEEDED         | Vượt ngưỡng dịch vụ                |
| 7   | 27           | PLATFORM\_ERR\_PERSON\_SERVER\_ERROR   | Lỗi dịch vụ định danh              |
| 8   | 28           | PLATFORM\_ERR\_FILE\_SERVER\_ERROR     | Lỗi dịch vụ file                   |
| 9   | 29           | PLATFORM\_ERR\_FACE\_SERVER\_ERROR     | Lỗi dịch vụ face                   |
| 10  | 30           | PLATFORM\_ERR\_OCR\_SERVER\_ERROR      | Lỗi dịch vụ OCR                    |
| 11  | 31           | PLATFORM\_DUPLICATE\_FACE              | Trùng lặp khuôn mặt                |
| 12  | 32           | PLATFORM\_DUPLICATE\_DEMOGRAPHIC       | Trùng lặp demographic              |
| 13  | 33           | PLATFORM\_ERR\_FILE\_UPLOAD            | Lỗi upload file lên minio          |
| 14  | 34           | PLATFORM\_ERR\_MISSING\_BODY           | Thiếu thông tin body request       |
| 15  | 35           | PLATFORM\_ERR\_EXECUTION               | Không có quyền thực hiện chức năng |
| 16  | 36           | PLATFORM\_ERR\_EXECUTION\_FILE         | Lỗi thao tác với file              |
| 17  | 37           | PLATFORM\_ERR\_INVALID\_PARAMETER      | Lỗi tham số không đúng định dạng   |

## CLIENT ERROR       

| STT | Error Number | Constant name                                           | Error description                                                                                 |
| --- | ------------ | ------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| 1   | 41           | CLIENT\_ERR\_PERSON\_IDENTIFY\_EXISTED                  | Mã định danh đã tồn tại                                                                           |
| 2   | 42           | CLIENT\_ERR\_PERSON\_PHONE\_EXISTED                     | Số điện thoại đã tồn tại                                                                          |
| 3   | 43           | CLIENT\_ERR\_PERSON\_EMAIL\_EXISTED                     | Tài khoản Email đã tồn tại                                                                        |
| 4   | 44           | CLIENT\_ERR\_PERSON\_IDENTIFY\_NOT\_FOUND               | Không tìm thấy mã định danh                                                                       |
| 5   | 45           | CLIENT\_ERR\_PERSON\_ID\_NOT\_FOUND                     | Không tìm thấy định danh                                                                          |
| 6   | 46           | CLIENT\_ERR\_PERSON\_IDENTIFY\_MISSING                  | Mã định danh không được để trống                                                                  |
| 7   | 47           | CLIENT\_ERR\_PERSON\_IDENTIFY\_INVALID                  | Mã định danh không đúng                                                                           |
| 8   | 48           | CLIENT\_ERR\_PERSON\_PHONE\_INVALID                     | Số điện thoại không đúng                                                                          |
| 9   | 49           | CLIENT\_ERR\_PERSON\_EMAIL\_INVALID                     | Email không đúng                                                                                  |
| 10  | 50           | CLIENT\_ERR\_PERSON\_ID\_CARD\_NUMBER\_EXISTED          | Số thẻ đã tồn tại                                                                                 |
| 11  | 51           | CLIENT\_ERR\_PERSON\_ID\_CARD\_NUMBER\_NOT\_FOUND       | Không tìm thấy số CMT/HC/BLX                                                                      |
| 12  | 52           | CLIENT\_ERR\_PERSON\_NAME\_MISSING                      | Tên không được để trống                                                                           |
| 13  | 53           | CLIENT\_ERR\_PERSON\_NAME\_NOT\_FOUND                   | Không tìm thấy tên định danh                                                                      |
| 14  | 54           | CLIENT\_ERR\_PERSON\_NAME\_INVALID                      | Tên không được chưa kí tự đặc biệt và nhỏ hơn 255 kí tự                                           |
| 15  | 55           | CLIENT\_ERR\_PERSON\_IAL\_INVALID                       | Cấp độ xác thực nằm trong khoảng 1-3                                                              |
| 16  | 56           | CLIENT\_ERR\_PERSON\_ADDRESS\_INVALID                   | Địa chỉ được chưa kí tự đặc biệt và nhỏ hơn 1000 kí tự                                            |
| 17  | 57           | CLIENT\_ERR\_PERSON\_DATE\_OF\_BIRTH\_INVALID           | Ngày sinh không hợp lệ                                                                            |
| 18  | 58           | CLIENT\_ERR\_PERSON\_PLACE\_OF\_BIRTH\_INVALID          | Địa chỉ khai sinh không được chưa kí tự đặc biệt và nhỏ hơn 1000 kí tự                            |
| 19  | 59           | CLIENT\_ERR\_PERSON\_GENDER\_INVALID                    | Giới tính không hợp lệ                                                                            |
| 20  | 60           | CLIENT\_ERR\_PERSON\_PERMANENT\_ADD\_INVALID            | Địa chỉ thường trú không được chưa kí tự đặc biệt và nhỏ hơn 1000 kí tự                           |
| 21  | 61           | CLIENT\_ERR\_PERSON\_BLOOD\_GROUP\_INVALID              | Nhóm máu không hợp lệ                                                                             |
| 22  | 62           | CLIENT\_ERR\_PERSON\_RELIGION\_INVALID                  | Tôn giáo không hợp lệ                                                                             |
| 23  | 63           | CLIENT\_ERR\_PERSON\_MARITAL\_STATUS\_INVALID           | Tình trạng hôn nhân không hợp lệ                                                                  |
| 24  | 64           | CLIENT\_ERR\_PERSON\_NATIONALITY\_INVALID               | Quốc tịch không hợp lệ                                                                            |
| 25  | 65           | CLIENT\_ERR\_PERSON\_ETHNIC\_GROUP\_INVALID             | Nhóm dân tộc không hợp lệ                                                                         |
| 26  | 66           | CLIENT\_ERR\_PERSON\_HOME\_TOWN\_INVALID                | Quê quán không hợp lệ                                                                             |
| 27  | 67           | CLIENT\_ERR\_PERSON\_ID\_MISSING                        | Mã ID không được để trống                                                                         |
| 28  | 68           | CLIENT\_ERR\_PERSON\_GROUP\_NAME\_EXISTED               | Tên nhóm định danh đã tồn tại                                                                     |
| 29  | 69           | CLIENT\_ERR\_PERSON\_GROUP\_ID\_NOT\_FOUND              | Không tìm thấy nhóm định danh                                                                     |
| 30  | 70           | CLIENT\_ERR\_PERSON\_GROUP\_CAN\_NOT\_DELETE            | Không được xóa nhóm định danh có thành viên                                                       |
| 31  | 71           | CLIENT\_ERR\_PERSON\_GROUP\_EMPTY                       | Danh sách thành viên trống                                                                        |
| 32  | 72           | CLIENT\_ERR\_PERSON\_GROUP\_NAME\_INVALID               | Tên nhóm không được để trống, hoặc dài hơn 200 kí tự                                              |
| 33  | 73           | CLIENT\_ERR\_PERSON\_GROUP\_DESC\_INVALID               | Mô tả nhóm không được dài hơn 200 kí tự                                                           |
| 34  | 74           | CLIENT\_ERR\_PERSON\_DEMOGRAPHIC\_PENDING\_ID\_EXISTED  | Demogarphic Pending ID is existed                                                                 |
| 35  | 75           | CLIENT\_ERR\_PERSON\_DUPLICATE\_ID\_REG\_INVALID        | IdRegistration is invalid                                                                         |
| 36  | 76           | CLIENT\_ERR\_PERSON\_DUPLICATE\_ID\_DUPLICATED\_INVALID | IdDuplicated is invalid                                                                           |
| 37  | 77           | CLIENT\_ERR\_PERSON\_DUPLICATE\_TYPE\_INVALID           | Duplicate type is invalid                                                                         |
| 38  | 78           | CLIENT\_ERR\_PERSON\_DUPLICATE\_ID\_NOT\_FOUND          | Duplicate ID not found                                                                            |
| 39  | 79           | CLIENT\_ERR\_PERSON\_DEMOGRAPHIC\_ID\_NOT\_FOUND        | Không tim thấy thông tin nhân khẩu học                                                            |
| 40  | 80           | CLIENT\_ERR\_PERSON\_STATUS\_INVALID                    | Thông tin trạng thái không hợp lệ(ACTIVE-INACTIVE-LOCK)                                           |
| 41  | 81           | CLIENT\_ERR\_PERSON\_TEMPLATE\_ID\_REQUIRED             | Template Id không thể bỏ trống                                                                    |
| 42  | 82           | CLIENT\_ERR\_PERSON\_PROFILE\_TOO\_LONG                 | Thông tin profiles cần ngắn hơn 10.000 ký tự                                                      |
| 43  | 83           | CLIENT\_ERR\_PERSON\_PROFILE\_NAME\_REQUIRED            | Tên của profile không thể bỏ trống                                                                |
| 44  | 84           | CLIENT\_ERR\_PERSON\_ATTRIBUTE\_CODE\_INVALID           | Attribute Code không đúng định dạng \[a-z, A-Z, 0-9, \_\]{1-255}                                  |
| 45  | 85           | CLIENT\_ERR\_PERSON\_TEMPLATE\_NAME\_INVALID            | Template Name không đúng định dạng \[a-z, A-Z, 0-9, \_\]{1-255}                                   |
| 46  | 86           | CLIENT\_ERR\_PERSON\_TEMPLATE\_DESC\_INVALID            | Mô tả template không đúng định dạng \[a-z, A-Z, 0-9, \_\]{1-255}                                  |
| 47  | 87           | CLIENT\_ERR\_PERSON\_ATTRIBUTE\_NAME\_INVALID           | Tên thuộc tính(attribute) không đúng định dạng \[a-z, A-Z, 0-9, \_\]{1-255}                       |
| 48  | 88           | CLIENT\_ERR\_PERSON\_ATTRIBUTE\_TYPE\_INVALID           | Loại thuộc tính(attribute type) bị bỏ trống hoặc không đúng định dạng \[a-z, A-Z, 0-9, \_\]{1-45} |
| 49  | 89           | CLIENT\_ERR\_PERSON\_ATTRIBUTE\_SELECT\_INVALID         | Loại select cần ít nhất 01 phần tử dữ liệu                                                        |
| 50  | 90           | CLIENT\_ERR\_PERSON\_DOCUMENT\_ID\_INVALID              | Mã ID giấy tờ không đúng hoặc không được để trống                                                 |
| 51  | 91           | CLIENT\_ERR\_PERSON\_DOCUMENT\_ID\_NOT\_FOUND           | Không tiìm thấy thông tin giấy tờ                                                                 |
| 52  | 92           | CLIENT\_ERR\_PERSON\_TEMPLATE\_ID\_NOT\_FOUND           | Không tiìm thấy thông tin template                                                                |
| 53  | 93           | CLIENT\_ERR\_PERSON\_TEMPLATE\_NAME\_EXISTED            | Tên Template đã tồn tại                                                                           |

## FileService Errors 

| STT | Error Number | Constant name                      | Error description                                                       |
| --- | ------------ | ---------------------------------- | ----------------------------------------------------------------------- |
| 1   | 101          | CLIENT\_ERR\_FILE\_MAX\_SIZE       | File không được lớn hơn 10mb                                            |
| 2   | 102          | CLIENT\_ERR\_FILE\_TYPE            | Định dạng file ảnh chỉ chấp nhận jpq, jpeg, png                         |
| 3   | 103          | CLIENT\_ERR\_READ\_FILE\_FROM\_URL | Lỗi không đọc được file từ url                                          |
| 4   | 104          | CLIENT\_ERR\_FILE\_REQUIRED        | File required                                                           |
| 5   | 105          | CLIENT\_ERR\_URL\_REQUIRED         | URL file required                                                       |
| 6   | 106          | CLIENT\_ERR\_FILE\_CONTENT         | File content không hợp lệ                                               |
| 7   | 107          | CLIENT\_ERR\_URL\_INVALID          | URL không đúng                                                          |
| 8   | 108          | CLIENT\_ERR\_SIGNATURE\_INVALID    | Nội dung bản tin không hợp lệ hoặc đã bị thay đổi                       |
| 9   | 109          | CLIENT\_ERR\_IMAGE\_SIZE\_INVALID  | Kích thước ảnh không hợp lệ. Vui lòng chọn kích thước 720p - 1080p - 2k |

## FaceService   

| STT | Error Number | Constant name                         | Error description                    |
| --- | ------------ | ------------------------------------- | ------------------------------------ |
| 1   | 111          | CLIENT\_ERR\_FACE\_PERSON\_NOT\_FOUND | Không tìm thấy person                |
| 3   | 113          | CLIENT\_ERR\_FACE\_PERSON\_REQUIRED   | Person id required                   |
| 4   | 114          | CLIENT\_ERR\_FACE\_PERSON\_NOT\_EXIST | Person không tồn tại                 |
| 5   | 115          | CLIENT\_ERR\_FACE\_ENROLLID\_REQUIRED | Enroll ID required                   |
| 6   | 116          | CLIENT\_ERR\_FACE\_ENROLL\_NOT\_EXIST | Enroll không tồn tại                 |
| 7   | 117          | CLIENT\_ERR\_FACE\_ENROLL\_DELETED    | Enroll đã được xóa khỏi hệ thống     |
| 8   | 118          | CLIENT\_ERR\_FACE\_PERSON\_BLACKLIST  | Người dùng hiện đang trong blacklist |
| 9   | 127          | CLIENT\_ERR\_FACE\_PERSON\_INACTIVE   | Người dùng chưa được xác minh        |

## OCRService         

| STT | Error Number | Constant name                     | Error description              |
| --- | ------------ | --------------------------------- | ------------------------------ |
| 1   | 150          | CLIENT\_ERR\_OCR\_TYPE\_INVALID   | Loại giấy tờ không hợp lệ      |
| 2   | 151          | CLIENT\_ERR\_OCR\_FRONT\_INVALID  | Mặt trước giấy tờ không hợp lệ |
| 3   | 152          | CLIENT\_ERR\_OCR\_BACK\_INVALID   | Mặt sau giấy tờ không hợp lệ   |
| 4   | 153          | CLIENT\_ERR\_OCR\_TYPE\_PARAMETER | Tham số type không hợp lệ      |

## License            

| STT | Error Number | Constant name                     | Error description                                    |
| --- | ------------ | --------------------------------- | ---------------------------------------------------- |
| 1   | 401          | LICENSE\_INVALID                  | Giấy phép không hợp lệ hoặc đã hết hạn               |
| 2   | 402          | LICENSE\_SUBSCRIPTION\_NOT\_FOUND | Dịch vụ không được đăng ký sử dụng                   |
| 3   | 403          | LICENSE\_QUOTAS\_EXCEEDED         | Quý khách đã sử dụng hết giới hạn tài nguyên dịch vụ |
| 4   | 404          | LICENSE\_NOT\_FOUND               | Không tìm thấy thông tin giấy phép                   |

