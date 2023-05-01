# C프로그래밍에 대해

#include <stdio.h> //printf 사용울 위해 헤더 파일 "stdio.h"를 추가

void main() { //프로그램의 시작점인 main함수를 시작
printf("hello~ \n"); //"hell0~"를 출력하고 줄바꿈 문자를 추가
} //main함수의 끝을 나타내는 중괄호
-----------------------------
/*
이 프로그램은 두 수를 키보드로 입력받아 곱의 결과를 출력하는 프로그램
*/
#include <stdio.h> //표준 입출력 라이브러리(printf,scanf)를 포함하는 헤더 파일이다.
#pragma warning(disable:4996) //보안 경고를 무시한다.

int a, b, c; //변수 a,b,c를 전역변수로 선언
int product(int x, int y); //사용자 함수(product) 원형 선언

void main() { //프로그램의 시작점
printf("Enter a number between 1 and 100: "); //첫 번째 숫자 입력 안내 메시지를 출력
scanf("%d", &a); //사용자로부터 첫 번째 숫자를 입력받는다

printf("Enter another number between 1 and 100: "); //두 번째 숫자 입력 안내 메시지를 출력
scanf("%d", &b); //사용자로부터 두 번째 숫자를 입력받는다.

c = product(a, b); //입력받은 두 수를 곱한 값을 c에 저장
printf("%d * %d = %d \n", a, b, c); //결과를 출력
} //main 함수의 끝을 나타내는 중괄호

int product(int x, int y) { //두 수를 곱한 값을 반환하는 함수
return (x * y); //두 수를 곱한 값을 반환
} //product 함수의 끝을 나타내는 중괄호
--------------------------------
#include <stdio.h> //stdio.h 헤더 파일을 포함
#define IN "원의 반지름은 100입니다. \n" //IN이라는 상수 매크로를 정의하고 문자열을 할당한다.
#define PI 3.1415926535 //PI라는 상수 매크로를 정의하고 값을 할당
#define AREA(X) (PI*(X)*(X)) //AREA라는 매크로를 정의하고, X의 제곱에 PI를 곱한 값으로 계산
#define OUT printf("원의 면적을 구하고 프로그램을 종료합니다. \n") //OUT이라는 매크로를 정의하고, 문자열을 출력

void main() { //프로그램의 시작점인 main함수를 시작
printf("%s \n", IN); //IN이라는 매크로에 할당된 문자열을 출력
printf("원의 면적은 %1.5f입니다. \n\n", AREA(100)); //AREA 매크로에 100을 대입하여 면적을 계산하고, 소수점 이하 5자리까지 출력.
OUT; //OUT이라는 매크로에 할당된 문자열을 출력
} //main함수의 끝을 나타내는 중괄호이다.