# freelec-srpingboot2-webservice

# 22.06.05
1. 범위 : TDD , 게시판 만들기
2. 코드 작성중 문제점
2-1 TDD : assertThat(테이블검증 라이브러리) import 안되는 문제발생.
- 해결방안 : 사용해야할 class에서 수동으로 추가함(라이브러리 사용안하면 import문장색이 회색으로 변함. 라이브러리 연결이 안된것이 아니고 사용을 안해서 회색으로 변함)
2-2 게시판 만들기 : 테스트 중 java.lang.Exception: No runnable methods 발생
- 해결방안 : 테스트할 메서드에 어노테이션 누락

# 22.06.05
1. 범위 : 게시판 만들기 내 조회,변경,등록 api 개발 및 mustache 적용
2. 코드 작성중 문제점 : 없음
3. 내용정리
3-1 : Spring 웹 계층
- web Layer : 컨트롤러와 JSP/Freemarker 등의 뷰 템플릿 영역, 필터, 인터셉터, 컨트롤러 어드바이스 등 외부 요청과 응답에 대한 전반적인 영역
- Service Layer : @Service에 사용되는 서비스 영역, 일반적으로 Controller 와 Dao의 중간 영역, @Transactional 이 사용되어야 하는 영역.
- Repository Layer : Database와 같이 데이터 저장소에 접근해야하는 영역.(기존 Dao 영역과 동일)
- Dtos : 계층 간의 데이터 교환을 위한 객체를 사용하는 영역, 예를들어 뷰 템플릿 엔진에서 사용될 객체나 Repository Layer에서 결과로 넘겨준 객체 등.
- Domain Model : 도메인이라 불리는 개발 대상을 모든 사람이 동일한 관점에서 이해할 수 있고 공유할 수 있도록 단순화시킨 것.
3-2 : Spring bean 등록방법
- @Autowired
- Setter
- 생성자(가장 권장하는 방식)

3-3 : Lombok
- RequiredArgsConstructor : final 로 선언된 모둔 필드를 인자값으로 하는 생성자로 만들어줌.

3-4 : JPA 
- 영속성 컨텍스트 : 엔티티를 영구저장하는 환경(추가 정보 필요)


