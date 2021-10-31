```{python}
  buildscript {
    ext {
        springBootVersion = '2.4.4'
    }
    repositories {
        mavenCentral()
    }
    dependencies {
        classpath("org.springframework.boot:spring-boot-gradle-plugin:${springBootVersion}")
    }
}
```

- ext : build.gradle에서 사용하는 전역변수 설정
- repositories : 각종 의존성(라이브러리)들을 어떤 원격 저장소에서 받을지 정함
- dependencies : 프로젝트 개발에 필요한 의존성들 선언
