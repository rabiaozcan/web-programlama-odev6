# web-programlama-odev6
jsp-servlet-hibernate-crud-example


Ondokuz Mayıs Üniversitesi Bilgisayar Mühendisliği Bölümü Web Programlama Dersi Ödev 6


Ödevde Jsp, Hibernate ve Servlet kullanılmıştır. IDE- Eclipse 2021-3, JDK 11, MySQL v8 ve Apache Tomcat v10  tercih edilmiştir.

Proje Eclipse üzerinden "Dynamic Web Project" olarak oluşturulup, "Maven Project" dönüşümü yapılmıştır. Src>main>webapp>WEB-INF>lib klasörüne, projenin yapıldığı
dökümantasyondan farklı olarak:

taglibs-standard-impl-1.2.5.jar
servlet-api-2.5.jar
protobuf-java-3.6.1.jar
mysql-connector-java-8.0.13.jar
jboss-transaction-api_1.2_spec-1.1.1.Final.jar
jboss-logging-3.3.2.Final.jar
javax.servlet.jsp.jstl-api-1.2.1.jar
javax.servlet.jsp.jstl-1.2.1.jar
javax.persistence-api-2.2.jar
javax.activation-api-1.2.0.jar
javassist-3.23.1-GA.jar
jandex-2.0.5.Final.jar
hibernate-core-5.3.7.Final.jar
hibernate-commons-annotations-5.0.4.Final.jar
dom4j-2.1.1.jar
classmate-1.3.4.jar
byte-buddy-1.8.17.jar
antlr-2.7.7.jar jar'ları eklenmiştir. lib klasörüne eklenen bu jarlar Buil Path şeklinde projenin Web-App Libraries'ine eklenmiştir.

Ayrıca projede jdk 11 kullanıldığı için javax.xml.bind desteği bulunmamaktadır. Bu sebeple pom.xml dosyasına

<dependencies>
<dependency>
    <groupId>javax.xml.bind</groupId>
    <artifactId>jaxb-api</artifactId>
    <version>2.3.1</version>
</dependency>
</dependencies>  şeklinde javax.xml.bind bağımlılığı eklenmiştir.


MySQL üzerinde 

CREATE DATABASE demo; kodu ile demo adında veri tabanı oluşturulup,

USE demo; kodu ile veritabanına geçiş sağlanmıştır. demo isimli veritabanında

CREATE TABLE users(id int(13) NOT NULL AUTO_INCREMENT, name varchar(120) NOT NULL, email varchar(120)
NOT NULL, country varchar(120), PRIMARY KEY(id)); kodu ile users adlı tablo oluşturulup, 13 karakterden oluşup integer değer alan, otomatik artan ve primary key 
olan id, 120 karakterden oluşup string değer alan ve boş olmayacak şartlı name, 120 karakterden oluşup string değer alan, boş olmayacak şartlı email, ve 120 
karakterden oluşup string değer alan country tanımlanmıştır.




