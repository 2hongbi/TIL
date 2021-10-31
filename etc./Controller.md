```{java}
@RestController
public class HelloController {

    @GetMapping("/hello")
    public String hello() {
        return "hello!";
    }
}
```

1. @RestController
    - 컨트롤러를 JSON을 반환하는 컨트롤러로 만들어줌
    - 예전에는 @ResponseBody를 각 메소드마다 선언했던 것을 한번에 사용할 수 있게 해줌

2. @GetMapping
    - HTTP Method인 Get 요청을 받을 수 있는 API를 만들어 줌
    - 예전에는 @RequestMapping(method=RequestMethod.GET) 으로 사용
  
  
  
 위 코드는 /hello로 요청이 오면 문자열 hello를 반환해주는 기능을 가짐
