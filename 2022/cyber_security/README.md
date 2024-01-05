# 2022_Reinforcement learning TeamProject
###### 강화학습 이후 공격 영상
![강화학습 시각화 실행영상](https://github.com/PG-RDC/TeamProject/assets/130644995/bf512889-fd34-40bf-8899-92a56d95464c)
###### epoch당 step
![KakaoTalk_20221207_150210538](https://github.com/PG-RDC/TeamProject/assets/130644995/d4fc0236-4f52-44af-8798-79304543d795)
###### epoch당 reward
![KakaoTalk_20221207_150243362](https://github.com/PG-RDC/TeamProject/assets/130644995/b7f3a245-0b09-446d-bb02-6af64a64e9be)

###### 사이버 보안 강화학습! 해킹하는 인공지능을 만들어 보자!

#### Main idea: 
- Environment는 graph로 구현
- action
  - local 공격 1개
  - remote 공격 2개
  - credit 획득 1개

## 결론
action, reward 설정이 잘 된다면 강화학습은 잘 동작한다.

#### 다음 코드에 사용하실 경로를 넣어주면 학습이 가능합니다.
DQN부분의 PATH 부분
```python
PATH = 'your path'
```

#### action 함수를 추가하고, action의 수를 늘려주시면 변경해서 강화학습이 가능합니다.
