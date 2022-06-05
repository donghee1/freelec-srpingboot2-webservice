# freelec-srpingboot2-webservice

# 22.06.05
1. 범위 : TDD , 게시판 만들기
2. 코드 작성중 문제점
2-1 TDD : assertThat(테이블검증 라이브러리) import 안되는 문제발생.
- 해결방안 : 사용해야할 class에서 수동으로 추가함(라이브러리 사용안하면 import문장색이 회색으로 변함. 라이브러리 연결이 안된것이 아니고 사용을 안해서 회색으로 변함)
2-2 게시판 만들기 : 테스트 중 java.lang.Exception: No runnable methods 발생
- 해결방안 : 테스트할 메서드에 어노테이션 누락
- 
