# Object Oriented Programming (Advanced)

## 상속 
: 한 클래스(부모)의 속성과 메서드를 다른 클래스(자식)가 물려받는 것 (코드 재사용, 계층 구조, 유지 보수 용이)

    class Animal:
    def eat(self):
        print('먹는 중')


    class Dog(Animal):
        def bark(self):
            print('멍멍')


    my_dog = Dog()

    # 부모 클래스(Animal) 메서드 사용 가능
    my_dog.eat()


## 메서드 오버라이딩
: 부모 클래스의 메서드를 같은 이름, 같은 파라미터 구조로 재정의하는 것

    class Animal:
        def eat(self):
            print('Animal이 먹는 중')


    class Dog(Animal):
        # 오버라이딩 (부모 클래스 Animal의 eat 메서드를 재정의)
        def eat(self):
            print('Dog가 먹는 중')

    my_dog = Dog()

    my_dog.eat()  # Dog가 먹는 중

오버로딩 : 같은 이름, 다른 파라미터를 가진 여러 메서드를 정의하는 기능. 파이썬에서는 지원하지 않음

