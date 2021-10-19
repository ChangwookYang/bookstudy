# bookstudy

gradle
* ext
    * build.gradle에서 사용하는 전역변수를 설정
* Repositories
    * 각종 의존성(라이브러리)들을 어떤 원격 저장소에서 받을지를 정한다.
    * mavenCentral, jcenter
        * 기본적으로 많이 사용하지만 최근 업로드 난이도 때문에 jcenter도 많이 사용한다.
        * 라이브러리를 업로드할 수 있고, 원격저장소에서 받아오기 위해 선언
* Dependencies
    * 프로젝트 개발에 필요한 의존성들을 선언
    * Compile 메소드 안에 라이브러리의 이름을 추가한다. 
        * 버전을 명시하지 않아야 ext에서 선언한 버전을 따라가게 된다.

@SpringBootApplication
* 스프링부트의 자동설정, 스프링 Bean 읽기와 생성을 모두 자동으로 설정한다.
* @SpringBootApplcation이 있는 위치부터 설정을 읽어나가기 때문에 이 클래스는 항상 프로젝트 최상단에 위치한다.

SpringApplication.run
* 내장 WAS를 실행한다.
* 내장 WAS란 별도로 외부에 WAS를 두지 않고 애플리케이션을 실행할때 내부에서 WAS를 실행하는 것을 이야기한다.
* 내부 WAS로 인해 서버에 톰캣을 설치할 필요가 없게 되고 스프링부트로 만들어진 Jar 파일로 실행하면된다.
* Jar : Java 패키징 파일
* 내장 Was로 언제 어디서나 같은 환경에서 스프링부트를 배포할 수 있다.


@RestController 
* 컨트롤러를 JSON을 반환하는 컨트롤러로 만들어준다.
* 예전에는 @ResponseBody를 각 메소드마다 선언했던것을 한번에 사용할 수 있게 해준다.


테스트코드
* @RunWith(SpringRunner.class)
    * 테스트를 진행할때 JUnit에 내장된 실행자 외에 다른 실행자를 실행
    * SpringRunner라는 스프링 실행자를 사용
    * 즉, 스프링부트 테스트와 JUnit사이에 연결자 역할을한다.

@RequiredArgsConstructor
* final 필드가 포함된 생성자를 생성해 준다.


 
