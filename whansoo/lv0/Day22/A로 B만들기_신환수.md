# 🦄[프로그래머스]A로 B 만들기

### 🧡문제 설명
문자열 before와 after가 매개변수로 주어질 때, before의 순서를 바꾸어 after를 만들 수 있으면 1을, 만들 수 없으면 0을 return 하도록 solution 함수를 완성해보세요.
***
### 💛제한사항
- 0 < before의 길이 == after의 길이 < 1,000
- before와 after는 모두 소문자로 이루어져 있습니다.
### 💙입출력 예 설명
입출력 #1
- "olleh"의 순서를 바꾸면 "hello"를 만들 수 있습니다.

입출력 #2
- "allpe"의 순서를 바꿔도 "apple"을 만들 수 없습니다.
***
### 💜나의 풀이
```javascript
function solution(before, after) {
   return before.split('').sort().join('') === after.split('').sort().join('') ? 1 : 0
}
```