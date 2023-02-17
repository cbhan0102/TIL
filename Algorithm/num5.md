*문제설명

자연수 n이 주어졌을 때, n의 다음 큰 숫자는 다음과 같이 정의 합니다.

조건 1. n의 다음 큰 숫자는 n보다 큰 자연수 입니다.
조건 2. n의 다음 큰 숫자와 n은 2진수로 변환했을 때 1의 갯수가 같습니다.
조건 3. n의 다음 큰 숫자는 조건 1, 2를 만족하는 수 중 가장 작은 수 입니다.
예를 들어서 78(1001110)의 다음 큰 숫자는 83(1010011)입니다.

자연수 n이 매개변수로 주어질 때, n의 다음 큰 숫자를 return 하는 solution 함수를 완성해주세요.


*제한사항

n은 1,000,000 이하의 자연수 입니다.




*입출력 예 설명

입출력 예#1
문제 예시와 같습니다.
입출력 예#2
15(1111)의 다음 큰 숫자는 23(10111)입니다.
----------

*문제 풀기 전에 정리


n(양꼬치) = 12,000
k (음료수) = 2,000
n(양꼬치) 10인분부터 k 빼주기

----------

*문제 풀이

function countOne(num) {
let count = 0, ejin = num.toString(2).split('');
for(let i = 0; i < ejin.length; i++) {
if (ejin[i] == 1) { count++; }
}
return count;
}

function solution(n) {
let testNum = n;
while(true) {
testNum++;
if(countOne(testNum) == countOne(n)) return testNum;
}
}


처음에는 이렇게 두 개의 함수를 만들었다.

countOne(num)은 자연수를 입력받고 2진수 변환 후 1의 갯수를 세어주는 함수
solution(n)은 반복문과 countOne(num)을 통해 n의 1의 갯수와 다음 자연수들의 1의 갯수를 비교하고, 일치하는 값을 찾았을 때 멈추는 함수
이렇게 풀어도 효율성 테스트까지 문제 없이 바로 통과할 수 있었다.

근데 작성한 코드를 쳐다보고 있다보니 더 간결하고, 더 읽기 쉽게 작성할 수 있을 것 같다는 생각이 들었다.

더 간결한 문제풀이
function solution(n) {
let oneNum = n.toString(2).split("1").length;
while (true) {
n++;
if (n.toString(2).split("1").length === oneNum) return n;
}
}
split("1").length를 통해 2진수로 변환된 값의 1의 갯수를 손쉽게 찾을 수 있었고,
덕분에 조금 더 간결하고 만족스러운 코드를 작성할 수 있었다.