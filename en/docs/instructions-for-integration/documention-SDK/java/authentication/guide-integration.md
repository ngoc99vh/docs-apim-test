# Tài liệu hướng dẫn tích hợp SDK
Trong quá trình tích hợp nếu có phát sinh vấn đề, xin vui lòng liên hệ quản trị

### I. Tổng quan
Tài liệu này nhằm mục đích mô tả chi tiết xây dựng ứng dụng tích hợp SDK cho VNPT BioID. Bộ SDK cung cấp những tính năng sau:

* [Đăng ký khuôn mặt thông qua ảnh]({{base_path}}/instructions-for-integration/documention-SDK/java/face-biometrics/docs/enrollments-faces/)
* Đăng ký khuôn mặt thông qua đường dẫn ảnh
* Xác minh khuôn mặt qua tệp ảnh
* Xác minh khuôn mặt qua đường dẫn ảnh
* Xác thực định danh khuôn mặt qua tệp ảnh
* Xác thực định danh khuôn mặt qua đường dẫn ảnh
* Lấy tất cả các khuôn mặt đã đăng ký của 01 người
* Lấy chi tiết thông tin đăng ký
* Xóa enroll theo enrollID
* Xóa tất cả face enroll của PersonID
* So sánh khuôn mặt qua file ảnh
* So sánh khuôn mặt qua đường dẫn ảnh
* Kiểm tra liveness

### II. Tích hợp thư viện SDK vào dự án
###1. Yêu cầu
* Java phiên bản JDK 1.7 trở lên
* Maven/Gradle
###2. Cài đặt
Để cài đặt thư viện ứng dụng API vào kho lưu trữ Maven cục bộ, bạn cần thực thi:
```shell
mvn clean install
```
###3. Bắt đầu sử dụng

```java

import io.swagger.client.*;
import io.swagger.client.auth.*;
import io.swagger.client.model.*;
import io.swagger.client.api.FacesApi;

import java.io.File;
import java.util.*;

public class FacesApiExample {

    public static void main(String[] args) {
        ApiClient defaultClient = Configuration.getDefaultApiClient();
        
        // Configure API key authorization: key
        ApiKeyAuth key = (ApiKeyAuth) defaultClient.getAuthentication("key");
        key.setApiKey("YOUR API KEY");
        // Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
        //key.setApiKeyPrefix("Token");

        FacesApi apiInstance = new FacesApi();
        File file = new File("/path/to/file.txt"); // File |  Thông tin đăng ký dữ liệu khuôn mặt
        Integer personId = 56; // Integer | ID của người được đăng ký
        try {
            EnrollResponse result = apiInstance.publicCreateEnrollmentsFaces(file, personId);
            System.out.println(result);
        } catch (ApiException e) {
            System.err.println("Exception when calling FacesApi#publicCreateEnrollmentsFaces");
            e.printStackTrace();
        }
    }
}

```

