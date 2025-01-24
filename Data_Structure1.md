# Method 1 
객체에 속한 함수 : 객체의 상태를 조작하거나 동작 수행

- 메서드는 클래스(class) 내부에 정의된 함수

- 'variable'.method()

## Str Method
str은 변경 불가 자료형. str.method는 문자를 바꾸는 게 아니라 새로운 문자열을 반환하는 동작

1. .find(x) : x의 첫 번째 위치를 반환. 없으면 -1 반환

2. .index(x) : x의 첫 번째 위치 반환. 없으면 에러

3. is.upper(x) : 문자열이 모두 대문자로 이루어져 있는지 확인

4. is.lower(x) : 문자열이 모두 소문자로 이루어져 있는지 확인

5. is.alpha(x) : 문자열이 알파벳으로만 이루어져 있는지 확인

6. .replace(old, new[, count]) : old의 글자를 new로 바꿔서 반환. count는 바꾸고자 하는 개수

7. .strip([ chars ]) : 문자열의 시작과 끝에 있는 공백 혹은 지정한 문자 제거

8. .split(sep = None) : sep을 구분자 문자열로 사용하여 문자열에 있는 단어들의 리스트 반환

9. 'seperator'.join(iterable) : iterable의 문자열을 연결한 문자열을 반환

## List Method

