# JS 100문제 모음집 Part.1
JS 알고리즘 100문제 모음집 1권

## 1. 배열의 삭제
💡 문제 : 다음 배열에서 400, 500를 삭제하는 code를 입력하세요.
```js
const nums = [100, 200, 300, 400, 500];
```
<strong>- 내가 푼 답</strong>
```js
  return nums.slice(0, -2); //slice는 원본배열의 값을 변화시키지 않는다.
```
<br>

## 2. 배열의 내장함수
💡 문제 : 배열 내장함수를 이용하여 코드를 입력하고 다음과 같이 출력되게 하세요.
```js
const arr = [200, 100, 300];
```
<strong>- 내가 푼 답</strong>
```js
  arr.splice(2, 0, 10000);
  console.log(arr);
```
