# BeanPal — Free Coffee Roasting Software

[![Total Downloads](https://img.shields.io/github/downloads/chrysaor80/BeanPal-Releases-/total?style=flat-square&label=Total%20Downloads&color=4a90d9)](https://github.com/chrysaor80/BeanPal-Releases-/releases)
[![Latest Release](https://img.shields.io/github/v/release/chrysaor80/BeanPal-Releases-?style=flat-square&label=Latest&color=2ea44f)](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest)
[![Windows](https://img.shields.io/badge/Windows-10%2F11-blue?style=flat-square&logo=windows)](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest)
[![macOS](https://img.shields.io/badge/macOS-11%2B-black?style=flat-square&logo=apple)](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest)

BeanPal은 커피 로스터를 위한 **무료** 로스팅 모니터링 & 제어 소프트웨어입니다.

---

## 📥 다운로드

| 플랫폼               | 파일                                                                                                           |
| -------------------- | -------------------------------------------------------------------------------------------------------------- |
| **Windows** (10/11 x64)  | [BeanPal_2.3.4_x64-setup.exe](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest)            |
| **macOS** (Intel + Apple Silicon) | [BeanPal_2.3.4_universal.dmg](https://github.com/chrysaor80/BeanPal-Releases-/releases/latest) |

→ 전체 릴리즈 이력: [Releases 페이지](https://github.com/chrysaor80/BeanPal-Releases-/releases)

---

## ⚠️ macOS 처음 실행 시 — Gatekeeper 경고 해결

앱을 처음 열면 **"Apple에서 악성 소프트웨어가 있는지 확인할 수 없습니다"** 경고가 나타날 수 있습니다.

BeanPal은 Apple Developer ID로 정식 서명된 앱이지만, 첫 공증 처리 완료 전까지 이 경고가 표시됩니다. **아래 방법 중 하나로 한 번만 해제하면** 이후에는 정상 실행됩니다.

### 방법 1 — 터미널 (가장 확실)

```bash
xattr -cr /Applications/BeanPal.app
open /Applications/BeanPal.app
```

> 아무 메시지도 나타나지 않으면 성공입니다.

상황에 따른 명령 변형:

| 상황 | 명령 |
| ---- | ---- |
| Downloads 폴더에 있을 때 | `xattr -cr ~/Downloads/BeanPal.app` |
| 권한 오류(operation not permitted)가 날 때 | `sudo xattr -cr /Applications/BeanPal.app` |

### 방법 2 — 우클릭으로 열기

1. Finder → 응용 프로그램에서 BeanPal 찾기
2. 우클릭 → "열기" 선택 → 경고창에서 "열기" 클릭

### 방법 3 — 시스템 설정

1. BeanPal 더블 클릭 (경고 발생)
2. 시스템 설정 → 개인정보 보호 및 보안 → "그래도 열기"

> **왜 이런 경고가 나타나나요?** BeanPal은 Apple Developer ID로 서명된 안전한 앱입니다. Apple 공증(Notarization) 심사가 완료되기까지 며칠 소요되며, 그 사이 macOS가 임시로 차단합니다. 공증 완료 후 배포되는 버전부터는 이 경고 없이 바로 실행됩니다.

---

## 주요 기능

- **실시간 로스팅 모니터링** — BT/ET/배기 온도, RoR 그래프, 크랙 자동 감지
- **하드웨어 제어** — 가스/풍량/드럼 슬라이더, 인버터·서보 직접 제어
- **오토파일럿** — 프로파일 기반 완전 자동 로스팅
- **예열 자동화** — PID 제어로 목표 온도까지 자동 예열
- **AI 온도 예측** — TensorFlow 기반 다음 30초 온도 상승률 예측
- **프로파일 관리** — 로스팅 기록 저장/불러오기/비교 오버레이
- **생두 재고 관리** — 입고·출고·블렌딩 레시피 추적
- **커뮤니티** — 프로파일 공유, 버그 리포트, 토론 게시판

---

## 지원 로스터 (270개 프리셋, 90개 브랜드)

| 프로토콜    | 대표 브랜드                                              |
| ----------- | -------------------------------------------------------- |
| Modbus RTU  | Proaster, Easyster, Diedrich, Kaldi, 부자로스터 외 50+  |
| Modbus TCP  | iRm, Sweet Coffee, Besca, Coffed, Atilla 외             |
| S7 PLC      | Giesen (22개 모델), Probat G/UG                         |
| WebSocket   | Probat PIII (P05/P12/P25/P60)                           |
| Kaleido     | Sniper M1, M2 Pro, M6/M10                               |
| IKAWA BLE   | HOME, PRO, PRO X                                        |
| USB HID     | Aillio Bullet R1 V2                                     |
| Hottop      | 2K+, KN-8828B-2K                                       |
| Behmor      | 1kg, Jake, 1600 Plus                                    |
| Phidget     | TMP1101, TMP1100, 1048, 1051                            |

---

## 시스템 요구사항

|            | Windows                | macOS                       |
| ---------- | ---------------------- | --------------------------- |
| OS         | Windows 10/11 (64-bit) | macOS 11 Big Sur 이상       |
| RAM        | 4GB 이상               | 4GB 이상                    |
| 저장공간   | 500MB                  | 500MB                       |
| 아키텍처   | x64                    | Intel + Apple Silicon (Universal) |

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
