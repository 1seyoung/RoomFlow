# RoomFlow


### 프로젝트 개요
사용자가 입력한 방 도면(문/창문 정보 포함)과 원하는 무드를 기반으로 AI 가 추천한 가구들을
배치해주는 AI 기반 인테리어 추천 시스템

### 전체 시스템 구조
```
RoomFlow/
  ├── web/        ← 프론트엔드 
  ├── server/     ← Spring Boot 
  └── ai-agent/   ← FastAPI + LangChain 
  └── .env
  └── docker-compose.yml
```

#### web

**목적**
사용자가 방 도면을 쉽게 입력하고
AI + 서버가 계산한 가구 배치 결과를 시각적으로 확인할 수 있는 UI 제공


#### server

**목적**
가구 좌표 배치 , 가구 정보 조회

#### ai-agent
 
**목적**
무드 문장 -> 추천 가구 목록
무드와 유사한 가구 검색

```
git clone <RoomFlow>
git submodule update --init --recursive
```
