문제 설명
머쓱이네 피자가게는 피자를 두 조각에서 열 조각까지 원하는 조각 수로 잘라줍니다. 피자 조각 수 slice와 피자를 먹는 사람의 수 n이 매개변수로 주어질 때, n명의 사람이 최소 한 조각 이상 피자를 먹으려면 최소 몇 판의 피자를 시켜야 하는지를 return 하도록 solution 함수를 완성해보세요.


제한사항
2 ≤ slice ≤ 10
1 ≤ n ≤ 100

최종 코드

function solution(slice, n) {
let pizzasNeeded = Math.ceil(n / slice);
return pizzasNeeded;
}

// 예제 사용법:
const slice = 3; // 피자 한 판을 3조각으로 나누는 경우
const n = 7; // 7명의 사람이 최소 한 조각 이상 피자를 먹어야 함

const result = solution(slice, n);
console.log(`최소 ${result}판의 피자를 시켜야 합니다.`);