# Upload File

Chức năng này giúp Upload file lên hệ thống BioId. Tương ứng với Api [/upload]()

## Tên hàm

```
FileDetail publicExecuteUpload(file)
```

## Tham số đầu vào
|Name|Type|Description|Notes|
 |----|----|-----------|-----|
|file|File|1 File muốn upload lên server||

## Kiểu dữ liệu trả về

[File Detail]({{base_path}}/instructions-for-integration/documention-SDK/java/list-model/FileDetail)

## Code Example

```java
import com.vnpt.client.ApiClient;
import com.vnpt.client.ApiException;
import com.vnpt.client.api.FilesApi;
import com.vnpt.client.model.FileDetail;
import java.io.File;

/**
 * Tải file lên server
 *
 */
ApiClient client = new ApiClient(); // Khởi tạo ApiClinet
client.addDefaultHeader("Authorization", "Bearer " + "44759bd5-a734-35a1-ae34-64260cc24d5b"); // 44759bd5-a734-35a1-ae34-64260cc24d5b là Asset token
client.setBasePath("https://10.1.125.90:8243/s2/1.0"); // Địa chỉ endpoints
client.setConnectTimeout(200000);
client.setReadTimeout(200000);
client.setVerifyingSsl(false);

FilesApi filesApi = new FilesApi(client); // Khởi tạo FilesApi
File file = new File("D:\\logo.png");
try {
    FileDetail fileDetail = filesApi.publicExecuteUpload(file);
} catch (ApiException e) {
    e.printStackTrace();
}

```

!!! note
    - File không lớn hơn 10Mb
    - File-Type: image/jpg,image/png,image/pdf,image/jpeg.
    - Những mã lỗi thường gặp khi tích hợp [Error-code]({{base_path}}/instructions-for-integration/error-code/#fileservice-errors)
