# BeanPal — Free Coffee Roasting Software

[![Total Downloads](https://img.shields.io/github/downloads/chrysaor80/BeanPal-Releases-/total?style=flat-square&label=Total%20Downloads&color=4a90d9)](https://github.com/chrysaor80/BeanPal-Releases-/releases)
[![Latest Release](https://img.shields.io/github/v/release/chrysaor80/BeanPal-Releases-?style=flat-square&label=Latest&color=2ea44f)](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%2F11-blue?style=flat-square&logo=windows)](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest)
[![macOS](https://img.shields.io/badge/macOS-11%2B-black?style=flat-square&logo=apple)](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest)

BeanPal은 커피 로스터를 위한 **무료** 로스팅 모니터링 & 제어 소프트웨어입니다.

---

## 📥 다운로드

| 플랫폼 | 파일 |
| ------ | ---- |
| **Windows** (10/11 x64) | [BeanPal_2.3.9_x64-setup.exe](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest) |
| **macOS** (Intel + Apple Silicon) | [BeanPal_2.3.9_universal.dmg](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest) |

> 전체 릴리즈 이력: [Releases 페이지](https://github.com/chrysaor80/BeanPal-Releases-/releases)

---

## 주요 기능

### 시작 마법사 — 3분 만에 로스팅 시작

처음 설치하면 시작 마법사가 로스터 선택부터 센서 연결까지 안내합니다. 210개 프리셋 중 자신의 로스터를 선택하면, 통신 설정·슬라이더·서브차트가 자동으로 구성됩니다. 별도의 매뉴얼 없이도 바로 로스팅을 시작할 수 있습니다.

[▶ 시작 마법사 데모](https://youtu.be/qlgDZ64wkxs)

### 실시간 로스팅 모니터링

온도계의 숫자가 바뀌는 순간 화면에 반영됩니다. 최대 19Hz 폴링으로 딜레이가 거의 없습니다. BT/ET/배기 온도, RoR 그래프를 실시간으로 확인하고, AUC(누적 열에너지)로 배치 간 일관성을 객관적으로 비교할 수 있습니다.

[▶ 일반 로스팅 데모](https://youtu.be/yWpkLqNIIF8)

### 하드웨어 제어

가스/풍량/드럼 슬라이더로 로스터를 직접 제어합니다. 인버터와 서보모터를 연결하면 소프트웨어에서 모든 조작이 가능합니다. 슬라이더 값을 직접 타이핑하여 정밀하게 입력할 수도 있습니다. 압력 단위(mmH₂O, kPa, mbar)도 선택할 수 있어 현장 게이지와 동일한 단위로 확인할 수 있습니다.

[▶ 슬라이더 사용 설정 데모](https://youtu.be/sH3jsN-MPKA) · [▶ 가스 압력 단위 설정 데모](https://youtu.be/k1qrBpALHUI)

### 압력 기반 가스 밸브 제어

가스 밸브 열림량과 실제 압력은 비선형 관계입니다. BeanPal은 자동 캘리브레이션 스캔으로 밸브 위치별 실제 압력을 측정하고, 슬라이더 50% = 실제 최대 압력의 50%가 되도록 자동 변환합니다. 사용할수록 자동 학습하여 정확도가 높아집니다.

[▶ 압력 연동 밸브 제어 데모](https://youtu.be/P5VXlBSfDGs)

### S7 PLC 로스터 지원 (Giesen · Probat · Bühler 등)

Giesen 22개 모델, Probat G/UG 등 S7 PLC 기반 로스터를 프리셋으로 지원합니다. 프리셋을 선택하고 로스터를 생성하면, 채널 매핑·슬라이더·서브차트가 모두 자동 설정된 상태로 바로 사용할 수 있습니다. 이전 버전처럼 사용자가 PLC 주소나 채널을 하나씩 설정할 필요가 없습니다.

[▶ Giesen 프리셋 생성 및 사용 데모](https://youtu.be/BBWBOp_it0Q)

### 오토파일럿 (자동 로스팅)

이전에 녹화한 로스팅 프로파일을 그대로 재생합니다. 가스, 풍량, 드럼 명령을 동일한 타임라인에 맞춰 자동으로 전송하여 일관된 로스팅을 구현합니다. 여러 배치를 연속 로스팅할 때 특히 유용합니다.

[▶ 오토파일럿 데모](https://youtu.be/JDIptR9ekEE)

### 예열 자동화

목표 온도를 설정하면 PID 제어로 자동 예열합니다. 예열이 완료되면 알림을 보내고, 투입 대기 상태로 전환됩니다. 예열 중에 다른 작업을 하다가 알림을 받고 투입하면 됩니다.

[▶ 예열 자동화 데모](https://youtu.be/-d-06vbugJ4)

### 온도 예측

과거 로스팅 패턴을 학습하여, 현재 로스팅에서 앞으로 온도가 어떻게 변할지 예측 곡선을 보여줍니다. 1크랙 타이밍이나 배출 시점을 미리 판단할 수 있어 로스팅 결정을 선제적으로 내릴 수 있습니다.

[▶ 온도 예측 데모](https://youtu.be/HEtWLcyNx4E)

### 프로파일 관리

로스팅 기록을 저장하고, 이전 프로파일을 현재 차트 위에 겹쳐서 실시간 비교할 수 있습니다. 최대 10개 프로파일을 동시에 비교하는 프로파일 비교 도구도 제공됩니다. 동일 원두의 배치별 편차를 한눈에 확인할 수 있습니다.

[▶ 참조 오버레이 데모](https://youtu.be/Z0HRGqu4CN4) · [▶ 프로파일 비교 데모](https://youtu.be/zvp-bFnCvwI)

### 건조 종료 자동 감지

BT 온도 변화율(RoR)을 분석하여 건조 종료 시점을 자동으로 잡아줍니다. 수동 마커도 3열 레이아웃으로 정리되어 있어 빠르게 찍을 수 있습니다.

### 생두 재고 관리

생두 입고, 출고, 재고량을 추적합니다. 블렌딩 레시피를 등록하면 각 원두의 배합 비율과 사용량을 자동으로 계산합니다. 국가별·등급별 필터링으로 원두를 빠르게 찾을 수 있습니다.

### 커뮤니티

프로파일을 다른 사용자와 공유하고, 버그 리포트나 기능 제안을 게시판에서 토론할 수 있습니다. 같은 로스터 사용자의 프로파일을 참고하여 자신의 로스팅을 개선하는 데 활용할 수 있습니다.

### 기타

- **투입 대기 모드** — 투입 전 데이터를 분리하여 RoR/AUC 계산에 영향 없음. 예열 완료 후 투입까지 기다리는 동안 불필요한 데이터가 로스팅 기록에 섞이지 않습니다.
- **온습도/압력 센서** — RS485 온습도 센서, 4-20mA ADC 압력 센서를 악세서리로 추가하여 환경 데이터를 함께 모니터링할 수 있습니다.
- **210개 로스터 프리셋** — Modbus RTU/TCP, S7 PLC, WebSocket, BLE, USB HID 등 다양한 프로토콜을 지원합니다. 프리셋을 선택하면 통신 설정이 자동 완료됩니다.

---

## 지원 로스터 (210개 프리셋, 86개 브랜드)

| 프로토콜 | 대표 브랜드 |
| -------- | ---------- |
| Modbus RTU | Proaster, Easyster, Kuban Manual, Kaldi, 부자로스터 외 50+ |
| Modbus TCP | iRm, Sweet Coffee, Besca, Coffed, Atilla, Diedrich, Petroncini ASEM 외 |
| S7 PLC | Giesen (22개 모델), Probat G/UG, Bühler RM 20/60-240, Brambati, Petroncini, Kuban Auto, Lilla |
| WebSocket | Probat PIII (P05/P12/P25/P60) |
| Kaleido | Sniper M1, M2 Pro, M6/M10 |
| USB HID | Aillio Bullet R1 V2 |
| Hottop | 2K+, KN-8828B-2K |
| Behmor | 1kg, Jake, 1600 Plus |
| Phidget | TMP1101, TMP1100, 1048, 1051 |

---

## 시스템 요구사항

| | Windows | macOS |
| --- | ------- | ----- |
| OS | Windows 10/11 (64-bit) | macOS 11 Big Sur 이상 |
| RAM | 4GB 이상 | 4GB 이상 |
| 저장공간 | 최소 500MB | 최소 500MB |
| 아키텍처 | x64 | Intel + Apple Silicon (Universal) |

> **macOS Intel Mac 참고**: 온도 예측(ML) 기능은 Intel Mac에서 사용할 수 없습니다 (TensorFlow AVX 요구사항). 그 외 모든 기능은 정상 동작합니다.

---

## 안전 주의사항

> BeanPal은 **"있는 그대로(AS-IS)"** 제공되는 무료 소프트웨어입니다.
> 오토파일럿 사용 중에도 **반드시 로스터를 직접 모니터링**하세요.
> 소프트웨어 사용 중 발생하는 장비 오작동, 화재, 데이터 손실에 대해 개발팀은 책임을 지지 않습니다.

---

## 문의

- **이메일**: [admin@beanpal.kr](mailto:admin@beanpal.kr)
- **웹사이트**: [https://beanpal.kr](https://beanpal.kr)
- **Issues**: [버그 신고 / 기능 제안](https://github.com/chrysaor80/BeanPal-Releases-/issues)
