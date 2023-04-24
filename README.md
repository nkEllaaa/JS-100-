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
<br>

## 3. 변수의 타입
💡 문제 : 다음 출력 값으로 올바른 것은?
```js
var arr = [100, 200, 300];
console.log(typeof(arr));
```
<strong>- 내가 푼 답</strong>
```js
object 
//Array.isArray(판별하고싶은 데이터)
//Array.isArray() 메서드는 인자가 Array인지 판별한다. true, false로 반환
```
<br>

## 4. 변수의 타입2
💡 문제 : 다음 변수 a를 typeof(a)로 넣었을 때 출력될 값과의 연결이 알맞지 않은 것은?
```js
1)  입력 : a =1,   출력 : number
2)  입력 : a = 2.22,   출력 : boolean
3)  입력 : a = 'p',   출력 : string
4)  입력 : a = [1, 2, 3],   출력 : object
```
<strong>- 내가 푼 답</strong>
```js
2 // number
```
<br>

## 5. for문 계산
💡 문제 : 다음 코드의 출력 값으로 알맞은 것은?
```js
var a = 10;
var b = 2;

for(var i=1; i<5; i+=2){
    a += i;
}

console.log(a+b);
```
<strong>- 내가 푼 답</strong>
```js
16 
// 10 + 1 + 3 + 2 
// i가 2씩 증가하는 것 주의
```
<br>

## 6. false
💡 문제 : 다음은 자바스크립트 문법 중에서 False로 취급하는 것들 입니다.
앗, False로 취급하지 않는 것이 하나 있네요! True를 찾아주세요.
```js
1)  NaN
2)  1
3)  ""
4)  0
5)  undefined
```
<strong>- 내가 푼 답</strong>
```js
2 
// NaN은 거짓 같은 값(Falsy, falsey로 쓰이기도 함) 값은 불리언 문맥에서 false로 평가되는 값이다.
// number에서 0이 아닌 수는 true
// "" 빈 문자열
// undefined 역시 falsy
```
<br>

## 7. 변수명
💡 문제 : 다음 중 변수명으로 사용할 수 없는 것 2개를 고르시오.
```js
1)  age
2)  Age
3)  let
4)  _age
5)  1age
```
<strong>- 내가 푼 답</strong>
```js
3, 5
// let 은 JavaScript의 예약어이다. 
// 숫자로 시작할 수 없다. age1은 가능
```
<br>

## 8. 객체의 키 이름 중복
💡 문제 : 자바스크립트 객체를 다음과 같이 만들었다. 출력값을 입력하시오. (출력값은 공백을 넣지 않습니다.)
```js
var d = {
    'height':180,
    'weight':78,
    'weight':84,
    'temperature':36,
    'eyesight':1
};

console.log(d['weight']);
```
<strong>- 내가 푼 답</strong>
```js
84
// weight에 78 -> 84로 재할당
```
<br>

## 10. 객체의 키 이름 중복
💡 문제 : 다음 소스 코드를 완성하여 날짜와 시간을 출력하시오.
```js
데이터
var year = '2019';
var month = '04';
var day = '26';
var hour = '11';
var minute = '34';
var second = '27';

var result = //빈칸을 채워주세요

console.log(result);


출력
2019/04/26 11:34:27
```

<strong>- 내가 푼 답</strong>
```js
const result = year.concat('/',month,'/',day,' ',hour,':',minute,':',second) 
console.log(result);
```
```js
const allData = [year,month,day,hour,minute,second]
const date = allData.slice(0,3).join('/')
const time = allData.slice(2, ).join(':')
console.log(date + ' ' + time)
// concat이 번거롭다고 느꼈는데 더 좋은(?) 방법은 없을까?
```
<br>

## 10. 별 찍기
💡 문제 : 크리스마스 날, 은비는 친구들과 함께 파티를 하기로 했습니다. 그런데, 크리스마스 트리를 사는 것을 깜빡하고 말았습니다. 온 가게를 돌아다녀 봤지만 크리스마스 트리는 모두 품절이었습니다. 
하는 수 없이 은비는 프로그래밍으로 트리를 만들기로 합니다. 
```js
입력
5

출력
    *
   ***
  *****
 *******
*********
```
<strong>- 내가 푼 답</strong>
```js
    
```
<br>

## 11.  for를 이용한 기본 활용
💡 문제 : 1부터 100까지 모두 더하는 Code를 <pass> 부분에 완성하세요. for를 사용해야 합니다.
```js
let s = 0;

//pass

console.log(s);
```
<strong>- 내가 푼 답</strong>
```js
for (let i=0; i<100; i++){
  s += i
}
```
<br>
