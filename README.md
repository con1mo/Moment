# Moment - 스프링, JPA를 사용하여 AWS에 배포해보는 프로젝트

- Java

- Spring Boot & Spring Security
- Build : Gradle

- H2(Local) & maridDB(AWS)
- JPA

- Test : JUnit5

- AWS EC2 Linux 2 AMI

* 클라이언트 학습 목적의 프로젝트가 아니기 때문에 화면구성은 Mustache, BootStrap으로 간소화하여 구현

!!! 02/03 13:31 - AWS EC2에서 코드의 배포까지 성공, mariaDB 연결 시 DB Type을 감지하지 못하는 오류 발생
                > 추측되는 원인 : 보안상의 목적으로 서버에 분리 생성한 db properties 파일을 제대로 읽지 못하는것 같음.
                
                cat honup.out > Caused by: java.lang.IllegalStateException: Unable to detect database type
