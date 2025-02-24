# KiemThuPhanMem
1. [Hướng dẫn test case JUnit5](#hướng-dẫn-test-case-junit5)
   - [thêm dependency](#thêm-dependency)


## Hướng dẫn test case junit5
## thêm dependency
vào file: Project file > pom.xml
```
<dependencies>
        <dependency>
            <groupId>org.junit.jupiter</groupId>
            <artifactId>junit-jupiter-engine</artifactId>
            <version>5.7.0-M1</version>
            <scope>test</scope>
        </dependency>
        <dependency>
            <groupId>org.junit.jupiter</groupId>
            <artifactId>junit-jupiter-params</artifactId>
            <version>5.7.0-M1</version>
            <scope>test</scope>
        </dependency>
        <dependency>
            <groupId>org.junit.platform</groupId>
            <artifactId>junit-platform-runner</artifactId>
            <version>1.7.0-M1</version>
            <scope>test</scope>
            <type>jar</type>
        </dependency>
    </dependencies>
```
và thêm
```
<build>
        <plugins>
            <plugin>
                <artifactId>
                    maven-surefire-plugin
                </artifactId>
                <version>2.22.2</version>
            </plugin>
        </plugins>
    </build>
```
Qua tab: File  
tạo cây thư mục sau nếu chưa có:   
- file > src > Test > Java  
- lúc này, bên project sẽ tự xuất hiện test packages  
=> đây là nơi dành riêng cho các dự án viết unit test  
- trong test packages > <default package>: tạo class java để test  
(trên đầu mỗi hàm test có thêm thông số: @Test)  

- tạo file muốn kiểm tra trong Sources pakeges > com.company.filenme > <tên file kiểm tra>


