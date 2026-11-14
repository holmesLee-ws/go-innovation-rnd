# 커리큘럼 지도

큰 윤곽만 둔다. 강의 내용은 여기 없다. 튜터가 세션마다 학습자의 수준·목표·실제 상황에 맞춰 조사하고 만든다.

- 기본 순서는 T → R → P → C → G → X다. 선수 관계만 지키면 학습자의 목표에 맞춰 순서를 바꿔도 된다. 정부과제가 급한 학습자는 T1 다음 G1까지 바로 가도 된다(G2부터는 R3 과제 기획이 선수다).
- 목표 수준은 그 모듈을 마쳤다고 볼 최소 수준이다. 수준의 뜻은 [tutor/assessment.md](../tutor/assessment.md)에 있다.
- 「국내 근거」는 그 모듈의 상황을 세울 한국 제도, 「글로벌 비교」는 비교 질문에 쓸 국제 기준·주요국 제도다. `[L1]`·`[G1]` 같은 키는 맨 아래 출처 절을 가리킨다. 조문은 확인 시점의 것이므로 세션에서 말하기 전에 [근거 규칙](../tutor/sources.md)대로 다시 확인한다. 금액·비율·기한 숫자는 일부러 적지 않았다.
- 「경계·연결」은 다른 go-* 영역과 겹치는 부분이다. 그 줄을 넘는 내용은 깊게 다루지 않는다.
- 겹치는 말의 구분: **기술료** — C4는 민간 계약에서 협상하는 기술료, G4는 정부 R&D 협약에 따른 기술료. **성과 측정** — R7은 회사가 자기 포트폴리오를 판단하는 지표, G5는 정부 평가·성과관리 제도. **계약** — R4는 민간 공동·위탁연구 계약, G2는 정부 협약.
- 모듈 id는 진도 기록의 키다. 바꾸면 `learner/state.json`이 깨지므로, 고칠 때는 새 id를 만든다.
- `node tools/check.mjs`로 형식·선수 관계·출처 키를 검사한다(리포 관리자용, 학습자에게는 필요 없다).

## T · 기술경영의 기초

### T1 · 혁신과 R&D는 무엇이 다른가
- 선수: 없음
- 핵심 질문: 우리 회사가 하는 일 중 어디까지가 R&D이고, 그 구분이 왜 돈과 권리를 바꾸는가?
- 목표: Apply — 처음 보는 활동을 혁신·R&D·일상적 개선으로 판정하고, 그 판단 기준을 말한다.
- 만들어 볼 것: 우리 회사 활동 다섯 개를 R&D·혁신·운영으로 나누고 국내 정의(혁신법·조특법 시행령)와 대조한 표
- 국내 근거: 국가연구개발혁신법 제2조(정의) — 국가연구개발사업·연구개발성과 [L1], 조세특례제한법 시행령 제9조(연구 및 인력개발비에 대한 세액공제)·별표 6 — 연구개발의 범위 [L10]
- 글로벌 비교: Frascati Manual 2015의 R&D 정의와 다섯 기준(¶2.5·¶2.7) [G6], Oslo Manual 2018의 혁신 정의(¶1.25) [G7]
- 경계·연결: 어떤 비용이 실제로 세액공제를 받는지의 세무 판단은 go-tax. 여기서는 정의의 구조만

### T2 · 기술의 성숙도와 수명주기
- 선수: T1
- 핵심 질문: 이 기술은 성숙도와 S곡선에서 지금 어디쯤 와 있고, 다음 단계로 가려면 무엇을 증명해야 하는가?
- 목표: Apply — 기술 하나의 TRL을 증거와 함께 판정하고, 다음 단계에 필요한 증거를 정한다.
- 만들어 볼 것: 내 기술(가린 요지) 하나의 TRL 판정 기록 — 정부 R&D 연구개발계획서에 시작·목표 수준을 적는다는 가정
- 국내 근거: 직접 규정 없음 — 실무 연결: 정부 R&D 연구개발계획서 표준 서식(국가연구개발혁신법 시행규칙 별지 제1호서식)에 쓰는 목표·성숙 단계, 항목 이름은 세션에서 서식으로 확인 [L3]
- 글로벌 비교: NASA NPR 7123.1D 부록 E의 TRL 정의 [G8], Horizon 2020 General Annex G의 TRL [G9]

### T3 · 기술 로드맵
- 선수: T2
- 핵심 질문: 시장이 원하는 것과 우리가 가진 기술 사이의 빈칸을 언제 무엇으로 메울 것인가?
- 목표: Apply — 시장·제품·기술 층을 시간축으로 잇는 로드맵을 그리고, 빈칸에서 R&D 과제 후보를 뽑는다.
- 만들어 볼 것: 내 사업의 3층 로드맵 초안과, 다음 정부 R&D 수요조사에 낼 과제 후보 목록
- 국내 근거: 직접 규정 없음 — 실무 연결: 중앙행정기관의 연구개발 수요조사·예고(국가연구개발혁신법 제9조(예고 및 공모 등))에 낼 과제 후보를 로드맵에서 뽑는다 [L1]
- 글로벌 비교: Phaal·Farrukh·Probert(2004)의 기술 로드맵 틀 [G12]
- 경계·연결: 제품 로드맵·우선순위는 go-product, 전사 전략·사업 포트폴리오는 go-strategy. 여기서는 기술 층과 R&D 과제의 연결만

### T4 · 혁신경영시스템
- 선수: T3
- 핵심 질문: 혁신을 운에 맡기지 않고 조직의 관리 체계로 만들려면 무엇을 갖춰야 하고, 인증이 필요한가?
- 목표: Evaluate — 요구사항 표준과 가이던스의 차이를 알고, 우리 조직에 인증·자율 적용·보류 중 무엇이 맞는지 근거와 함께 정한다.
- 만들어 볼 것: 우리 회사 혁신 활동의 간이 진단과 도입 권고 한 장 — KS A ISO 56001 인증을 받을지, KS A ISO 56002를 자율 지침으로만 쓸지의 판단 포함
- 국내 근거: KS A ISO 56001(혁신경영시스템 — 요구사항)·KS A ISO 56002(혁신경영 – 혁신경영시스템 - 가이던스) [L19]
- 글로벌 비교: ISO 56001:2024 [G1], ISO 56002:2019(개정 진행 중) [G2]

## R · R&D 포트폴리오와 과제 관리

### R1 · R&D 포트폴리오 구성
- 선수: T2
- 핵심 질문: 과제 하나하나는 좋아 보이는데, 모아 놓으면 왜 회사가 원하는 곳에 가지 못하는가?
- 목표: Evaluate — 과제들을 목적 유형·위험·기대가치·전략 적합성으로 나눠 균형을 판단하고 넣고 뺄 과제를 정한다.
- 만들어 볼 것: 지금(또는 가상의) 과제 대여섯 개의 포트폴리오 표와 위험·가치 지도
- 국내 근거: 직접 규정 없음 — 실무 연결: 정부 R&D를 포트폴리오의 한 자금원으로 넣을 때 따라오는 단계 구조와 연구개발기간(국가연구개발혁신법 제12조(연구개발과제의 수행 및 관리)) [L1]
- 글로벌 비교: ISO 56008:2024의 혁신 포트폴리오 측정 [G5], ISO 56002:2019 [G2]
- 경계·연결: 전사 사업 포트폴리오는 go-strategy, 투자 결정(NPV·IRR)은 go-finance. 여기서는 R&D 과제 묶음만

### R2 · 스테이지게이트와 중단 결정
- 선수: R1
- 핵심 질문: 돈을 이미 많이 쓴 과제를 멈출지 계속할지 누가 무엇을 보고 정하는가?
- 목표: Evaluate — 게이트 기준을 미리 세우고, 주어진 중간 결과로 계속·수정·중단을 근거와 함께 결정한다.
- 만들어 볼 것: 과제 하나의 단계·게이트 기준표와, 2단계 목표 미달 시나리오의 판정 기록 — 정부 과제의 단계평가·특별평가와 비교
- 국내 근거: 국가연구개발혁신법 제12조(연구개발과제의 수행 및 관리) — 단계별 수행·단계평가, 제15조(특별평가를 통한 연구개발과제의 변경 및 중단) [L1]
- 글로벌 비교: Cooper(1990)의 Stage-Gate [G10], 미국 SBIR의 Phase I·II·III 구조 [G27]
- 경계·연결: 과제의 일정·원가·위험 관리 기법(WBS·EVM)은 go-project-management. 여기서는 R&D 고유의 불확실성과 중단 결정만

### R3 · 과제 기획: 목표·지표·예산
- 선수: R2
- 핵심 질문: 평가위원이 「그래서 무엇이 되면 성공인가」를 묻는다면 무엇으로 답하는가?
- 목표: Apply — 과제의 최종 목표를 검증 가능한 정량 지표로 쓰고, 그 목표에 맞게 비용을 직접비·간접비로 구성한다.
- 만들어 볼 것: 과제 하나의 목표·지표·비목 요지 한 장(연구개발계획서 표준 서식 항목에 맞춰)
- 국내 근거: 국가연구개발혁신법 시행규칙 제2조(서식)·별지 제1호서식 — 연구개발계획서 [L3], 국가연구개발혁신법 제13조(연구개발비의 지급 및 사용 등)제3항 — 직접비·간접비 [L1]
- 글로벌 비교: 미국 2 CFR 200.403(비용 인정 요건) [G25]

### R4 · 개방형 혁신과 공동·위탁연구 계약
- 선수: R2, P1
- 핵심 질문: 기술을 직접 만들까, 같이 만들까, 사 올까 — 고른 뒤 성과는 누구 것이 되는가?
- 목표: Evaluate — 내부 개발·공동연구·위탁·기술도입 중 하나를 고르고, 계약의 성과 귀속·실시권·비용·공개 제한 조항을 판단한다.
- 만들어 볼 것: 대학(또는 대기업)과의 민간 공동연구 조건표 — 특허법의 공유 규정을 그대로 두면 생길 일을 함께 적기
- 국내 근거: 특허법 제33조(특허를 받을 수 있는 자)제2항 — 공동발명의 공유, 제99조(특허권의 이전 및 공유 등) [L9]
- 글로벌 비교: Chesbrough(2003)의 개방형 혁신 [G11], ISO 56003:2019(혁신 파트너십) [G3]
- 경계·연결: 계약 해석·손해배상 같은 계약 법리 일반은 go-compliance-and-legal. 정부 협약은 G2

### R5 · 연구조직과 기업부설연구소
- 선수: T1
- 핵심 질문: 연구소 인정은 왜 받고, 무엇을 소홀히 하면 잃는가?
- 목표: Apply — 연구소·연구개발전담부서 인정 기준과 준수사항을 우리 조직에 대입해 인정 유지 위험을 진단한다.
- 만들어 볼 것: 우리(또는 가상의) 연구소의 인정 유지 점검표 — 인력 겸직, 변경신고, 실적 제출
- 국내 근거: 기업부설연구소등의 연구개발 지원에 관한 법률 제7조(기업부설연구소등의 인정) — 변경신고는 제4항, 제8조(기업부설연구소등의 인정취소), 제9조(기업부설연구소등의 준수사항), 시행령 제6조(기업부설연구소등의 인정기준) [L11]
- 글로벌 비교: 조직 인정 없이 활동 요건으로 연구를 판단하는 미국 IRC §41(d)의 qualified research [G14]

### R6 · R&D 세액공제의 구조
- 선수: R5
- 핵심 질문: 같은 연구비인데 왜 어떤 것은 공제가 크고 어떤 것은 안 되는가?
- 목표: Apply — 비용 항목을 연구·인력개발비 여부와 일반·신성장·원천기술·국가전략기술 갈래로 숫자 없이 분류하고, 연구소 인정과의 연결을 짚는다.
- 만들어 볼 것: 우리 비용 항목 열 개를 공제 구조로 분류한 표 — 실제 적용은 세무사 확인으로 표시
- 국내 근거: 조세특례제한법 제10조(연구·인력개발비에 대한 세액공제), 시행령 제9조(연구 및 인력개발비에 대한 세액공제)·별표 6·별표 7·별표 7의2 [L10]
- 글로벌 비교: 미국 IRC §41 연구 세액공제와 §174A 국내 연구비 당기 공제 [G14], 영국 merged R&D 세액공제·ERIS [G18]
- 경계·연결: 공제율·한도·최저한세·세무조정·사후관리는 go-tax. 여기서는 구조만, 숫자 없이

### R7 · R&D 성과 측정
- 선수: R3
- 핵심 질문: 특허 건수가 늘었는데 왜 사업은 그대로인가?
- 목표: Evaluate — 투입·활동·산출·성과 지표를 구분하고, 포트폴리오 결정에 쓸 지표와 버릴 지표를 근거와 함께 고른다.
- 만들어 볼 것: 우리 R&D 성과 지표 세트 초안과 버릴 지표 목록 — 정부 평가 지표와 겹치는 것 표시
- 국내 근거: 국가연구개발사업 등의 성과평가 및 성과관리에 관한 법률 제7조(연구개발사업에 대한 자체평가 등)·제16조(연구성과 관리·활용 계획의 마련) — 정부 평가 체계와의 비교용 [L5]
- 글로벌 비교: ISO 56008:2024 [G5], AUTM Licensing Activity Survey의 사업화 지표 [G29]
- 경계·연결: 전사 성과관리(KPI·BSC)는 go-controllership. 정부 과제 평가 대응은 G5

## P · IP 전략

### P1 · 보호 수단 고르기
- 선수: T1
- 핵심 질문: 이 기술은 특허로 공개하고 지킬까, 비밀로 묻어 둘까, 일부러 공개해 버릴까?
- 목표: Evaluate — 특허·영업비밀·방어적 공개 중 기술 요소마다 맞는 수단을 역설계 가능성·수명·집행 가능성으로 고른다.
- 만들어 볼 것: 우리 기술 요소 서너 개(가린 요지)의 보호 수단 결정표 — 특허요건(신규성·진보성)과 영업비밀 요건(비공지성·경제적 가치·비밀관리)을 칸으로 두고 판정
- 국내 근거: 특허법 제29조(특허요건)·제88조(특허권의 존속기간) [L9], 부정경쟁방지 및 영업비밀보호에 관한 법률 제2조(정의)제2호 — 영업비밀 [L14]
- 글로벌 비교: ISO 56005:2020(IP 관리 가이던스) [G4], 미국 Defend Trade Secrets Act의 영업비밀 정의(18 U.S.C. §1839) [G24]
- 경계·연결: 특허·영업비밀의 법리와 침해 소송은 go-compliance-and-legal. 여기서는 고르는 사업 판단만

### P2 · 특허요건과 출원 타이밍
- 선수: P1
- 핵심 질문: 학회 발표, 투자 IR, 전시회가 잡혀 있다면 특허는 언제 내야 하는가?
- 목표: Apply — 신규성·진보성·공지예외·선출원·국내우선권을 써서 공개 일정과 출원 순서를 정한다.
- 만들어 볼 것: 발표·IR·전시회가 겹친 일정표에서 출원 시점을 정한 결정 기록
- 국내 근거: 특허법 제29조(특허요건) — 신규성·진보성, 제30조(공지 등이 되지 아니한 발명으로 보는 경우) — 공지예외, 제36조(선출원), 제55조(특허출원 등을 기초로 한 우선권 주장) — 국내우선권 [L9]
- 글로벌 비교: 미국 35 U.S.C. §102(b)(1)의 발명자 공개 유예 [G15]

### P3 · 직무발명 제도
- 선수: P1
- 핵심 질문: 연구원이 만든 발명은 언제 회사 것이 되고, 회사는 무엇을 해야 하는가?
- 목표: Apply — 완성 통지·승계 통지·보상 규정·협의 절차의 흐름을 사례에 적용해 빠진 절차와 그 결과를 찾는다.
- 만들어 볼 것: 우리 회사 직무발명 규정 요지 — 통지, 승계 여부 결정, 보상 형태, 규정 작성·변경 협의
- 국내 근거: 발명진흥법 제2조(정의)제2호 — 직무발명, 제10조(직무발명) — 사용자의 통상실시권, 제12조(직무발명 완성사실의 통지), 제13조(직무발명의 권리승계), 제15조(직무발명에 대한 보상), 제17조(직무발명심의위원회의 운영 등), 시행령 제7조(승계 여부의 통지기간) [L8]
- 글로벌 비교: 독일 종업원발명법 §5·§6·§9 [G16], 일본 특허법 제35조(2015년 개정 후 원시귀속 선택) [G17]
- 경계·연결: 보상 분쟁의 법리는 go-compliance-and-legal, 연구 인력의 근로계약·성과급은 go-hr

### P4 · 국제출원 전략
- 선수: P2
- 핵심 질문: 해외 시장이 아직 정해지지 않았을 때 특허는 어떤 경로로 시간을 벌 수 있는가?
- 목표: Evaluate — 파리협약 우선권으로 바로 각국에 내는 경로와 PCT 경로를 시장·비용·시간으로 비교해 고른다.
- 만들어 볼 것: 진출 후보국 두세 곳의 출원 경로 결정표 — 국내 출원일을 기준으로
- 국내 근거: 특허법 제54조(조약에 의한 우선권 주장) [L9]
- 글로벌 비교: 파리협약 제4조 [G21], PCT 국제출원 체계 [G20]
- 경계·연결: 해외 진출 방식과 국가 선정은 go-global-business

### P5 · 선행기술조사·FTO·IP 포트폴리오
- 선수: P2
- 핵심 질문: 우리가 만들려는 제품이 남의 특허를 밟는지, 우리 특허가 비어 있는 곳은 어디인지 어떻게 아는가?
- 목표: Apply — 공개 특허 DB에서 선행기술을 찾아 우리 출원의 위치와 실시 위험을 판단하고 포트폴리오의 빈 곳을 찾는다.
- 만들어 볼 것: 우리 기술 한 가지를 공개 특허 DB(KIPRIS 등)에서 찾은 선행특허 목록과 위험 메모 — 우리가 먼저 실시하고 있었다면 선사용 통상실시권을 주장할 증거가 있는지 포함(최종 판단은 변리사 확인으로 표시)
- 국내 근거: 특허법 제94조(특허권의 효력)·제103조(선사용에 의한 통상실시권) [L9]
- 글로벌 비교: ISO 56005:2020 [G4]
- 경계·연결: 침해 여부의 법적 판단은 변리사와 go-compliance-and-legal

### P6 · 라이선스와 공동소유
- 선수: P5, R4
- 핵심 질문: 같은 특허라도 누구에게 어떤 범위로 허락하느냐에 따라 사업이 어떻게 달라지는가?
- 목표: Evaluate — 전용·통상 실시권, 독점·비독점, 공동소유 조건을 사업 목적에 맞게 골라 조건표로 만든다.
- 만들어 볼 것: 라이선스 조건 요약표(범위·지역·기간·대가 구조·개량발명 처리) — 전용실시권으로 줄지 통상실시권으로 줄지, 공유 특허라면 다른 공유자 동의를 받았는지를 칸으로 둔다
- 국내 근거: 특허법 제99조(특허권의 이전 및 공유 등)·제100조(전용실시권)·제102조(통상실시권) [L9]
- 글로벌 비교: 표준특허의 FRAND 약정(ETSI IPR Policy 6.1) [G22]
- 경계·연결: 해외 라이선스·JV는 go-global-business, 계약 법리는 go-compliance-and-legal

### P7 · 중소기업 기술 보호
- 선수: P1
- 핵심 질문: 거래처 대기업이 도면과 공정 자료를 달라고 하면 무엇을 주고 무엇을 남기는가?
- 목표: Apply — 공동개발·납품 상황에서 기술자료 요구에 대응하는 절차를 정하고 임치·비밀유지계약을 고른다.
- 만들어 볼 것: 거래처의 기술자료 요구 상황 대응 절차 한 장(요구 서면, 비밀유지계약, 임치)
- 국내 근거: 대·중소기업 상생협력 촉진에 관한 법률 제24조의2(기술자료 임치제도)·제25조(준수사항) [L17], 하도급거래 공정화에 관한 법률 제12조의3(기술자료 제공 요구 금지 등) [L18], 중소기업기술 보호 지원에 관한 법률 제9조(임치제도 활용 지원) [L16]
- 글로벌 비교: 넘긴 자료가 영업비밀로 남으려면 「합리적인 비밀유지 조치」가 요건이라는 EU 영업비밀 지침 2016/943 제2조(1)(c) — 비밀유지계약·임치가 왜 그 조치가 되는지 비교 [G23]
- 경계·연결: 유용 분쟁·제재의 법리는 go-compliance-and-legal, 구매·하도급 거래 실무는 go-scm

## C · 기술 사업화

### C1 · 사업화 경로 고르기
- 선수: P1, T3
- 핵심 질문: 좋은 기술이 있을 때 직접 팔까, 남에게 넘길까, 회사를 따로 세울까(공공기술이면 기술지주회사·연구소기업 같은 구조까지)?
- 목표: Evaluate — 자체 사업화·기술이전·창업·합작 중 기술과 조직 상황에 맞는 경로를 근거와 함께 고른다.
- 만들어 볼 것: 기술 하나의 사업화 경로 비교표 — 기술이전법의 기술이전 방식 목록을 기준으로
- 국내 근거: 기술의 이전 및 사업화 촉진에 관한 법률 제2조(정의)제2호 — 기술이전, 제3호 — 사업화 [L7]
- 글로벌 비교: Chesbrough(2003) [G11]
- 경계·연결: 창업·투자 유치는 go-startup-agile, 해외 JV는 go-global-business. 기술을 해외로 넘길 때는 국가핵심기술 수출 승인 대상인지 먼저 본다(산업기술의 유출방지 및 보호에 관한 법률 제11조(국가핵심기술의 수출 등)) [L15] — 깊이는 다루지 않는다

### C2 · 공공기술 이전과 기술이전 전담조직
- 선수: C1
- 핵심 질문: 대학·출연연에 있는 기술은 어떤 경로로 기업에 오고, 그 권리는 처음에 누구 것이었는가?
- 목표: Explain — 공공연구성과의 귀속 원칙, 기술이전 전담조직의 역할, 기업이 기술을 들여올 때 거치는 단계를 설명한다.
- 만들어 볼 것: 대학 기술 도입 상담 전에 준비할 질문 목록
- 국내 근거: 기술의 이전 및 사업화 촉진에 관한 법률 제11조(공공연구기관의 기술이전·사업화 전담조직)·제24조(공공연구개발 성과의 귀속 등) [L7], 국가연구개발혁신법 제16조(연구개발성과의 소유·관리) [L1]
- 글로벌 비교: 미국 Bayh-Dole Act §202 [G13], 연방 연구소 CRADA(15 U.S.C. §3710a) [G30]

### C3 · 기술가치평가가 필요한 순간
- 선수: C1
- 핵심 질문: 기술의 값을 매겨야 하는 결정은 언제 오고, 평가 결과를 어디까지 믿어야 하는가?
- 목표: Explain — 이전·현물출자·담보·투자 같은 결정에서 가치평가가 필요한 이유와 평가 목적에 따라 결과가 달라지는 까닭을 설명한다.
- 만들어 볼 것: 우리 상황에서 평가가 필요한 결정 목록과 평가 의뢰 전 준비물
- 국내 근거: 기술의 이전 및 사업화 촉진에 관한 법률 제2조(정의)제4호 — 기술평가, 제35조(기술평가기관의 지정 등) [L7]
- 글로벌 비교: International Valuation Standards의 IVS 210 무형자산 [G28]
- 경계·연결: 평가 방법론(DCF·로열티 공제법·실물옵션)은 go-valuation. 여기서는 언제·왜 필요한지만

### C4 · 기술료와 라이선스 대가 구조
- 선수: C1, P6
- 핵심 질문: 선급금을 크게 받을까, 매출에 따라 받을까 — 그 선택은 누구에게 위험을 넘기는가?
- 목표: Apply — 선급금·경상기술료·마일스톤 조합을 시나리오로 계산해 협상안을 만든다.
- 만들어 볼 것: 라이선스 대가 시나리오 비교표(예시 값) — 정부 R&D 성과라면 협약 기술료 규정이 어디서 끼어드는지 표시
- 국내 근거: 직접 규정 없음 — 실무 연결: 정부 R&D 성과를 실시계약할 때는 협약 기술료 규정(국가연구개발혁신법 제18조(기술료의 징수 및 사용))이 따라온다 [L1]
- 글로벌 비교: AUTM Licensing Activity Survey의 라이선스 수입 구성 [G29]
- 경계·연결: 라이선스 수익의 회계 처리는 go-accounting, 세무는 go-tax

### C5 · 죽음의 계곡과 사업화 지원 제도
- 선수: C1, T2
- 핵심 질문: 시제품까지는 됐는데 양산까지 가는 돈과 증거는 어디서 오는가?
- 목표: Evaluate — 성숙도 구간별 자금 공백을 진단하고, 그 구간에 맞는 공공 지원 제도를 고른다.
- 만들어 볼 것: 우리 기술의 TRL 구간별 필요 자금과 지원 제도 지도
- 국내 근거: 중소기업 기술혁신 촉진법 제9조(중소기업의 기술혁신 촉진 지원사업) [L13], 산업기술혁신 촉진법 제11조(산업기술개발사업) [L12]
- 글로벌 비교: 미국 SBIR·STTR(15 U.S.C. §638) [G27]
- 경계·연결: 창업 지원사업·투자 유치 단계는 go-startup-agile

## G · 정부 R&D 과제 수행

### G1 · 국가연구개발의 체계와 법령 지도
- 선수: T1
- 핵심 질문: 공고를 낸 곳, 평가하는 곳, 돈을 주는 곳, 성과를 가져가는 곳은 각각 누구인가?
- 목표: Explain — 중앙행정기관·전문기관·연구개발기관·연구자의 역할과, 법·시행령·고시·협약의 층위를 설명한다.
- 만들어 볼 것: 내가 지원할(또는 지원했던) 사업의 관계도 — 누가 공고·평가·협약·정산하는가
- 국내 근거: 과학기술기본법 제11조(국가연구개발사업의 추진) [L6], 국가연구개발혁신법 제2조(정의)·제22조(전문기관의 지정 등) [L1]
- 글로벌 비교: EU Horizon Europe 표준 협약(Model Grant Agreement) [G19]

### G2 · 공모·선정·협약
- 선수: G1, R3
- 핵심 질문: 공고문의 어느 줄이 평가를 가르고, 협약서에 서명하면 무엇을 약속한 것인가?
- 목표: Apply — 공고에서 참여 자격·평가 기준을 짚어 제안 전략을 세우고, 협약서의 권리·의무를 읽는다.
- 만들어 볼 것: 공개된 실제 공고 하나의 요건 점검표와 협약서 표준 서식에서 우리가 지킬 의무 목록
- 국내 근거: 국가연구개발혁신법 제9조(예고 및 공모 등)·제10조(연구개발과제 및 수행 연구개발기관의 선정)·제11조(연구개발과제 협약 등) [L1], 시행령 제9조(연구개발과제 및 연구개발기관의 공모 절차)·제13조(연구개발과제협약의 체결) [L2], 시행규칙 별지 제2호서식 — 국가연구개발사업 협약서 [L3], 범부처 통합연구지원시스템 [L20]
- 글로벌 비교: Horizon Europe Model Grant Agreement [G19]

### G3 · 연구개발비 사용·변경·정산
- 선수: G2
- 핵심 질문: 이 지출은 어느 비목이고, 미리 승인받아야 하며, 정산에서 인정되는가?
- 목표: Apply — 지출 사례를 비목에 분류하고, 사전 승인이 필요한 변경인지와 정산에서 불인정될 위험을 판단한다.
- 만들어 볼 것: 지출 열 건의 비목 분류와 위험 표시(최신 사용 기준 고시로 대조)
- 국내 근거: 국가연구개발혁신법 제13조(연구개발비의 지급 및 사용 등) [L1], 시행령 제20조(연구개발비의 사용용도 등)·제26조(연구개발비의 정산 등) [L2], 국가연구개발사업 연구개발비 사용 기준 제5조(직접비와 간접비의 사용용도), 제3장(제73조~) — 사용계획 변경의 사전 승인 [L4], 범부처 통합연구지원시스템 [L20]
- 글로벌 비교: 미국 2 CFR 200 Subpart E(비용 원칙, §200.403) [G25]
- 경계·연결: 정부보조금·개발비의 회계 처리는 go-accounting, 연구비 부정 방지 통제 설계는 go-control

### G4 · 성과 소유·활용과 협약상 기술료
- 선수: G2, P3
- 핵심 질문: 정부 돈으로 만든 특허는 누구 것이고, 그 대가로 무엇을 해야 하는가?
- 목표: Evaluate — 공동과제 성과의 소유자를 정하고, 활용·공개·기술료 의무와 공동기관 간 배분을 판단한다.
- 만들어 볼 것: 공동과제의 성과 귀속·활용 계획 한 장 — 직무발명 승계(P3)와 이어서
- 국내 근거: 국가연구개발혁신법 제16조(연구개발성과의 소유·관리)·제17조(연구개발성과의 활용)·제18조(기술료의 징수 및 사용) [L1], 시행령 제32조(연구개발성과의 소유), 제38조~제41조 — 정부납부기술료와 기술료의 사용 [L2]
- 글로벌 비교: 미국 Bayh-Dole Act §202·§203 [G13], Horizon Europe Model Grant Agreement 부속서 5 [G19]

### G5 · 평가와 성과관리
- 선수: G2
- 핵심 질문: 단계평가에서 떨어지는 과제는 무엇이 다르고, 과제가 끝난 뒤에도 남는 의무는 무엇인가?
- 목표: Apply — 단계·최종 평가 기준을 과제에 적용해 대비하고, 성과 등록·추적 의무를 정리한다.
- 만들어 볼 것: 단계평가 대비 자기점검표와 종료 뒤 성과관리 일정
- 국내 근거: 국가연구개발혁신법 제14조(연구개발과제의 평가 등) [L1], 시행령 제33조(연구개발성과의 관리) [L2], 국가연구개발사업 등의 성과평가 및 성과관리에 관한 법률 제16조(연구성과 관리·활용 계획의 마련)·제20조(연구성과 데이터베이스 구축 등) [L5]
- 글로벌 비교: ISO 56008:2024 [G5]
- 경계·연결: 회사 안의 성과 지표 설계는 R7, 전사 KPI는 go-controllership

### G6 · 연구윤리·부정행위·제재·연구보안
- 선수: G3
- 핵심 질문: 어떤 실수가 제재로 이어지고, 무엇을 기록해 두면 나를 지킬 수 있는가?
- 목표: Apply — 사례에서 부정행위·제재 사유를 찾아내고, 예방 장치(연구노트·증빙·보안과제 관리)를 정한다.
- 만들어 볼 것: 우리 과제의 연구노트·보안·증빙 점검표 — 연구데이터 관리는 혁신법·시행령 본문에 별도 조문이 없으므로(확인 2026-11-14) 협약·소관 부처 지침에서 찾는 칸을 둔다
- 국내 근거: 국가연구개발혁신법 제21조(국가연구개발사업 등의 보안)·제31조(국가연구개발사업 관련 부정행위의 금지)·제32조(부정행위 등에 대한 제재처분)·제35조(연구개발과제의 성실 수행)제2항 — 연구 수행 과정의 기록 [L1], 시행령 제45조(보안과제·민감과제의 분류)·제59조(부정행위 등에 대한 제재처분)·제65조(연구수행과정 및 연구개발성과의 작성·기록·관리 등) — 연구노트 [L2]
- 글로벌 비교: 미국 42 CFR Part 93의 연구부정 정의(§93.234) [G26]
- 경계·연결: 연구보안의 정보보호 기술 통제는 go-security, 국가핵심기술 지정·보호는 산업기술의 유출방지 및 보호에 관한 법률 제9조(국가핵심기술의 지정·변경 및 해제 등) [L15] — 이름만

## X · 졸업 프로젝트

### X1 · 정부 R&D 과제 제안서 골격과 R&D 포트폴리오 표
- 선수: R1, R3, P3, C1, G3, G4
- 핵심 질문: 배운 것을 내 실제 상황의 과제 하나와 포트폴리오 전체에 맞물리게 쓸 수 있는가?
- 목표: Develop — 제안서 골격과 포트폴리오 표를 서로 맞물리게 만들고, 국내 제도 근거와 검토 질문에 산출물로 답한다.
- 만들어 볼 것: ① 정부 R&D 과제 제안서 골격(필요성, 목표와 정량 지표, TRL 시작·목표, 추진 체계, 단계별 계획과 중단 기준, 비목 구성 요지, 성과 활용과 IP 계획) ② R&D 포트폴리오 표(과제마다 목적 유형·TRL·기대가치 또는 전략 적합성·위험·자원·다음 게이트·IP 보호 수단) — 판정 기준은 [tutor/assessment.md](../tutor/assessment.md)의 졸업 판정
- 국내 근거: 국가연구개발혁신법 시행규칙 별지 제1호서식 — 연구개발계획서 [L3], 국가연구개발혁신법 제16조(연구개발성과의 소유·관리) [L1], 발명진흥법 제13조(직무발명의 권리승계) [L8], 국가연구개발사업 연구개발비 사용 기준 제5조(직접비와 간접비의 사용용도) [L4]
- 글로벌 비교: 미국 SBIR의 단계 구조 [G27], Horizon Europe Model Grant Agreement [G19]

## 이 지도에 넣지 않은 것

특허 청구항 작성·심판·소송, 상표·디자인·저작권, 표준화 기구 활동 전략, 연구실 안전, 산업정책의 거시경제는 깊게 다루지 않는다. 학습자가 원하면 튜터가 선택 모듈로 더한다. 선택 모듈 id는 `E`로 시작하고 `learner/state.json`에만 둔다.

## 출처

법령은 국가법령정보센터(law.go.kr)가 2026-11-14 21:00까지 점검 중이어서 국회 법률정보시스템 현행본(시행일 기준 화면)으로 확인했다. 국회 화면은 공포됐지만 아직 시행되지 않은 개정 문구를 같은 조에 함께 보여 줄 수 있어, 「시행 예정」을 따로 적었다. 원문이 유료인 ISO 표준은 발행처 페이지로 이름·판·연도·상태만 확인했다. 부처 명칭은 2025-10-01부터 특허청장 → 지식재산처장, 산업통상자원부장관 → 산업통상부장관으로 법령 본문에 반영돼 있다.

### 국내

- [L1] 국가연구개발혁신법 — 현행 법률 제21857호(시행 2026-10-02). 시행 예정: 법률 제21913호(시행 2027-03-16, 제2·9·10·18·22·32조 개정, 제36조의2 신설). 제32조 제재 상한은 현행·예정 문구를 law.go.kr 연혁으로 다시 가려야 한다(숫자는 이 지도에 쓰지 않음). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2020060900000043&contSid=0027&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L2] 국가연구개발혁신법 시행령 — 대통령령 제36525호(시행 2026-09-11, 일부 규정 시행 2027-01-01 — 기술료 제38~41조 포함). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2021010800000032&contSid=0054&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L3] 국가연구개발혁신법 시행규칙 — 과학기술정보통신부령 제173호(시행 2026-08-20). 별지 제1호서식 연구개발계획서, 제2호서식 협약서. https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2021010900000002&contSid=0013&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L4] 국가연구개발사업 연구개발비 사용 기준 — 과학기술정보통신부고시 제2026-13호(시행 2026-03-11) 원문 확인. 그 뒤 2026-05-06 일부개정(연구혁신비 신설, 간접비 사용용도 개편 — 고시 번호는 원문 미확인)이 있다. 세션에서는 최신 개정부터 확인한다. https://environment.pusan.ac.kr/bbs/environment/9628/981478/download.do (제2026-13호 law.go.kr 출력본, 확인 2026-11-14), 개정고시안 https://www.konkuk.ac.kr/bbs/research/4214/1213733/download.do (확인 2026-11-14)
- [L5] 국가연구개발사업 등의 성과평가 및 성과관리에 관한 법률 — 법률 제19782호(시행 2023-10-31). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2005123000000002&contSid=0036&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L6] 과학기술기본법 — 법률 제21493호(시행 2026-07-01). 시행 예정: 법률 제21861호(시행 2027-02-12, 대상 조 미확인). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2001011600000001&contSid=0092&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L7] 기술의 이전 및 사업화 촉진에 관한 법률 — 현행 법률 제21065호(시행 2025-10-01). 시행 예정: 법률 제21681호(시행 2026-11-27, 제2·11·16·19·21조의3~5·24·35조의2·35조의7 개정). 시행령 대통령령 제36221호. https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2000012800000009&contSid=0050&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L8] 발명진흥법 — 법률 제21065호(시행 2025-10-01), 시행령 대통령령 제36563호(시행 2026-08-07). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=1994032400000003&contSid=0107&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14), 시행령 https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=1994090900000002&contSid=0224&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L9] 특허법 — 법률 제21134호(시행 2025-11-11). 시행 예정: 법률 제21955호(시행 2027-03-16, 제81조의3·제87조). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=1961123100000013&contSid=0157&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L10] 조세특례제한법 제10조·시행령 제9조 — 법률 제21467호(시행 2026-09-18), 시행령 대통령령 제36587호(시행 2026-09-18). 시행령 제9조에 2027-01-01 시행 예정 개정 표지가 있다. https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=1965122000000003&contSid=0828&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14), 시행령 https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=1974071800000003&contSid=0887&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L11] 기업부설연구소등의 연구개발 지원에 관한 법률 — 법률 제20727호로 2025-01-31 제정, 2026-02-01 시행(현행 법률 제21309호). 기초연구진흥법 제14조의2~제14조의6은 같은 날 삭제됐다. 시행령 대통령령 제36055호, 시행규칙 과학기술정보통신부령 제163호. 인정 업무는 한국산업기술진흥협회에 위탁(시행령 제16조). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2025012400000079&contSid=0004&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14), 시행령 https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2026012700000016&contSid=0001&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L12] 산업기술혁신 촉진법 — 법률 제21467호(시행 2026-09-18). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=1994122200000007&contSid=0119&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L13] 중소기업 기술혁신 촉진법 — 법률 제21289호(시행 2026-07-01). 시행 예정: 법률 제22039호(시행 2027-03-30, 대상 조 미확인). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2001052400000001&contSid=0086&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L14] 부정경쟁방지 및 영업비밀보호에 관한 법률 — 법률 제20963호(시행 2026-05-28). 시행 예정: 법률 제21952호(시행 2027-03-16, 제2조·제18조). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=1961123000000009&contSid=0064&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L15] 산업기술의 유출방지 및 보호에 관한 법률 — 법률 제21154호(시행 2026-06-03). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2006102700000002&contSid=0040&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L16] 중소기업기술 보호 지원에 관한 법률 — 법률 제21291호(시행 2026-07-01). 시행 예정: 법률 제22041호(시행 2027-03-30, 대상 조 미확인). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2014052800000003&contSid=0016&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14)
- [L17] 대·중소기업 상생협력 촉진에 관한 법률 — 법률 제22033호(시행 2026-09-29). 시행 예정: 법률 제21191호(시행 2026-12-03, 제25조 등 개정), 법률 제21377호(시행 2028-02-20). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=2006030300000005&contSid=0110&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14 — 페이지가 커서 WebFetch 요약이 조문을 놓칠 수 있다)
- [L18] 하도급거래 공정화에 관한 법률 — 법률 제21857호(시행 2026-10-02). 시행 예정: 법률 제21905호(시행 2027-09-09, 제12조의3은 대상 아님). https://likms.assembly.go.kr/law/lawsLawtInqyDetl1030.do?genActiontypeCd=2ACT1010&contId=1984123100000007&contSid=0122&basicDt=20261114&cachePreid=ALL&viewGb=EXE (확인 2026-11-14 — 페이지가 커서 WebFetch 요약이 조문을 놓칠 수 있다)
- [L19] KS A ISO 56000 계열 — KS A ISO 56002(혁신경영시스템 — 가이던스, 개정·확인 2022-06-30), KS A ISO 56001(혁신경영시스템 — 요구사항, 2026-08-26), KS A ISO 56005(지식재산관리, 2022-12-29). 국가기술표준원 e나라표준인증 목록. https://www.standard.go.kr/KSCI/standardIntro/getStandardSearchList.do (검색어 「혁신경영」, 확인 2026-11-14)
- [L20] 범부처 통합연구지원시스템(IRIS) — 법적 근거는 국가연구개발혁신법 제20조(통합정보시스템)·제13조제5항, 시행령 제43조. https://www.iris.go.kr (확인 2026-11-14)

### 글로벌

- [G1] ISO 56001:2024 Innovation management system — Requirements. 1판, 2024-09-10 발행, Published. https://www.iso.org/standard/79278.html (확인 2026-11-14)
- [G2] ISO 56002:2019 Innovation management — Innovation management system — Guidance. Published, 개정 결정(90.92) — 개정판 ISO/CD 56002 작성 중. https://www.iso.org/standard/68221.html (확인 2026-11-14)
- [G3] ISO 56003:2019 Innovation management — Tools and methods for innovation partnership — Guidance. Published, 2025 검토에서 유지. https://www.iso.org/standard/68929.html (확인 2026-11-14)
- [G4] ISO 56005:2020 Innovation management — Tools and methods for intellectual property management — Guidance. Published, 개정 결정 — ISO/CD 56005 2026-11-13 등록. https://www.iso.org/standard/72761.html (확인 2026-11-14)
- [G5] ISO 56008:2024 Innovation management — Tools and methods for innovation operation measurements — Guidance. Published. https://www.iso.org/standard/78485.html (확인 2026-11-14)
- [G6] OECD Frascati Manual 2015 — Chapter 2, ¶2.5(R&D 정의)·¶2.7(다섯 기준: novel, creative, uncertain, systematic, transferable and/or reproducible). https://www.oecd.org/content/dam/oecd/en/publications/reports/2015/10/frascati-manual-2015_g1g57dcb/9789264239012-en.pdf (확인 2026-11-14)
- [G7] OECD/Eurostat Oslo Manual 2018(4판) — ¶1.25 혁신 정의. https://www.oecd.org/content/dam/oecd/en/publications/reports/2018/10/oslo-manual-2018_g1g9373b/9789264304604-en.pdf (확인 2026-11-14)
- [G8] NASA NPR 7123.1D Appendix E, Technology Readiness Levels(시행 2023-07-05). https://nodis3.gsfc.nasa.gov/displayDir.cfm?Internal_ID=N_PR_7123_001D_&page_name=AppendixE (확인 2026-11-14)
- [G9] Horizon 2020 Work Programme 2018-2020 General Annexes, G. Technology readiness levels. https://ec.europa.eu/research/participants/data/ref/h2020/other/wp/2018-2020/annexes/h2020-wp1820-annex-g-trl_en.pdf (확인 2026-11-14)
- [G10] Cooper, R. G. (1990). Stage-gate systems: A new tool for managing new products. Business Horizons 33(3), 44–54. https://doi.org/10.1016/0007-6813(90)90040-I (확인 2026-11-14)
- [G11] Chesbrough, H. W. (2003). Open Innovation: The New Imperative for Creating and Profiting from Technology. Harvard Business School Press. ISBN 978-1-57851-837-1. https://books.google.com/books?vid=ISBN9781578518371 (확인 2026-11-14)
- [G12] Phaal, R., Farrukh, C. J. P., & Probert, D. R. (2004). Technology roadmapping — A planning framework for evolution and revolution. Technological Forecasting and Social Change 71(1–2), 5–26. https://doi.org/10.1016/S0040-1625(03)00072-6 (확인 2026-11-14)
- [G13] Bayh-Dole Act, 35 U.S.C. §§200–212 — §202(권리 귀속 선택·신고), §203(march-in). https://www.law.cornell.edu/uscode/text/35/part-II/chapter-18 (확인 2026-11-14)
- [G14] 26 U.S.C. §41(연구 세액공제, qualified research는 (d))·§174A(국내 연구비 당기 공제, Pub. L. 119-21로 2025-07-04 개정). https://www.law.cornell.edu/uscode/text/26/41 , https://www.law.cornell.edu/uscode/text/26/174A (확인 2026-11-14)
- [G15] 35 U.S.C. §102 — (b)(1) 발명자 공개 예외. https://www.law.cornell.edu/uscode/text/35/102 (확인 2026-11-14)
- [G16] Gesetz über Arbeitnehmererfindungen(ArbnErfG) — §5(신고), §6(청구·청구 의제), §9(보상). https://www.gesetze-im-internet.de/arbnerfg/ (확인 2026-11-14)
- [G17] 日本 特許法 第35条(職務発明) — 제3항 원시귀속 선택, 제4항 相当の利益. https://laws.e-gov.go.jp/law/334AC0000000121 (화면은 스크립트로 그려져 WebFetch로 비어 보인다 — 조문은 e-Gov 법령 API https://laws.e-gov.go.jp/api/1/articles;lawId=334AC0000000121;article=35 로 읽는다, 확인 2026-11-14)
- [G18] UK HMRC, Research and Development (R&D) tax relief: the merged scheme and Enhanced R&D Intensive Support(2024-04-01 이후 시작 회계기간). https://www.gov.uk/guidance/research-and-development-rd-tax-relief-the-merged-scheme-and-enhanced-rd-intensive-support (확인 2026-11-14)
- [G19] EU Horizon Europe Unit Model Grant Agreement V1.3(2025-12-15) — Article 16, Annex 5(결과의 소유·보호·활용). https://ec.europa.eu/info/funding-tenders/opportunities/docs/2021-2027/horizon/agr-contr/unit-mga_he_en.pdf (확인 2026-11-14)
- [G20] WIPO Patent Cooperation Treaty(PCT) 체계. https://www.wipo.int/en/web/pct-system (확인 2026-11-14)
- [G21] Paris Convention for the Protection of Industrial Property — Art.4(우선권). https://www.wipo.int/wipolex/en/text/288514 (확인 2026-11-14)
- [G22] ETSI Intellectual Property Rights Policy(ETSI Directives Annex 6, Version 52, 2025-12-05) — Clause 6.1 FRAND 약정. https://portal.etsi.org/directives/52_ETSI_directives_dec_2025.pdf (확인 2026-11-14)
- [G23] Directive (EU) 2016/943(영업비밀 보호) — Art.2(1) 정의. https://eur-lex.europa.eu/eli/dir/2016/943/oj (본문은 https://www.legislation.gov.uk/eudr/2016/943/article/2 보관본으로 확인, 확인 2026-11-14)
- [G24] Defend Trade Secrets Act, 18 U.S.C. §1839(정의)·§1836(민사 구제). https://www.law.cornell.edu/uscode/text/18/1839 (확인 2026-11-14)
- [G25] 2 CFR Part 200 Subpart E(Cost Principles) — §200.403 비용 인정 요건. https://www.law.cornell.edu/cfr/text/2/200.403 (확인 2026-11-14)
- [G26] 42 CFR Part 93(PHS Policies on Research Misconduct, 2024 개정 — 2026-01-01 이후 접수분 적용) — §93.234 정의. https://www.law.cornell.edu/cfr/text/42/93.234 (확인 2026-11-14)
- [G27] SBIR·STTR, 15 U.S.C. §638 — (e)(4) Phase I·II·III. Pub. L. 119-83(2026-04-13)으로 재승인. https://www.law.cornell.edu/uscode/text/15/638 (확인 2026-11-14)
- [G28] International Valuation Standards(effective 31 January 2025) — IVS 210 Intangible Assets. https://www.ivsc.org/standards/ (확인 2026-11-14)
- [G29] AUTM Licensing Activity Survey FY2024. https://autm.net/surveys-and-tools/surveys/licensing-survey/2024licensingsurvey (확인 2026-11-14)
- [G30] Stevenson-Wydler, 15 U.S.C. §3710a(CRADA). https://www.law.cornell.edu/uscode/text/15/3710a (확인 2026-11-14)
