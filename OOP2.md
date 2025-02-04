# Class Inheritance

## 상속

: 한 클래스(부모)의 속성과 메서드를 다른 클래스(자식)가 물려받는 것 (코드 재사용, 계층 구조, 유지 보수 용이)

    class Parent:
        def cook(self):
            print("밥 먹자")


    class Child(Parent):             # 상속 
        def eat(self):
            print("잘 먹겠습니다.)

    child1 = Child('중학생')

    child1.cook()        #부모 클래스의 메서드 사용 가능 

## 메서드 오버라이딩

: 부모 클래스의 메서드를 같은 이름, 같은 파라미터 구조로 재정의하는 것

    class Parent:
        def cook(self):
            print("밥 먹자")


    class Child(Parent):    
        def cook(self):              # 덮어 쓰기 
            print("맛있게 드세요.)

    child1 = Child('중학생')

    child1.cook()       

오버로딩 : 같은 이름, 다른 파라미터를 가진 여러 메서드를 정의하는 기능. 파이썬에서는 지원하지 않음

## 다중 상속

: 둘 이상의 상위 클래스로부터 여러 행동이나 특징을 상속받을 수 있는 것, 중복된 속성이나 메서드가 존재할 시 상속 순서에 의해 결정. (MRO 알고리즘)

### super()

: 부모 클래스(또는 상위 클래스)의 메서드를 호출하기 위해 사용하는 내장 함수

    class Parent:
        def __init__(self, name, age):
            self.name = name
            self.age = age


    class Child(Parent):
        def __init__(self, name, age, student_no):
            # super()를 통해 Person의 __init__ 메서드 호출
            super().__init__(name, age, number, email)
            self.student_no = student_no

- MRO 알고리즘의 순서에 따라 탐색, 만약 상위 클래스가 존재하지 않으면 동일한 레벨의 상속 순서 다음 클래스를 호출

- 클래스 이름이 변경되거나 부모 클래스가 교체될 시 코드 수정 최소화 가능

- class.mro() 메서드로 mro 순서를 파악 가능
