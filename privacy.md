# Shelfy 개인정보 처리방침 (Privacy Policy)

**앱 이름:** Shelfy
**개발자:** Kim Yongjin (개인 개발자)
**연락처:** anfy5118@gmail.com
**시행일:** 2026년 4월 18일

---

## 목차

1. 수집하는 정보 (Information We Collect)
2. 수집 목적 (Purpose of Collection)
3. 제3자 제공 (Third-Party Sharing)
4. 데이터 보관 기간 (Data Retention)
5. 데이터 보호 조치 (Data Security)
6. 이용자의 권리 (Your Rights)
7. 아동 개인정보 (Children's Privacy)
8. 광고 및 앱 추적 투명성 (Advertising & App Tracking Transparency)
9. 개인정보 처리방침 변경 (Changes to This Policy)
10. 연락처 (Contact)

---

## 1. 수집하는 정보 (Information We Collect)

Shelfy는 개인을 직접 식별하는 정보(이름, 이메일, 전화번호 등)를 수집하지 않습니다. 수집되는 정보는 서비스 제공에 필요한 최소한으로 제한됩니다.

### 1-1. 익명 사용자 ID (Firebase Authentication)

앱 설치 시 Firebase Authentication을 통해 익명 UID(User ID)가 자동 생성됩니다. 이 ID는 이용자를 개인으로 식별하지 않으며, 다음 용도에만 사용됩니다.

- Shelfy Pro 구독 상태 확인
- AI 기능(Gemini) 사용량 미터링
- Cloud Functions 감사 로그(audit log) 기록

### 1-2. 구독 정보 (RevenueCat)

Shelfy Pro 구독 시 RevenueCat SDK가 다음 정보를 수집합니다.

- RevenueCat이 생성한 익명 식별자
- 구매 영수증 데이터(App Store 또는 Google Play 검증용)
- 구독 상태 및 거래 이력

RevenueCat은 이름, 이메일, 결제 카드 정보를 수집하지 않습니다. 실제 결제 처리는 Apple 또는 Google이 담당합니다.

### 1-3. AI 사용량 미터링 (Cloud Functions)

AI 대화 기능 이용 시 Firebase Cloud Functions를 통해 Google Gemini API가 호출됩니다. 이 과정에서 다음 정보가 Firestore에 기록됩니다.

- 익명 UID
- 요청 횟수 및 타임스탬프

대화 내용(메시지 본문)은 서버에 저장되지 않습니다.

### 1-4. 사용 분석 (Firebase Analytics)

Firebase Analytics를 통해 익명 사용 패턴 데이터가 수집됩니다.

- 화면 조회, 기능 사용 이벤트 등 익명 행동 데이터
- 기기 유형, OS 버전, 앱 버전, 언어 설정
- 광고 ID는 ATT 동의 범위 내에서만 광고 타게팅에 사용되며, Firebase Analytics 이벤트 자체에는 연결되지 않습니다.

### 1-5. 충돌 로그 (Firebase Crashlytics)

앱 충돌 발생 시 Firebase Crashlytics를 통해 다음 정보가 자동 수집될 수 있습니다.

- 충돌 스택 트레이스 및 오류 유형
- 기기 모델, OS 버전, 앱 버전
- 충돌 발생 시각

충돌 로그에는 이용자의 개인 식별 정보나 앱 내 콘텐츠가 포함되지 않습니다.

### 1-6. 기기 로컬 데이터

아래 데이터는 이용자의 기기에만 저장되며, 개발자 서버로 전송되지 않습니다.

- 등록한 책, 독서 세션 기록, 독서 타이머 데이터
- 노트 및 인용문
- 바이브(감정) 트래킹 기록

이 데이터는 개발자가 접근할 수 없으며, 앱 삭제 시 영구적으로 삭제됩니다.

---

## 2. 수집 목적 (Purpose of Collection)

| 수집 항목 | 수집 목적 |
|---|---|
| 익명 UID (Firebase Auth) | 구독 확인, AI 사용량 제한, 감사 로그 |
| 구독 정보 (RevenueCat) | Shelfy Pro 구독 관리 및 검증 |
| AI 사용량 로그 (Firestore) | 무료/유료 플랜별 AI 사용량 미터링 |
| 사용 분석 (Firebase Analytics) | 앱 개선을 위한 익명 사용 패턴 파악 |
| 충돌 로그 (Crashlytics) | 버그 식별 및 앱 안정성 향상 |
| 기기 로컬 데이터 | 핵심 독서 기록 기능 제공 |

수집된 분석/로그 정보는 Shelfy의 서비스 개선 용도로만 사용됩니다. 광고 노출은 Google Mobile Ads SDK가 담당하며, 자세한 사항은 아래 8항을 참고해 주십시오.

---

## 3. 제3자 제공 (Third-Party Sharing)

Shelfy는 이용자의 개인정보를 판매하거나 임대하지 않습니다. 서비스 운영에 필요한 범위 내에서만 아래 제3자와 정보를 공유합니다.

### Google / Firebase

Firebase Authentication, Firestore, Analytics, Crashlytics, Cloud Functions를 운영합니다. Google은 이 데이터를 Google의 개인정보 처리방침에 따라 처리합니다.

참고: [Google 개인정보 처리방침](https://policies.google.com/privacy)

### RevenueCat

Shelfy Pro 구독 관리를 위해 익명 구독 데이터를 공유합니다.

참고: [RevenueCat 개인정보 처리방침](https://www.revenuecat.com/privacy)

### Apple / Google (결제 플랫폼)

인앱 구매 처리를 위해 해당 플랫폼과 결제 정보가 공유됩니다. 개발자는 결제 카드 정보에 접근하지 않습니다.

- Apple: [App Store 개인정보 정책](https://www.apple.com/legal/privacy/en-ww/)
- Google: [Google Play 개인정보 정책](https://policies.google.com/privacy)

위에 열거된 제3자 이외에는 이용자 데이터를 공유하지 않습니다.

---

## 4. 데이터 보관 기간 (Data Retention)

### 개발자가 보관하는 데이터

Firebase Firestore에 저장되는 AI 사용량 로그 및 감사 로그는 서비스 운영 목적에 필요한 기간 동안 보관되며, 해당 UID와 연결된 데이터는 익명 ID 삭제 또는 계정 비활성화 시 삭제 요청을 통해 처리됩니다.

### 제3자가 보관하는 데이터

RevenueCat, Firebase Analytics, Crashlytics가 보관하는 데이터의 보관 기간은 각 서비스의 개인정보 처리방침을 따릅니다.

### 기기 로컬 데이터

앱 삭제 시 기기의 모든 로컬 데이터가 영구 삭제됩니다.

---

## 5. 데이터 보호 조치 (Data Security)

Shelfy는 수집된 정보를 보호하기 위해 아래 조치를 취합니다.

- Firebase 보안 규칙을 통한 Firestore 접근 제어
- Cloud Functions에서의 HTTPS 암호화 통신
- 최소 권한 원칙 적용: 기능별로 필요한 데이터만 수집

다만, 인터넷을 통한 데이터 전송이나 전자적 저장 방식은 100% 보안을 보장할 수 없습니다. 중요한 개인 데이터는 앱 내에 저장하지 않도록 주의해 주십시오.

---

## 6. 이용자의 권리 (Your Rights)

이용자는 아래 권리를 행사할 수 있습니다.

- **열람권:** 수집된 데이터가 무엇인지 확인 요청
- **정정권:** 부정확한 데이터의 수정 요청
- **삭제권:** 수집된 데이터의 삭제 요청
- **처리 정지권:** 특정 목적의 데이터 처리 중단 요청

Shelfy 자체 서버에 저장되는 데이터는 최소한이므로, 대부분의 요청은 Firebase 또는 RevenueCat 등 제3자 서비스에 직접 요청하실 수 있습니다.

권리 행사 요청은 [anfy5118@gmail.com](mailto:anfy5118@gmail.com)으로 연락해 주십시오. 요청 접수 후 30일 이내에 처리합니다.

본 권리는 한국 개인정보보호법 및 GDPR, CCPA 등 관련 법령에 근거합니다.

---

## 7. 아동 개인정보 (Children's Privacy)

Shelfy는 만 14세 미만 아동을 대상으로 하지 않습니다. 만 14세 미만 아동으로부터 개인정보를 의도적으로 수집하지 않으며, 만 14세 미만은 Shelfy 사용이 제한됩니다.

만 14세 미만 아동이 앱을 사용하고 있다고 판단되는 경우, [anfy5118@gmail.com](mailto:anfy5118@gmail.com)으로 알려주시면 즉시 적절한 조치를 취하겠습니다.

(This app is not directed to children under the age of 14. We do not knowingly collect personal information from children under 14.)

---

## 8. 광고 및 앱 추적 투명성 (Advertising & App Tracking Transparency)

Shelfy는 무료 이용자에게 Google Mobile Ads(AdMob) 광고를 표시합니다. 광고 및 관련 추적은 다음과 같이 처리됩니다.

- **광고 제공:** Google Mobile Ads SDK를 통해 광고가 노출됩니다. Shelfy Pro 구독 시 광고가 비활성화됩니다.
- **App Tracking Transparency(ATT):** iOS 이용자에게는 앱 실행 시 ATT 권한 요청이 표시됩니다. 허용하지 않아도 광고는 계속 표시되지만, 맞춤형 광고는 제공되지 않습니다.
- **IDFA / GAID:** ATT 허용 시에만 iOS 광고 식별자(IDFA) 또는 Android 광고 식별자(GAID)가 광고 타게팅에 사용됩니다. 비허용 시에는 문맥 기반 광고만 제공됩니다.
- **광고 제공자의 개인정보 처리:** Google Mobile Ads의 데이터 처리 방침은 [Google Privacy Policy](https://policies.google.com/privacy)를 따릅니다.

Firebase Analytics가 수집하는 사용 패턴 데이터는 앱 품질 개선 용도이며, Shelfy는 Firebase Analytics를 광고 타게팅 목적으로 사용하지 않습니다.

---

## 9. 개인정보 처리방침 변경 (Changes to This Policy)

본 방침은 서비스 변경, 법령 개정 등의 사유로 업데이트될 수 있습니다. 변경 시 상단의 시행일을 갱신하며, 중요한 변경이 있는 경우 앱 내 공지를 통해 이용자에게 알립니다.

변경된 방침은 시행일부터 효력이 발생하며, 이후에도 앱을 계속 사용하면 변경된 방침에 동의한 것으로 간주됩니다.

---

## 10. 연락처 (Contact)

개인정보 처리방침 관련 문의, 권리 행사 요청, 기타 문의는 아래로 연락해 주십시오.

**Kim Yongjin**
독립 개발자 (Individual Developer)
이메일: [anfy5118@gmail.com](mailto:anfy5118@gmail.com)

---

*본 개인정보 처리방침은 2026년 4월 18일부터 시행됩니다.*

*Effective Date: April 18, 2026*

*© 2026 Kim Yongjin. All rights reserved.*
