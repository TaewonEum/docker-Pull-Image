# docker_Pull

- ML/DL 환경이 구축된 파이썬 기반 이미지 Pull

- reference: https://hub.docker.com/r/teddylee777/deepko

 ![image](https://github.com/TaewonEum/docker-Pull-Image/assets/104436260/93423d08-dab0-4691-9d70-7fcc90efa92e)

teddylee777/deepko:2023-01 이미지 Pull

# 도커 컨테이너 실행

- docker run -it --name 컨테이너명 이미지명 /bin/bash
- 터미널에 python 입력
- import torch 후 사진과같이 진행
  
![image](https://github.com/TaewonEum/docker-Pull-Image/assets/104436260/7c95903e-c4e5-4669-b05e-9b3a2faedc4e)

- cuda available 사용 불가->GPU 사용 불가

![image](https://github.com/TaewonEum/docker-Pull-Image/assets/104436260/199c774e-aae5-4e57-8f0b-8bc728b3f3b3)

# Jupyter lab 연동

- docker run -it --name test3 -p 8881:8881 teddylee777/deepko:2023-01

- 컨테이너 환경 내: jupyter lab --ip=0.0.0.0 --port=8881 --no-browser --allow-root

![image](https://github.com/TaewonEum/docker-Pull-Image/assets/104436260/8227a82c-0988-41d0-ae2e-8d1b245ba7ea)

- cmd창에 주소가 나오면 웹 브라우저에 해당 주소와 제공받은 토큰 입력하여 log in

![image](https://github.com/TaewonEum/docker-Pull-Image/assets/104436260/ab7ca88b-d682-4eda-bf64-0ce16839e078)

- 해당 주피터랩에서 해당 이미지 환경 사용 가능

# 이미지 (GPU 연동하여 ML/DL 수행)

- tar 파일로 저장
- 내 서버에 Docker image load
- 이후 GPU 서버와 연동하여 수행해보기
