# JS 100문제 모음집 Part.1
JS 알고리즘 100문제 모음집 1권

## 1. 배열의 삭제
다음 배열에서 400, 500를 삭제하는 code를 입력하세요.
```js
const nums = [100, 200, 300, 400, 500];
```
<strong>- 내가 푼 답</strong>
```js
  nums.slice(0, -2);
```
<br>

## 2. 배열의 내장함수

```js
const arr = [200, 100, 300];
```
<strong>- 내가 푼 답</strong>
```js
  arr.splice(2, 0, 10000);
  console.log(arr);
```
