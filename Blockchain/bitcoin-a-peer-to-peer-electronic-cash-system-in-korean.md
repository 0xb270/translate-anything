[Original](./original/bitcoin.pdf)

# 비트코인: 개인간 전자 화폐 체계
사토시 나카모토  
satoshin@gmx.com  
www.bitcoin.org  

## 초록.
전자 화폐의 완전한 개인간 버전은 금융 기관을 거칠 필요 없이 한 쪽에서 다른 쪽으로 직접 온라인 결제를 할 수 있게 한다. 디지털 서명이 해결책의 일부분이지만, 만약 신뢰하는 제 3자가 [이중 소비(double-spending)](https://en.wikipedia.org/wiki/Double-spending)를 여전히 막을 수 없다면 주요 장점이 사라진다. 우리는 개인간 네트워크를 이용한 이중 소비 문제 해결책을 제안한다. 이 네트워크는 해시 기반 [작업 증명(Proof-of-Work)](https://en.wikipedia.org/wiki/Proof-of-work_system)의 연속적인 체인 안에 [트랜잭션](https://www.quora.com/What-is-a-Blockchain-transaction)들을 해싱하여 집어넣어서 트랜잭션들의 시간 도장을 찍는데, 이는 작업 증명을 다시 할 필요 없이 바뀔 수 없는 기록을 생성한다. 최장 체인은 여러 목격된 이벤트들을 증명할 뿐 아니라, 최대 CPU 연산력 풀로부터 나왔다는 것을 나타낸다. 주 CPU 연산력이 이 네트워크를 공격하는 데 협조하지 않는 노드들로부터 제어되는 한, 이들은 최장 체인을 만들어내고 공격자들을 따돌린다. 이 네트워크 자체로는 최소한의 구조를 요구한다. 메세지들은 [최선의 노력(best effort basis)](https://financial-dictionary.thefreedictionary.com/best-efforts+basis)으로 퍼뜨려지고, 노드들은 이 네트워크를 떠나거나 다시 합칠 수 있고, 없었던 동안 무엇이 일어났는지에 대한 증명으로 최장 작업 증명 체인을 받아들인다.

## 1. 도입
인터넷에서의 상업은 전자 결제를 처리하는 신뢰하는 제 3자로서의 금융 기관에 거의 독점적으로 의존하게 된다. 