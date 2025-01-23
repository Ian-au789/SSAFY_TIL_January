# Module
한 파일로 묶인 변수와 함수의 모음, 특정한 기능을 하는 코드가 작성된 파이썬 파일 (.py)

- 내장 모듈 : 파이썬이 미리 작성해둔 변수 및 함수 모음 (math, random, datetime ...)

- import 모듈 -> 모듈.변수 형태로 호출

- from 모듈 import 변수 -> 변수 이름으로 호출 (이름 충돌이 날 확률이 상대적으로 상승)

- 서로 다른 모듈이 같은 이름의 함수를 제공할 경우 충돌 -> 마지막에 import된 이름으로 대체

- as 키워드를 사용해 별칭(alias) 부여해서 충돌 해소 (from module import function as alias)

- 