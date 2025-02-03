# Object Oriented Programming (OOP)

: 데이터와 함수를 하나의 단위(**객체**)로 묶어서 관리, 객체들을 조합하고 재활용하는 방식으로 프로그램 구성 (데이터와 메서드의 결합)

-> 상속, 코드 재사용성, 유지보수성 등의 이점

## Object
: 실제 존재하는 사물을 추상화한 것 (속성, 동작)

## Class

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

2. 생성자 메서드 __init__ : 인스턴스 생성 시 자동 호출되는 특별한 메서드, 객체의 초기값을 설정

3. 인스턴스 변수(속성) : self.변수명 형태로 정의, 각 인스턴스 별 고유한 값

4. 클래스 변수(속성) : 클래스 내부에 직접 정의, 모든 인스턴스가 공유하는 속성

## Instance

: 클래스를 통해 생성된 객체 (클래스라는 인쇄판이 찍어낸 인쇄물)

    p1 = Person('Alice', 25)
    p2 = Person('Bella', 30)

ex) 변수에 값을 할당할 때 그 변수는 해당 데이터 타입 클래스의 인스턴스이다. (str, int, list, dict..)

메서드도 데이터 타입 클래스에 만들어져 있는 동작

## Method

: 클래스 내부에 정의된 함수로, 객체의 동작 정의

### 인스턴스 메서드
: 각 인스턴스에서 호출해 인스턴스의 상태를 조작하거나 동작을 수행

- 클래스 내부에 정의되는 메서드의 기본

- 반드시 첫 번째 인자로 인스턴스 자신(**self**)을 받음 (매개변수의 이름일 뿐이며 다른 이름 사용은 가능하지만 권장x)

- 큰 틀에서 생성자 메서드도 인스턴스 메서드에 포함


### 클래스 메서드

: 클래스가 호출, 클래스 변수를 조작하거나 클래스 레벨의 동작 수행

    class Person:
        population = 0

        def __init__(self, name):
            self.name = name
            Person.increase_population()

        @classmethod
        def increase_population(cls):
            cls.population += 1

- **@classmethod** 데코레이터를 사용하여 정의

- 호출 시 첫 번째 인자로 해당 메서드를 호출하는 클래스(**cls**)가 전달

- 클래스 메서드를 인스턴스가 호출할 때는 cls가 아닌 클래스 이름을 사용


### 스태틱 메서드
: 클래스, 인스턴스 상관없이 독립적으로 동작

- **@staticmethod** 데코레이더 사용

- 호출 시 자동으로 전달 받는 인자 존재 x (self, cls 등)

- 라이브러리 함수와 비슷한 느낌 
