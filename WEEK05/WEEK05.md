# 변경사항
5주차와 6주차의 스터디 진행 순서를 바꾸게 되었습니다. 6주차 범위인 Cahpter 8: 클래스 단원을 5주차에 진행해주시고 6주차에 Chapter 6: 예외처리를 진행하시면 됩니다.

# 스터디 범위
교재 p.460~473, p.496~497

# 5주차 과제
중점 내용:
1. 클래스, 객체, 인스턴스 세 가지 용어에 대해 각각 개념을 이해해보세요.
2. 객체 지향 프로그래밍에 대해 설명하세요.
2. 클래스 상속에 대해 설명하세요.

# 추가 스터디 내용
좋은 프로그래머가 되기 위해선 프로그래밍 언어 뿐만 아니라 컴퓨터에 대한 이해를 얻기 위해 많은 공부와 경험을 요구합니다.
메모리(RAM)는 실행중인 프로그램(명령어)와 데이터를 저장하는데 사용됩니다. 파이썬의 메모리 구조에 대해 설명하는 다음 블로그 게시물을 순서대로 읽고 요약해옵시다. ([파이썬의 메모리 구조](https://hkim-data.tistory.com/180))
코드영역에 실행할 프로그램의 코드가 저장됨,데이터 영역에 전역변수,정적변수가 저장됨,힙 영역에 사용자가 동적으로 할당하는 변수나 메소드가 저장됨,스택 영역에 지역변수나 매개변수가 저장됨. x=10을 실행하면 10이라는 객체가 메모리에 생성되고,변수 x에 의해 참조됨(x가 10이라는 객체의 주소를 참조함).
y=x을 실행하면 y는 x가 참조하고 있는 객체를 동일하게 참조함(y와 x의 id값은 동일).
sys.getrefcount()는 호출 시 해당 객체를 임시로 참조하여, 객체의 참조 횟수를 증가시킨 상태에서 값을 반환합니다. 그래서 getrefcount()로 확인한 참조 횟수는 실제 참조 횟수보다 1만큼 더 큽니다.
스택 메모리로부터 메서드가 실행,참조자는 stack메모리에 생성됨,객체는 보통heap메모리에 생성됨,가비지 컬렉터는 더 사용할 가능성이 없는 데이터를 메모리에서 제거하는 역할을 합니다(참조자 수가 0이 되는 즉시 메모리에서 해제시킨다)