# EU 사이버 복원력법(CRA) 실무 가이드

**디지털 제품 제조사 실무팀을 위한 기본 해설**
*EU Cyber Resilience Act (CRA): A Practitioner's Guide — A basic guide for product teams at manufacturers of products with digital elements (Korean-language edition)* · [English](#in-english)
- **저자** 최윤성 (한국오픈소스보안커뮤니티 리더)
- **발행** 한국오픈소스보안커뮤니티(K-OSSC)
- **판** v1.0 · 발행일 2026년 11월 23일(온라인판)
- **대상 규정** Regulation (EU) 2024/2847
- **이용 조건** CC BY-NC 4.0 · 온라인 무료 공개 · 비매품
<img width="1920" height="1080" alt="CRA_실무가이드_해설영상_썸네일" src="https://github.com/user-attachments/assets/1b56a4cd-3990-46bc-afbf-4fcace5046a0" />

## 내려받기

PDF는 2026년 11월 23일부터 **[Releases](https://github.com/k-ossc/cra-guide/releases)** 에서 내려받을 수 있습니다. 새 판이 나와도 이 페이지의 주소는 바뀌지 않습니다.

## 이 가이드는

2027년 12월 11일부터 EU 시장에 출시되는 디지털 요소를 포함한 제품은 CRA의 사이버보안 요건을 갖추어야 합니다. 적극적으로 악용된 취약점과 심각한 사고의 보고 의무는 2026년 9월 11일부터 이미 적용되고 있습니다. CRA는 EU 시장에 나가는 디지털 제품의 보안에 공통 기준을 세웁니다.

이 가이드는 EU에 제품을 수출하는 제조사가 제품에 내장된 소프트웨어의 취약점을 지원 기간 내내 관리하는 체계를 갖추고, 그 체계와 SBOM을 기술 문서의 증거로 남기도록 돕는 한국어 실무서입니다. 취약점 처리 요건(Annex I Part II)과 보고 의무(Article 14), SBOM의 작성·운영·제출, 그리고 이를 증빙으로 남기는 기술 문서(Annex VII)를 중심에 두고, 적용 범위·등급·적합성 평가는 그 체계가 놓이는 자리를 보여 주는 만큼만 다룹니다. 부록의 절차서·대장·점검표·추적표는 사내 문서로 바로 옮겨 쓸 수 있게 만들었습니다.

EU 시장에 제품을 내는 제조사의 실무팀과 경영·컴플라이언스 담당, 그리고 그 제품에 들어가는 소프트웨어를 만드는 개발자를 위해 썼습니다.

## 누가 어디를 읽으면 되나

이 가이드는 EU에 제품을 내는 제조사의 두 독자층을 위해 썼습니다. 체계를 만들고 운영하는 실무팀(보안·개발·제품 엔지니어링, PSIRT, DevSecOps)과, 그 체계에 책임을 지는 경영·컴플라이언스 담당입니다. 그 제품에 들어가는 소프트웨어를 만드는 개발자(OSS 개발자·스튜어드 포함)도 1·2·9·11·12장에서 자기 자리를 찾을 수 있습니다.

| 산출물 | 근거 조문 | 읽을 장 | 바로 쓰는 양식 |
|---|---|---|---|
| 취약점 관리 체계 | Article 13(8)·13(5)·13(6), Annex I Part II, Article 14 | 2장(2.6절), 5장(5.3절), 10장, 12장 | 부록 K 보고 절차서, 부록 I 점검표 |
| SBOM 증빙 | Annex I Part II(1), Annex VII 2(b)·8 | 8장(8.3절), 9장 | 부록 J SBOM 대장 5종, 부록 B 기술 문서 체크리스트 |
| 적용·분류·일정 | Article 2·3·7·8·71 | 2·3·4장 | 부록 D 결정 트리 |
| 요건·평가·문서 | Article 13, Annex I, Article 28~32 | 5·6·7·8장 | 부록 A·C·L |

## 구성

본문 15장과 부록 12개입니다.

1. 서론 및 배경
2. 제조사를 위한 CRA 핵심 개념 완전 해설
3. CRA 시행 일정 및 의무 발효 로드맵
4. 제품 분류 체계
5. 필수 사이버보안 요건(Annex I): 기술 구현 가이드
6. 사이버보안 위험 평가
7. 적합성 평가 절차
8. CE 마킹 및 3대 문서화 의무
9. SBOM(소프트웨어 구성요소 명세) 요건
10. 취약점 및 보안 사고 보고 의무 (Article 14)
11. 오픈소스 소프트웨어(OSS) 개발자·스튜어드를 위한 지침
12. 공급망 보안 및 제3자 컴포넌트 관리
13. CRA 규정 준수 로드맵
14. CRA와 타 EU 규제 연계
15. 제재·과징금 및 시장 감시

**부록**

- A. 필수 사이버보안 요건 전문 (Annex I 번역)
- B. 기술 문서 작성 체크리스트 (Annex VII 기반)
- C. EU 적합성 선언서(DoC) 기재 항목 양식
- D. 제품 분류 결정 트리 (Class I/II/일반)
- E. CRA 주요 용어 한-영 대조표
- F. 조화 표준 및 공통 사양 참조 목록
- G. 국가별 시장 감시 기관 현황과 확인 경로
- H. OSS 개발자 CRA 적용 여부 자가 진단 체크리스트
- I. 제조사 실무 CRA 준수 체크리스트
- J. 제조사 실무팀을 위한 SBOM 관리 5종 대장
- K. Article 14 보고 의무 이행 절차서 템플릿
- L. CRA 이행 단계별 진행 현황 추적표

## 기준 시점

본문은 2026년 11월 현재를 기준으로 합니다. 2026년 9월 11일부터 적용 중인 보고 의무(Article 14), 2026년 9월 11일 개통한 ENISA 단일 신고 플랫폼, 2025년 11월 채택된(12월 관보 게재) 중요·핵심 제품 기술 설명(Implementing Regulation (EU) 2025/2392)을 반영했습니다. 2026년 7월 집행위원회가 채택한 CRA 적용 가이던스(C(2026) 5252)의 내용도 반영했습니다. 조화 표준은 2026년 11월 19일 첫 표준(EN 40000-1-1·1-2)이 발간되었으나 관보에 인용된 것은 없어 3장·7장과 부록 F는 현황으로 적었습니다.

## 발행과 감수

- 발행: 한국오픈소스보안커뮤니티(K-OSSC)
- 저자: 최윤성
- 법률 감수: 법무법인 율촌 (변호사 김익현)
- 초안 리뷰: K-OSSC SIG 리드 (윤승한, 문광석)

이 가이드의 내용은 저자의 것이며, 감수와 리뷰에 참여한 단체와 개인의 공식 입장이 아닙니다. 감수의 범위는 책의 「감사의 글」에 적혀 있습니다.

## 이용 조건

© 2026 최윤성 · [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)(크리에이티브 커먼즈 저작자표시-비영리 4.0 국제)

저자 표기를 유지하면 비영리 목적으로 복제·배포·전송·번안할 수 있습니다. 그 밖의 상업적 이용을 원하면 저자 또는 한국오픈소스보안커뮤니티에 연락해 주십시오.

## 면책

이 가이드는 Regulation (EU) 2024/2847과 집행위원회·ENISA의 공개 자료를 바탕으로 한 저자의 해설이며 공식 해석이 아닙니다. 집행위원회·ENISA의 공식 자료가 우선합니다. 개별 사안의 법률 판단은 자격 있는 전문가와 상의하십시오. 저자와 발행처는 이 가이드의 이용으로 발생한 결과에 책임을 지지 않습니다.

## 정정 사항과 의견

오류와 개선 의견은 이 저장소의 [Issues](https://github.com/k-ossc/cra-guide/issues)로 보내 주십시오. 쪽 번호와 해당 문장을 함께 적어 주시면 됩니다. 다음 판에 반영합니다.

| 날짜 | 쪽 | 고치기 전 | 고친 뒤 |
|---|---|---|---|
| | | (아직 없습니다) | |

## 인용 표기

최윤성, 『EU 사이버 복원력법(CRA) 실무 가이드』 v1.0, 한국오픈소스보안커뮤니티(K-OSSC), 2026. https://github.com/k-ossc/cra-guide

## 한국오픈소스보안커뮤니티(K-OSSC)

커뮤니티 소개와 참여 방법은 [조직 페이지](https://github.com/k-ossc)에 있습니다.

## In English

**EU Cyber Resilience Act (CRA): A Practitioner's Guide** — a basic guide for product teams at manufacturers of products with digital elements (Korean-language edition).

- Author: Yunseong Choi · Publisher: Korea Open Source Security Community (K-OSSC)
- Version 1.0 · Publication date: 23 November 2026 (online edition) · Free to download, not for sale
- Subject: Regulation (EU) 2024/2847. The guide centres on vulnerability handling (Annex I, Part II), reporting obligations (Article 14), the SBOM, and the technical documentation (Annex VII) that keeps them as evidence. The appendices contain templates for procedures, registers, checklists and progress tracking.
- Licence: [CC BY-NC 4.0](https://creativecommons.org/licenses/by-nc/4.0/)
- This guide is the author's commentary and not an official interpretation. Official materials from the European Commission and ENISA take precedence.
- The text is in Korean. Corrections and comments are welcome through [Issues](https://github.com/k-ossc/cra-guide/issues), in Korean or English.
