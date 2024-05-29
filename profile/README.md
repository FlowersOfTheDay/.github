# Flwers Of The Day

## Target

### 타겟 사용자
수목원에 꽃을 보러온 사람들

### 문제점
수목원에 왔으나 무슨 꽃을 봐야할 지 모르는 경우, 수목원에 있는 상투적인 꽃 설명에 지루함을 느낌.

### 기대점
즐길 수 있는 컨텐츠 요소를 제공함으로써 수목원을 오게 할 목적을 부여하고 수목원 활성화 및 지속성 문제 해결

자신에게 어울리는 꽃을 추천하여 수목원을 방문한 것이 단순히 꽃을 보고 분위기를 즐기는 것을 넘어 자신에 대해 알아가는 의미있는 경험 제공

## Value
### Core idea
꽃을 추천해주는 알고리즘 혹은 인공지능 챗봇을 만들어보자

### Idea’s main feature
사용자가 자신의 상황, 기분에 맞는 단어 선택 -> 현재 상황에 어울리는 꽃 반환

### Technical challenge
LLM을 이용하여 사람의 상태를 알아내는 것

## Teams

### 팀 이름
FOTD(Flowers Of The Day)

### 팀 리더
박시원

### 역할

#### 박시원 [Github](https://github.com/siwonpada)
- Backend 구성
- 깃허브 설정
- 인프라 구성

#### 서은원 [Github](https://github.com/seunwon)
- 프론트엔드 구현

#### 장서연  [Github](https://github.com/Jangseo5160)
- 기획안 작성
- 프롬프트 엔지니어링

## Result

### Frontend

streamlit으로 구성된 프론트엔드를 구성하였다. 

배포를 위하여, github registry를 사용, github action으로 도커 빌드를 자동화하였습니다. (현재 org의 package에서 docker image를 확인하실 수 있습니다.)


### Backend

http 통신을 위하여 fastapi 라이브러리를, LLM을 사용하기 위해, langchain을, 더해서 database를 사용하기 위해서, prisma python을 사용하였습니다.  

배포를 위하여, github registry를 사용, github action으로 도커 빌드를 자동화하였습니다. (현재 org의 package에서 docker image를 확인하실 수 있습니다.)

### AI (LLM)


### INFRA

GIST moblieX cluster에 배포를 진행하였습니다.
테스트를 위하여 infra repository의 yaml 파일을 사용하였으며, 한번에 배포를 하기 위해서 helm-chart repository의 helm chart를 이용해서 배포를 진행하였습니다. 



