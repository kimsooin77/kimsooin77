# 김수인 | Web Developer

React·Next.js와 Node.js 기반으로 사용자 기능부터 API·데이터 처리까지  
서비스 흐름 전반을 개발해 온 4년차 웹 개발자입니다.

실시간 상태 동기화, 인증·세션, 외부 시스템 연계처럼  
운영 환경에서 발생하는 복잡한 상태와 예외 흐름을 구조화하는 데 강점이 있습니다.

최근에는 Java와 Spring Boot를 활용해  
데이터 동기화와 외부 시스템 연계 영역까지 개발 범위를 넓히고 있습니다.

[GitHub](https://github.com/kimsooin77) · [Velog](https://velog.io/@ssooo_kk_77/posts)

---

## Featured Project

### Employee Lifecycle Sync

HR 직원 정보를 내부 DB와 동기화하고,  
입사·정보 변경·퇴사에 따른 그룹웨어 계정 작업과 외부 연계 실패 이력을 관리하는 시스템입니다.

**주요 구현**

- 직원 데이터 처리와 외부 시스템 호출을 분리해 외부 장애 영향 최소화
- 외부 호출 실패 자동 재처리 및 중단 작업 복구
- 동일 요청의 중복 반영 방지
- 10,000건 반복 동기화의 직원 조회 구조 개선
- GitHub Actions와 AWS를 이용한 자동 배포

**성능 개선**

| 처리 데이터 | 개선 전 | 개선 후 |
|---|---:|---:|
| 10,000건 변경 없음 | 27.17초 | 18.33초 |
| 1,000건 변경 + 9,000건 변경 없음 | 29.77초 | 21.99초 |

**Tech**

`Java 21` `Spring Boot` `PostgreSQL` `React` `TypeScript` `Docker` `AWS`

[Repository](https://github.com/kimsooin77/Sync) · [Live Demo](https://d2cpqpf162fsls.cloudfront.net)

---

## Experience Highlights

### 인증 상태 충돌 문제 해결

로그아웃 이후 이전 요청의 응답이 뒤늦게 도착하면서  
삭제한 인증 정보가 다시 저장되는 문제를 추적했습니다.

오래된 응답의 상태 반영을 차단하고 중복 인증 갱신을 방지해  
로그아웃 이후 인증 상태가 다시 생성되지 않도록 수정했습니다.

### 대시보드 장애 범위 분리

여러 위젯을 동시에 제공하는 대시보드에서  
한 위젯의 응답 지연이 전체 화면에 영향을 주는 문제를 개선했습니다.

15개 위젯의 로딩·오류 상태를 개별 관리하고,  
지연된 위젯만 다시 요청할 수 있도록 처리 범위를 분리했습니다.

### 오프라인 요청 복구

PWA 환경에서 네트워크가 끊겨도 사용자가 입력한 내용을 잃지 않도록  
등록·수정 요청과 첨부파일을 IndexedDB에 저장했습니다.

온라인 복귀 시 저장된 요청을 순서대로 다시 전송하도록 구현했습니다.

---

## Tech

| | |
|---|---|
| **Frontend** | React · Next.js · Vue · TypeScript · React Native |
| **Backend** | Node.js · Express · Java · Spring Boot |
| **Database** | PostgreSQL · Oracle · Redis |
| **Infra** | Docker · AWS · GitHub Actions |
| **Tools** | Git · GitHub · Figma |

---

## Writing

개발하면서 해결한 문제와 새롭게 학습한 내용을 기록하고 있습니다.

- Next.js에서 PWA로 오프라인 입력 데이터를 저장하고 재전송하기
- OpenLayers Overlay와 iframe 레이어 문제
- GraphRAG, Knowledge Graph, Ontology의 차이

[Velog 전체 글 보기 →](https://velog.io/@ssooo_kk_77/posts)
