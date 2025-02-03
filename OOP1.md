# Object Oriented Programming (OOP)

: 데이터와 함수를 하나의 단위(**객체**)로 묶어서 관리, 객체들을 조합하고 재활용하는 방식으로 프로그램 구성 (데이터와 메서드의 결합)

-> 상속, 코드 재사용성, 유지보수성 등의 이점

## Object
: 실제 존재하는 사물을 추상화한 것 (속성, 동작)

### Class

- 객체를 만들기 위한 설계도 (객체 찍어내는 인쇄판)

- 데이터와 기능을 함께 묶어 관리하는 방법

- 파이썬에서 타입을 표현하는 방법

<문법>

class Person:

    def __init__ (self, name, age):
        self.name = name
        self.age = age

    def introduce(self):
        print("안녕하세요, 저는 {self.name}, 나이는 {self.age} 입니다")

1. 클래스 이름은 파스칼케이스 방식으로 작성 (style guide)


2. 생성자 메서드 __init__ : 객체의 초기값을 설정


### Instance

: 클래스를 통해 생성된 객체 (클래스라는 인쇄판이 찍어낸 인쇄물)

    p1 = Person('Alice', 25)
    p2 = Person('Bella', 30)

ex) 변수에 값을 할당할 때 그 변수는 해당 데이터 타입 클래스의 인스턴스이다. (str, int, list, dict..)

메서드도 데이터 타입 클래스에 만들어져 있는 동작

