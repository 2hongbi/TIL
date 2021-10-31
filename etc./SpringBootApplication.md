***@SpringBootApplication*** 은 스프링 부트의 자동 설정, 스프링 Bean 읽기와 생성을 모두 자동으로 생성함.

***@SpringBootApplication***이 있는 위치부터 설정을 읽어감 -> 이 클래스는 항상 프로젝트의 최상단에 위치해야 함

```{java}
import org.springframework.boot.SpringApplication;
import org.springframework.boot.autoconfigure.SpringBootApplication;

@SpringBootApplication
public class Application {
    public static void main(String[] args) {
        SpringApplication.run(Application.class, args);
    }
}
```

main 메소드에서 실행하는 SpringApplication.run으로 인해 내장 WAS(Web Application Server, 웹 애플리케이션 서버)를 실행
  - 내장 WAS : 별도로 외부에 WAS를 두지 않고 애플리케이션을 실행할 때 내부에서 WAS를 실행하는 것
  - 이는 항상 서버에 톰캣을 설치할 필요가 없게 되고, 스프링 부트로 만들어진 Jar 파일로 실행하면 됨
  - 스프링부트에서는 내장 WAS 사용을 권장




\[출처\] 스프링 부트와 AWS로 혼자 구현하는 웹 서비스
