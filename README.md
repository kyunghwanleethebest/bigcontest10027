# Big Contest 퓨쳐스리그 (Team 10027) 

##### by 이경환, 김진영, 변영목, 홍기봉



## 분석 환경 및 사용 Packages

### 1. 분석 환경

- OS: Windows  & MacOS & Linux-Ubuntu / RAM: 16GB

- Python == 3.7x version

- Pycharmproject / Jupyter Notebook 

  

### 2. 사용 주요 packages

- beautifulsoup4==4.9.1

- bs4==0.0.1

- joblib==0.16.0

- Keras==2.4.3

- lightgbm==3.0.0

- numpy==1.19.2

- pandas==1.1.2

- selenium==3.141.0

- scikit-learn==0.23.2

- tensorflow==2.3.0

  



## 실행 방법

0. (preprocess.py) 를 실행하여 raw_data를 나중에 사용할 Input으로 가공해준다. (여러 변수 추가 및 2020-07-21~ 2020-09-27의 크롤링 데이터까지 더해준다. - 이미 해놨습니다. )
1. train.py를 돌려준다.(1차 rnn model과 2차 lightgbm model이 다 생성되고, MinMax 및 정규화 모델까지 저장됩니다. )
2. predict.py를 돌려준다. (result폴더에 prediction.csv가 생성됩니다! )
3. 연속 3번을 돌리고 Average 값을 내줬습니다.



** 가상환경설치 한 뒤, requirements.txt에 있는 pip들을 설치해야 합니다. (pip install -r requirements.txt를 치시면 됩니다!)

  #### ※ 혹시라도 가상환경(Virtual environment) 생성을 모른다면?

  ```bash
 #(리눅스 기준)
 # 1 코드를 실행 할 디렉토리에 들어가서 venv라는 이름의 가상환경을 생성한다.
  python3 -m venv venv

  # 2 가상환경을 실행시켜준다.
  (디렉토리에 들어갔다는 가정) source bin/activate

  # 3 가상환경 실행 후, pip를 설치해준다.
  pip3 -r install requirements.txt

  # ** 가상환경을 끄는 방법도 있다.
  source deactivate

  ```



<img src="./image/전처리.PNG">

<img src="./image/모델1.PNG">

<img src="./image/모델2.PNG">



** 7월 19일 이후에 트레이드 한 선수 혹은 이후에 팀에 입단 한 외국인용병에 대한 인적사항은 따로 기입해줬습니다. 

2020   99999   팔카   SS
2020   99998   러셀   WO
2020   99997   화이트   SK

2020   63950  장현식   HT
2020   64984  김태진   HT
2020   65643 문경찬   NC
2020   65639   박정수   NC
2020   63634  이홍구   KT
2020   60558   오태곤   SK