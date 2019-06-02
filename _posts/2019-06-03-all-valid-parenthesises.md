---
layout: post
title: K쌍의 괄호로 표현 가능한 유효한 모든 괄호쌍 구하기
categories: recursion
comments: true
---

정수 K를 입력으로 받으면, K쌍으로 표현이 가능한 유효한 모든 괄호쌍을 구하는 문제입니다.
```
입출력 예:
Input: K=1
Output: ()
Input: K=2
Output: ()(), (())
Input: K=3
Output: ((())), (()()), (())(), ()(()), ()()()
```

이 문제는 여는 괄호 `(`와 닫는 괄호 `)`의 개수가 모두 K개가 되는 표현 중에서,
왼쪽부터 읽으면서 출현하는 여는 괄호의 개수보다 닫는 괄호의 개수가 더 많아지면 유효하지 않은 표현이 된다는 성질을 이용할 수 있습니다.

{% gist 6ce93f650c35b62eb0215f11233efb99 %}

전체 코드는 [Go Playground](https://play.golang.org/p/GMVVG21nNxH){:target="_blank"}에서 확인하고, 직접 실행해 볼 수 있습니다.
