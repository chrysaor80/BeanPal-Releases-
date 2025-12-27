# BeanPal v1.8.9

**무료 AI 로스팅 소프트웨어** - AI 온도 예측까지 무료로.

---

## v1.8.9 신규 기능

### Probat PIII WebSocket 연동
- Probat PIII 시리즈 실시간 WebSocket 통신 지원
- 센서 데이터 자동 수신 (Bean/Air/배기 온도, 버너, 드럼 속도)
- 로스팅 이벤트 자동 감지 (CHARGE, DROP, DRY, 1차/2차 크랙)
- **지원 모델**: P01, P05 III, P12 III, P25 III, P60 III (2020년~)

---

## 주요 기능

### 모니터링 & AI
| 기능 | 설명 |
|------|------|
| **실시간 모니터링** | 온도(Bean/Air/배기), RoR, 인버터, 댐퍼, 압력 그래프 표시 |
| **기울기 예측** | AI 학습 없이 바로 사용 가능한 온도 추세 예측 |
| **AI 온도 예측** | TensorFlow 기반 다음 온도 예측 (세계 최초 무료) |
| **AI 학습 시스템** | 나만의 로스팅 패턴 학습 및 모델 관리 |

### 자동화 기능
| 기능 | 설명 |
|------|------|
| **로스팅 오토파일럿** | 이벤트/온도/시간/RoR 기반 자동 제어 (v1.8.6+) |
| **로스터기 예열** | PID 제어 자동 예열 + 평형점 탐색 (v1.8.8+) |
| **자동 로스팅** | 저장된 프로필대로 자동 로스팅 (튜닝 필요) |
| **S7 PLC 슬라이더 제어** | Giesen 등 S7 로스터기 실시간 제어 (v1.8.5+) |

### 데이터 관리
| 기능 | 설명 |
|------|------|
| **프로필 관리/비교** | 최대 10개 프로필 동시 비교 + 참조 오버레이 |
| **생두 정보 관리** | 원산지, 품종, 가공법, 등급 등 상세 정보 |
| **재고 관리** | 생두 입고/출고, 로스팅 시 자동 차감 |
| **블렌드 관리** | 블렌드 레시피 저장 및 구성 비율 설정 |
| **커핑 스코어** | SCA 기준 커핑 점수 및 노트 기록 |

### 시스템
| 기능 | 설명 |
|------|------|
| **다중 사용자** | 역할별 권한 설정 (관리자/로스터/뷰어) |
| **다국어** | 한국어 / English |

---

## 지원 로스터기

**Modbus RTU/TCP**
- RoastPro, Easyster, Proaster THCR, TRINITAS, Toper, Has Garanti, Santoker, Kaleido, KAMEL

**Siemens S7 PLC** *(실제 검증 전)*
- Giesen (WxA 시리즈), Bühler, Probat G/UG, Petroncini, Kirsch+Mausser, Kuban, Lilla, Brambati

**WebSocket (신규)**
- Probat PIII (P01, P05 III, P12 III, P25 III, P60 III)

**USB 센서 / 시리얼 온도계**
- Phidget TMP1101/1100/1048/1051
- CENTER 306/305, VOLTCRAFT K202

---

## 시스템 요구사항

- **OS**: Windows 10/11 (64-bit)
- **RAM**: 4GB 이상
- **저장공간**: 1GB 이상

---

## 설치

1. `BeanPal_1.8.9_x64-setup.exe` 다운로드
2. 설치 파일 실행
3. BeanPal 실행 후 로스터기 연결 설정

---

## 데모 영상

| 주제 | 링크 |
|------|------|
| 시작 마법사 | https://youtu.be/qlgDZ64wkxs |
| 슬라이더 설정 | https://youtu.be/sH3jsN-MPKA |
| 가스 압력 단위 설정 | https://youtu.be/k1qrBpALHUI |
| 참조 기능 | https://youtu.be/Z0HRGqu4CN4 |
| 일반 로스팅 | https://youtu.be/yWpkLqNIIF8 |
| 프로필 비교 | https://youtu.be/zvp-bFnCvwI |
| AI 모델 설정 | https://youtu.be/HEtWLcyNx4E |
| 예열 기능 | https://youtu.be/-d-06vbugJ4 |
| 오토파일럿 | https://youtu.be/JDIptR9ekEE |

---

## 튜닝 서비스

| 패키지 | 가격 | 내용 |
|--------|------|------|
| Basic | 30만원 | 로스터기 연동 + 기본 설정 + 방문 지원 1회 |
| **Auto** | ~~100만원~~ **50만원** | 자동 로스팅 세팅 + 밸브 제어 서비스 포함 |

### 프로모션 안내

> **Auto 패키지 50% 할인 이벤트** (2026년 5월까지)
> - 정가 100만원 → **50만원**
> - 밸브 제어 서비스(서보모터 설치) 포함
> - 자동 로스팅 세팅 완료까지 지원

### 출장 지역 안내

> **기준 지역**: 성남시
> - 성남시 기준 **50km 이내**: 출장비 무료
> - 성남시 기준 **50km 초과**: 별도 출장비 추가 (거리에 따라 상이, 문의 필요)

> **참고**: 튜닝에 필요한 디바이스(인버터, 압력계 등)는 직접 구매하셔야 합니다.

### 호환 디바이스

| 종류 | 제조사 | 모델 | 비고 |
|------|--------|------|------|
| 인버터 | LS산전 | Modbus RTU 지원 모델 | 배기 모터 / 드럼 스피드 제어 |
| 압력계 | 센서시스템 | Modbus RTU 지원 모델 | 드럼 내부 압력 측정 |
| 서보모터 | - | - | 화력(가스밸브) 제어, Auto 튜닝 시 무료 제공 |

> 인버터, 압력계는 고가의 기성품입니다. 구매 전 문의 주시면 상담해드립니다.

---

## 문의

- **웹사이트**: https://beanpal.kr
- **이메일**: chrysaor80@naver.com
- **GitHub Issues**: [버그 리포트](https://github.com/chrysaor80/BeanPal/issues)
- **GitHub Discussions**: [질문/제안](https://github.com/chrysaor80/BeanPal/discussions)

---

*프로그램 자체는 영구 무료입니다. 피드백 주시면 최대한 반영하겠습니다.*
