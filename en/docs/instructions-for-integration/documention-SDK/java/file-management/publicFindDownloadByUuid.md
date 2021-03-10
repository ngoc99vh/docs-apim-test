# Download file từ server

Chức năng này giúp download file từ server. Tương ứng với Api [/download/{uuid}]()

## Tên hàm

```
publicFindDownloadByUuid(uuid)
```

## Tham số đầu vào

|Name|Type|Description|Notes|
 |----|----|-----------|-----|
|uuid|String|ID cùa file trên hệ thống||

## Kiểu dữ liệu trả về

File

## Code Example

```java
import com.vnpt.client.ApiClient;
import com.vnpt.client.ApiException;
import com.vnpt.client.api.FilesApi;
import com.vnpt.client.model.FileDetail;
import java.io.File;

/**
 * Download file từ server
 *
 */
ApiClient client = new ApiClient(); // Khởi tạo ApiClinet
client.addDefaultHeader("Authorization", "Bearer " + "44759bd5-a734-35a1-ae34-64260cc24d5b"); // 44759bd5-a734-35a1-ae34-64260cc24d5b là Asset token
client.setBasePath("https://10.1.125.90:8243/s2/1.0"); // Địa chỉ endpoints
client.setConnectTimeout(200000);
client.setReadTimeout(200000);
client.setVerifyingSsl(false);

FilesApi filesApi = new FilesApi(client); // Khởi tạo FilesApi
String uuid = "0b0bd6ec-8e31-4599-b34a-b72d6da06691"; // ID cùa file trên hệ thống
try {
    File file = filesApi.publicFindDownloadByUuid(uuid);

} catch (ApiException e) {
    e.printStackTrace();
}
```

!!! note
    - **uuid** là kết quả trả về khi upload file lên hệ thống [publicExecuteUpload]({{base_path}}/instructions-for-integration/documention-SDK/java/file-management/publicExecuteUpload)
    - Những mã lỗi thường gặp khi tích hợp [Error-code]({{base_path}}/instructions-for-integration/error-code/#fileservice-errors)