# etfholdings

ETF·펀드 정보 사이트(etfholdings.co.kr)를 만들려고 IEX Cloud API(미국 주식·ETF 시세 API)를 연동하던 백엔드 코드입니다. (2021-02)

> 원래 [dnd-project](https://github.com/kalraid/dnd-project)(던전앤파이터 도구 모음) 안의 `fund` 패키지로 시작했습니다. 게임과 상관없는 기능이라 2026-11-10에 이 저장소로 분리했습니다.

## 상태

초기 뼈대만 있습니다.

- `fund/etc/api/EtcApi.java`: IEX Cloud 엔드포인트 목록(주석)과 시세 조회 메서드 자리. 실제 호출은 구현 전입니다.
- `fund/etc/controller`, `service`, `vo`: 빈 클래스입니다.
- `application.yml`: IEX Cloud 운영·샌드박스 URL. `***REMOVED***` 자리에 본인 토큰을 넣어야 합니다.

패키지 이름(`com.dnd.project.fund`)은 원래 프로젝트의 것을 그대로 두었습니다. 단독으로 빌드하려면 Spring Boot 프로젝트 설정(Gradle)과 `CommonApiService` 같은 공통 클래스가 따로 필요합니다.

## 관련 저장소

- [dnd-project](https://github.com/kalraid/dnd-project): 이 코드가 원래 있던 저장소
- [chatserver](https://github.com/kalraid/chatserver): etfholdings.co.kr에 붙이려던 채팅 서버
