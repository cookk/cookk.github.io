---
title: "Coding Interview - Linked List"
layout: post
date: 2019-12-29 11:11
headerImage: false
tag:
- coding-interview
category: blog
author: cook
description: Linked List
---

# 연결리스트
- 연결리스트는 차례로 연결된 노드를 표현하는 자료구조
- 단방향 연결리스트에서는 각 노드가 다음 노드를 가리키고,
- 양방향 연결리스트에서는 각 노드가 다음 노드와 이전 노드를 함께 가리킨다
- **배열과는 달리, 특정 인덱스를 상수 시간에 바로 접근할 수 없음**
- **노드의 추가나 삭제는 상수 시간에 할 수 있다. 가운데 끼워넣으면 되니까**
- **Runner 기법**
  - 부가 포인터를 이용해서 원하는 작업을 하는 것
  - 예를 들어, 한칸씩 이동하는 포인터와 두칸씩 이동하는 포인터를 같이 이동시킨다
    - 두칸씩 이동하는 포인터가 마지막에 다다르면, 한칸씩 이동하는 포인터는 연결리스트의 가운데에 위치할 것
- **재귀 문제**
  - 연결 리스트 문제는 재귀 호출에 많이 의존한다. 연결리스트 문제를 풀다 막힌다면, 재귀적 접근법을 시도하자
  - 다만 재귀 호출 깊이가 n이 되면, 해당 알고리즘은 적어도 O(n)만큼의 공간을 사용한다는것을 명심하자


## 면접 문제
- 2.1 중복 없애기
  - 두바퀴 돌기..?
- 2.2 뒤에서 k번째 원소 구하기
  - k만큼 거리가 있는 두개의 포인터를 이동시키면 될 듯. 뒤의 포인터가 끝에 다다르면 앞의 포인터가 뒤에서 k번째 노드
- 2.3 중간 노드 삭제
  - 이것도 두개의 포인터를 이용하면 될 듯. 하나는 그냥 이동, 하나는 두칸씩 이동
