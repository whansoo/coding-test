# 🦄[프로그래머스]k의 개수

### 🧡문제 설명
1부터 13까지의 수에서, 1은 1, 10, 11, 12, 13 이렇게 총 6번 등장합니다. 정수 i, j, k가 매개변수로 주어질 때, i부터 j까지 k가 몇 번 등장하는지 return 하도록 solution 함수를 완성해주세요.
***
### 💛제한사항
- 1 ≤ i < j ≤ 100,000
- 0 ≤ k ≤ 9
### 💙입출력 예 설명
입출력 #1
- 10부터 50까지 5는 15, 25, 35, 45, 50 총 5번 등장합니다. 따라서 5를 return 합니다.

입출력 #2
- 3부터 10까지 2는 한 번도 등장하지 않으므로 0을 return 합니다.
***
### 💜나의 풀이
```javascript
function solution(i, j, k) {
    let count = i-1;
    let newarr = [];
   for(let a  = i; i<=j; i++) {
       count++
      newarr.push(count)
   }
 return newarr.join('').split('').filter((a) => a.includes(k)).length
   
}
```