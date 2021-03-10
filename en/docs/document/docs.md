#Tài liệu hướng dẫn

###1. Cấu trúc của WSO2-Document

####a. Giới thiệu cấu trúc


####b. Cách thêm Routing vào Navigation

Để thêm 1 Routing vào Navigation chúng ta chọn file **en/mkdocs.yml**
[![name]({{base_path}}/assets/img/tailieu/img.png)]({{base_path}}/assets/img/tailieu/img.png)

Sau đó thêm Routing vào mục **nav**
Các mục cha con được biểu diễn dưới dạng dấu "-", ở mỗi cấp bậc dấu "-" sẽ biểu diễn lùi vào so với cấp trên.

[![img.png]({{base_path}}/assets/img/tailieu/img_1.png)]({{base_path}}/assets/img/tailieu/img_1.png)

Kết quả đạt được: 
[![img_2.png]({{base_path}}/assets/img/tailieu/img_2.png)]({{base_path}}/assets/img/tailieu/img_2.png)

###2. Cấu trúc file Markdown

####a. Links

-   Link đến 1 trang bên ngoài.
    - Cú pháp: 
         - Sử dụng thẻ [a]() trong HTML. Vd: [<a href="http://java.sun.com/javase/downloads/index.jsp">Oracle Java SE Development Kit (JDK)</a>]() 
         - Sử dụng link trong Markdown. Cú pháp: [Name](Url) Ví dụ: **[https://localhost:9443/publisher](https://localhost:9443/publisher)**
    
-   Link đến 1 trang khách trong thư mục.
    - Cú pháp: [Name](URL) Ví dụ: **[Tài liệu](#tab)**
    
    
#### Note

-   Chú thích Note có 2 kiểu biểu diễn:
    - Sử dụng HTML để biểu diễn. Cú pháp:
    ```
        <html><div class= “admonition note”>
        <p class= “admonition-title”>Note</p>
        </html>
    ```
      
    - Sử dụng Markdown để biểu diễn. Cú pháp:
    ```
    !!! note
     Content
    ```
    
-   Kết quả:
    
      [![name]({{base_path}}/assets/img/tailieu/img_4.png)]({{base_path}}/assets/img/tailieu/img_4.png)

#### Image

- Để thêm 1 hình ảnh vào tài liệu chúng ta thêm hình ảnh vào **/en/docs/assets/img**

- Sau thêm vào tài liệu bằng cú pháp: [![name](Url)](URL) Ví dụ: 
  
  [![name]({{base_path}}/assets/img/tailieu/img_6.png)]({{base_path}}/assets/img/tailieu/img_6.png)

####d. Bôi đen

- Bôi đen text bằng cú pháp **Text**

####e. Code exemple

- Để biểu diễn code exemple trong Markdown chúng ta sử dụng cú pháp: 
    `
         ```Ngôn ngữ
         Code example
    `
  
  Ví dụ:
 
     [![name]({{base_path}}/assets/img/tailieu/img_5.png)]({{base_path}}/assets/img/tailieu/img_5.png)

#### Tab

- Để viết các tab trong Markdown chúng ta sử dụng:
  
    ```
        ```bash tab= ‘Format’
				Content
        ```
         ```bash tab= ‘Example’
				Content
         ```
    ```

- Kết quả: 

  [![name]({{base_path}}/assets/img/tailieu/img_6.png)]({{base_path}}/assets/img/tailieu/img_6.png)

####g. Table

- Để viết Table trong Markdown chúng ta có thể sử dụng 2 cách:
    - Sử dụng table trong HTML
    ```
            <table>
            <tbody>
                <th>Id</th>
                <th>Name</th>
                <tr>
                    <td>1</td>
                    <td>Sơn</td>
                </tr>
                <tr>
                    <td>2</td>
                    <td>Ngọc</td>
                </tr>
            </tbody>
        </table>
    ```

    - Sử dụng table trong Markdown
    
      
        |Id           |Name                        |
        |-----------|------------------------------|
        |1          |Tạ Anh Sơn                    |
        |2          |Nguyễn Tuấn Ngọc              |

    
####h. API

- Đầu tiên chúng ta cần có 1 file API .yaml
  
- Sau đó chúng ta thêm vào en/docs.

- Vì Markdown chỉ hỗ trợ đọc file .md nên chúng ta cần có 1 file .md để include file .yaml
  
  [![name]({{base_path}}/assets/img/tailieu/img_12.png)]({{base_path}}/assets/img/tailieu/img_12.png)

- Include file .yaml bằng cách:
  
  [![name]({{base_path}}/assets/img/tailieu/img_13.png)]({{base_path}}/assets/img/tailieu/img_13.png)

- Ở đây chúng ta thấy phần teamplate/redoc.html được kế thừa, teamplate/redoc.html hỗ trợ cho API, hỗ trợ download file .yaml và hiển thị name và version của API

  [![name]({{base_path}}/assets/img/tailieu/img_14.png)]({{base_path}}/assets/img/tailieu/img_14.png)