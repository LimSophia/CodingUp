### *[Functions in C]최대 정수 출력 *

*문제*
Write a function int max_of_four(int a, int b, int c, int d) which reads four arguments and returns the greatest of them.

```c
#include <stdio.h>

int max_of_four(int a, int b, int c, int d) {

    int max_var = 0;

    max_var = (a > b) ? a : b;
    max_var = (max_var > c) ? max_var : c;
    max_var = (max_var > d) ? max_var : d;

    return max_var;
}

int main() {
    int a, b, c, d;
    scanf("%d %d %d %d", &a, &b, &c, &d);
    int ans = max_of_four(a, b, c, d);
    printf("%d", ans);

    return 0;
}
```
![image](https://github.com/minahLim/CodingTest/assets/146914181/a390c20c-dfd3-4aa4-8600-02384a82cb5c)<br>
<hr>

출처: 해커랭크<br>
https://www.hackerrank.com/challenges/functions-in-c/problem?isFullScreen=true
