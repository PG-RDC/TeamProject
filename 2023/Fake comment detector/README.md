# 2023_AI system TeamProject

![Fake comment](https://github.com/PG-RDC/TeamProject/assets/130644995/631b4dc6-cbca-474d-a64a-ad8ac68f8c23)

###### 최근 인공지능의 발달과 sns, 인터넷의 발달로 가짜 댓글을 만드는 인공지능들이 나타났다. 가짜 댓글들은 악영향을 끼칠 우려가 있기에, 만약의 경우 사용하기 위한 인공지능에 대항 할 수 있는 시스템을 만들기 위해 이 프로젝트를 기획했다.

#### Main idea: GAN을 사용해서 가짜 댓글을 판별하는 판별기를 만들자!
![image](https://github.com/PG-RDC/TeamProject/assets/130644995/960762a3-7d18-4b8e-9a16-c9901aa0a8d1)

## 결론
Generator의 경우 gpt2를 사용했는데 더 좋은 성능의 Generator를 사용한다면 Discriminator 또한 성능이 올라 갈 것이라고 생각합니다.

#### 다음 코드에 사용하실 경로를 넣어주면 학습이 가능합니다.
train 부분의 save 부분
```python
if (epoch + 1) % 10 == 0:
  torch.save(generator, '/change_your_dir/generator.pt')
  torch.save(discriminator, '/change_your_dir/discriminator.pt')
```
train 부분의 data 설정 부분
```python
data = list(pd.read_csv('your_data').dropna(axis=0, how='any')) #list 형식의 자연어 data
```
Discriminator.ipynb의 세번 째 셀
```python
discriminator = torch.load('/your_dir/discriminator.pt')
```
