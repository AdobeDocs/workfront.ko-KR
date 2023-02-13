---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 최종
description: 다음 기능은 현재 미리 보기 또는 베타에서 사용할 수 없지만 R1 - EDIT ME의 프로덕션 환경으로 릴리스되고 있습니다.
author: Luke
feature: Product Announcements
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1196'
ht-degree: 0%

---

# R1 최종

다음 기능은 현재 미리 보기 또는 베타에서 사용할 수 없지만 R1의 프로덕션 환경으로 릴리스됩니다.

## 내 작업 영역에서 증명을 위한 승인 결정(Workfront)

이제 사용자가 증명에 사용자를 추가하고 승인자 역할이나 검토자 및 승인자 역할(독립형 ProofHQ 애플리케이션이나 Workfront 내의 자동 워크플로우 사용)을 부여하면 승인 요청이 내 작업 영역의 승인 탭에 표시됩니다. 그런 다음 Workfront에서 직접 증명을 보고 증표에 대한 승인 결정을 내릴 수 있습니다.

자동화된 워크플로우를 사용하여 사용자를 증표에 추가하는 방법에 대한 자세한 내용은 [Adobe Workfront에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) in [Adobe Workfront에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

내 작업 영역에서 승인 결정을 내리는 방법에 대한 자세한 내용은 [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md) in [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## 내 작업 영역(Workfront) 내 교정 승인 보고서

이제 증명 승인 개체를 기반으로 보고서를 만들 수 있습니다. 이 보고서를 사용하면 사용자의 내 작업 영역에서 아직 결정을 내리지 않은 증명 승인을 보고할 수 있습니다.

증명 승인 보고서에는 다음 정보가 포함됩니다.

* 승인을 위해 제출된 문서
* 승인자의 이름
* 증명 버전
* 증명 ID
* 증명 생성 날짜

에 설명된 대로 개체를 기반으로 보고서를 만들 때 이 승인에 액세스합니다 [사용자 지정 보고서 만들기](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

증명 승인 객체 보고서에 대한 자세한 내용은 [Adobe Workfront의 개체 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 섹션 [Adobe Workfront의 개체 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 드래그 앤 드롭(Workfront)을 사용하여 새 버전의 문서 증명을 자동으로 생성

드래그 앤 드롭 방법을 사용하여 교정을 필요로 하는 문서의 새 버전을 추가하면 증명을 자동으로 생성합니다. 증명에는 원본 증명 또는 이전 버전과 동일한 옵션 및 워크플로우가 있습니다.

이전에는 새 버전의 문서를 추가할 때 새 버전에서 증명이 자동으로 생성되지 않았으므로 새 버전에 대한 증명을 다시 생성해야 했습니다.

[문서 추가 메뉴]를 사용하여 새 버전을 업로드하면 증명이 자동으로 생성되지 않습니다.

자세한 내용은

## 모든 교정 사용자가 Workfront 인터페이스에서 직접 ProofHQ에 액세스할 수 있도록 설정(Workfront)

이제 시스템의 모든 교정 사용자가 Workfront 인터페이스에서 직접 ProofHQ Premium 계정에 원활하게 액세스할 수 있도록 할 수 있습니다. 사용하도록 설정하면 모든 언어 교정 사용자는 전역 탐색 모음에 ProofHQ 사이트로 연결되는 ProofHQ 아이콘이 표시됩니다.

이 옵션은 기본적으로 활성화되어 있지 않습니다. 이 옵션을 사용하려면 Workfront 기술 지원 센터에 문의하여 시스템의 모든 언어 교정 사용자에 대해 이 액세스를 요청하십시오.

자세한 내용은 [Adobe Workfront에서 Workfront 증명 액세스](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) in  [Adobe Workfront에서 Workfront 증명 액세스](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

이 변경 전에 Workfront 관리자만 Workfront 인터페이스에서 ProofHQ 사이트에 직접 액세스할 수 있습니다.

## 발신 메일에 대한 TLS 보안 연결 새 옵션(Workfront)

고유한 이메일 서버를 사용하여 Workfront 통신을 관리하도록 선택하면 이제 발신 메일이 TLS 보안 연결을 사용하도록 설정할 수 있습니다.

이 개선 사항 전에 SSL 보안 연결을 통해서만 발신 메일을 활성화할 수 있습니다.

보내는 메일 구성에 대한 자세한 내용은 을 참조하십시오.

## 미리 보기 샌드박스 환경에서 전자 메일 관리를 위한 새 필드

이제 Workfront이 미리 보기 샌드박스 환경 및 사용자 지정 새로 고침 환경에서 모든 이메일 통신을 비활성화합니다. 미리 보기 샌드박스 또는 사용자 지정 새로 고침 환경에서 이메일 알림을 수신하려면 사용자 설정에서 이 기능을 활성화해야 합니다.

자세한 내용은 다음 정보를 참조하십시오.

* [Adobe Workfront 미리 보기 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) in [Adobe Workfront 미리 보기 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* 의 &quot;사용자 지정 새로 고침 샌드박스에서 이메일 수신&quot; [Adobe Workfront 사용자 지정 새로 고침 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Outlook for Office 365 (Workfront)

이제 Outlook 365용 Workfront 추가 기능을 사용할 수 있습니다. 

추가 기능 사용에 대한 자세한 내용은 [Outlook for Office 365에서 Workfront 추가 기능 사용.](https://support.workfront.com/hc/en-us/sections/205046167)

## 모바일 앱에서 검색(Workfront)

이제 웹 애플리케이션에서 검색하는 것과 유사한 방식으로 모바일 앱 내에서 개체를 검색할 수 있습니다. 새 검색 기능은 먼저 최근 항목 목록에서 항목을 찾고 이전에 모바일 장치로 다운로드한 개체를 찾습니다. 최근 항목 목록은 웹 응용 프로그램에서 보는 것과 동일한 목록입니다.

>[!NOTE]
>
>이 기능은 2017년 5월 첫 주에 제공됩니다.

모바일 앱에 대한 자세한 내용은 의 &quot;모바일에서 검색&quot; 섹션을 참조하십시오.  

## 모바일 앱의 개선된 도움말: Tutorials(Workfront)

4월에 모바일 릴리스부터 모바일 경험을 안내하는 새로운 자습서 화면이 표시됩니다. 처음으로 모바일 앱에 로그인하고 기능을 처음 사용하는 경우 이 기능이 작동하는 방식을 설명하는 간단한 자습서가 표시됩니다. 특정 기능을 처음 사용하는 경우에는 자습서가 한 번만 표시됩니다.

모바일 앱에 대한 자세한 내용은 을 참조하십시오.

## PDF 문서에서 검색(ProofHQ)

이제 PDF 문서, Office 문서 및 정적 웹 페이지에서 검색을 수행할 수 있습니다.

자세한 내용은  [증명 내에서 컨텐츠 검색](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## 전역 탐색 모음(ProofHQ)이 업데이트되었습니다.

이제 Workfront과 통합된 ProofHQ Premium 계정에는 ProofHQ 내의 전역 탐색 표시줄에 다음과 같은 개선 사항이 표시됩니다.

* 새 사용자 프로필 사진 
* 모양 및 느낌 업데이트

## 사용자 지정 보기에 추가 정보 포함(ProofHQ)

이제 사용자 지정 보기에 다음 추가 정보를 포함할 수 있습니다.

* **수신자 수준 데이터**\
   수신자 수준 데이터와 관련된 다음 열을 포함하도록 사용자 지정 보기를 구성할 수 있습니다. 역할, 위치, 이메일 경고, 내 최종 기한, 증명 추가 날짜 및 수신자 검색.\
   자세한 내용은 [Workfront 증명 증명에서 사용자 지정 보기 만들기 및 관리](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **교정 데이터**\
   교정 데이터와 관련된 다음 열을 포함하도록 사용자 정의 뷰를 구성할 수 있습니다. 주석 수(모든 버전), 디스크의 크기, 증명 유형, 버전당 파일 수, 주석 첨부 데이터(디스크의 크기, 파일 이름) 및 하위 폴더별 필터링\
   자세한 내용은 [Workfront 증명 증명에서 사용자 지정 보기 만들기 및 관리](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **자동화된 워크플로우와 관련된 단계 수준 데이터**\
   자동화된 워크플로우의 개별 단계와 관련된 다음 열을 포함하도록 사용자 지정 보기를 구성할 수 있습니다. SOCD 상태, 스테이지 마감일, 활성 스테이지 이름, 다음 단계 이름, 스테이지 이름 및 템플릿\
   자세한 내용은 [Workfront 증명 증명에서 사용자 지정 보기 만들기 및 관리](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## 교정 보고서 개선 사항(이전 Analytics)(ProofHQ)

보고 기능(이전의 Analytics)에는 다음과 같은 개선 사항이 포함되어 있습니다.

* 새 기본 보고서 유형:

   * 증명 전환 시간
   * 지연 승인 비율
   * 첫 번째 활동 시간 증명
   * 댓글 및 답글 수

* 보고서 인쇄
* 모양 및 느낌 업데이트

## 미리 보기 환경에서 증명 HQ 기능 보기(증명 HQ)

ProofHQ에 릴리스된 기능은 먼저 프로덕션 환경에 릴리스하기 전에 미리 보기 환경에서 테스트할 수 있습니다.

프로덕션 전 미리 보기에 기능을 릴리스하는 이 새로운 워크플로우를 통해 향후 ProofHQ 프로덕션 환경에 대한 업데이트를 보다 잘 준비할 수 있습니다.

ProofHQ 미리 보기 환경에 대한 자세한 내용은 [미리 보기 샌드박스 테스트 환경 - Workfront 증명](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
