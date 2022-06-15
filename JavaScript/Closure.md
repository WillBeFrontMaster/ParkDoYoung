# Closure

---

###### 본 문서는 MDN문서를 기반으로 작성되었습니다([링크](https://developer.mozilla.org/ko/docs/Web/JavaScript/Closures))

---

### Closure?
- 클로저는 함수와 함수가 선언된 어휘적 환경의 조합이다. (MDN 설명)
- 클로저(Closure)는 일급 객체 함수(first-class functions)의 개념을 이용하여 유효범위(scope)에 묶인 변수를 바인딩 하기 위한 일종의 기술이다.([블로그](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwim3sb-j6_4AhUTglYBHUVAAN4QFnoECBAQAQ&url=https%3A%2F%2Fheropy.blog%2F2017%2F11%2F10%2Fclosure%2F&usg=AOvVaw01kCdrjUgjxqlKeeYKQMBi))
- 클로저란 이미 생명 주기가 끝난 외부 함수의 변수를 참조하는 함수를 클로저라고 합니다.([블로그](https://victorydntmd.tistory.com/44))

클로저를 위와 같이 설명하곤 한다. 클로저의 정의가 다양하게 나오는 이유는
``` javascript
function makeFunc() {
  var name = 'Mozilla';
  function displayName() {
    alert(name);
  }
  return displayName;
}

var myFunc = makeFunc();
myFunc();
```
