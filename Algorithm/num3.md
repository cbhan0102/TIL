*문제설명

정수를 담고 있는 배열 arr의 평균값을 return하는 함수, solution을 완성해보세요.


*제한사항

arr은 길이 1 이상, 100 이하인 배열입니다.
arr의 원소는 -10,000 이상 10,000 이하인 정수입니다.




*입출력 예 설명

-

----------

*문제 풀기 전에 정리


평균을 구하는 간단하고 쉬운 문제이다.
1. 배열에 담긴 요소들의 합을 구한다.
2. 요소들의 합을 배열의 길이 (=요소 갯수)로 나눈다.

----------

*문제 풀이

function solution(arr) {
var answer = 0;
let sum = 0;

    for (let i = 0; i < arr.length; i++){
     sum += arr[i];   // 배열의 요소들을 하나씩 더한다.
    }
    return answer = sum / arr.length; // 더한 값과 배열의 길이(=요소 갯수)를 나눈다.
}
// reduce() 메서드를 사용해 풀어보기
function solution(arr) {
return arr.reduce((sum, current) => sum + current) / arr.length;
}
reduce() : 배열의 각 요소에 대해 주어진 리듀서 함수를 실행하고, 하나의 결과값을 반환한다.
const reducer = (a, b) => a + b;
const array = [1, 2, 3, 4];

console.log(array.reduce(reduer));
// 10