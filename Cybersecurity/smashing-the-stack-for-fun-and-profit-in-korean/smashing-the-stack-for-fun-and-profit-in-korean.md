[original](./original/stack_smashing.pdf)

.oO Phrack Oo.  
  
7권 49호, 총 16 중 14번째  
  
BugTraq, r00t, 그리고 Underground.Org가 제공함  

# 재미 그리고 이득을 위한 스택 격파하기

## Aleph One
aleph1@underground.org

\`스택 격파\` [C 프로그래밍] n. 많은 C 구현체에서, 루틴 안에 동적 할당된 배열의 끝을 지나쳐 씀으로서 실행 스택을 더럽히는 것이 가능하다. 이러한 코드를 스택 격파라 불리며, 이는 루틴으로부터 리턴하는 것으로 임의의 주소로 점프하는 것을 일으킬 수 잇다. 이것은 인류에게 알려진 가장 교활한 데이터 의존적인 버그들을 일으킬 수 있다. 동의어로 스택 폐기, 스택 갈겨 쓰기, 스택 실종이 있다; 스택 어지럽힘([mung](http://www.catb.org/~esr/jargon/html/M/mung.html) the stack)이라는 용어는, 의도적으로 행하여지는 것이 아니기 때문에, 쓰이지 않는다. 스팸을 보라; [`alias`](https://ss64.com/bash/alias.html) 버그, [코어 위의 환당고 춤](http://www.catb.org/jargon/html/F/fandango-on-core.html), 메모리 누수, 앞서기로 인한 누락, [오버런 스크루](http://www.catb.org/jargon/html/O/overrun-screw.html)를 보라.