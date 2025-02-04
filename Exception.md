# Error and Exception

## 디버깅

: 소프트웨어에서 발생하는 오작동의 원인을 식별하여 수정하는 작업

- print 함수 활용해서 변수나 특정 함수 결과 확인

- 개발 환경에서 제공하는 기능 활용

- Python tutor 활용

## 에러

: 프로그램 실행 중 발생하는 예외 상황

1. Syntax Error : 프로그램 구문이 올바르지 않은 문법적 오류 (프로그램 실행 x)

2. Exception : 프로그램 실행 중 감지되는 에러

## 예외 처리

: 예외가 발생했을 때 프로그램이 비정상적으로 종료되지 않고, 적절하게 처리할 수 있도록 하는 방법

- try : 예외가 발생할 수 있는 코드 작성

- except : 예외가 발생했을 때 실행할 코드 작성

- else : 예외가 발생하지 않았을 때 실행할 코드 작성

- finally : 예외 발생 여부와 상관없이 항상 실행할 코드 작성

<try - except 구조>

    try:
    num = int(input())
    print(10 / num)

    except: ValueError
        print("type in number")

    except: ZeroDivisionError
        print("cannot divide by 0")

    except:
        print("unexpected error occured")

### Guideline

- 내장 예외의 상속 계층구조 주의 -> except 절로 분기 시 반드시 **하위 클래스**를 먼저 확일할 수 있도록 순서 결정

- as 키워드를 사용해서 예외 객체를 받아 상세한 예외 정보 활용

- try-except 와 if-else문 함께 활용

