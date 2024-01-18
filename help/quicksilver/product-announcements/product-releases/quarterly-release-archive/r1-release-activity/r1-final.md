---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 최종
description: 2018.3 릴리스 활동
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 38974e97-dea3-4c9e-bc32-bd55665370c7
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1177'
ht-degree: 0%

---

# R1 최종

다음 기능은 현재 미리보기 또는 베타에서 사용할 수 없지만 R1의 프로덕션 환경에 릴리스됩니다.

## 내 작업 영역에서 증명에 대한 승인 결정(Workfront)

이제 사용자가 증명에 귀하를 추가하고 승인자 역할 또는 검토자 및 승인자 역할( 독립 실행형 ProofHQ 애플리케이션에서 또는 Workfront 내의 자동화된 워크플로 사용)을 부여하면 승인 요청이 내 작업 영역의 승인 탭에 표시됩니다. 그런 다음 증명을 보고 Workfront에서 직접 증명에 대한 승인 결정을 내릴 수 있습니다.

자동화된 워크플로를 사용하여 증명에 사용자를 추가하는 방법에 대한 자세한 내용은 [Adobe Workfront 내에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) 위치: [Adobe Workfront 내에서 증명 공유](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

내 작업 영역에서 승인 결정을 내리는 방법에 대한 자세한 내용은 [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md) 위치: [작업 승인](../../../../review-and-approve-work/manage-approvals/approving-work.md). 

## 내 작업 영역 내의 증명 승인에 대한 보고서(Workfront)

이제 증명 승인 개체를 기반으로 보고서를 만들 수 있습니다. 이 보고서를 통해 아직 결정이 내려지지 않은 사용자의 내 작업 영역에서 증명 승인을 보고할 수 있습니다.

증명 승인 보고서에는 다음 정보가 포함되어 있습니다.

* 승인을 위해 제출된 문서
* 승인자 이름
* 증명 버전
* 증명 ID
* 증명 생성일

에 설명된 대로 객체를 기반으로 보고서를 작성할 때 이 승인에 액세스합니다 [사용자 지정 보고서 만들기](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

증명 승인 개체 보고서에 대한 자세한 내용은 [Adobe Workfront의 오브젝트 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 의 섹션 [Adobe Workfront의 오브젝트 이해](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## 드래그 앤 드롭을 사용하여 새 버전의 문서 증명 자동 생성(Workfront)

드래그 앤 드롭 방법을 사용하여 증명이 필요한 새 문서 버전을 추가하면 증명이 자동으로 생성됩니다. 증명에는 원본 증명 또는 이전 버전과 동일한 옵션 및 워크플로가 있습니다.

이전에는 문서 새 버전을 추가할 때 새 버전에서 증명이 자동으로 생성되지 않았으며 새 버전에 대한 증명을 다시 생성해야 했습니다.

추가 문서 메뉴를 사용하여 새 버전을 업로드할 때 증명이 자동으로 생성되지 않습니다.

자세한 내용은 의 섹션을 참조하십시오.

## 모든 증명 사용자가 Workfront 인터페이스(Workfront)에서 직접 ProofHQ에 액세스할 수 있도록 설정

이제 시스템의 모든 증명 사용자가 Workfront 인터페이스에서 직접 ProofHQ Premium 계정에 원활하게 액세스할 수 있습니다. 활성화되면 모든 증명 사용자에게 ProofHQ 사이트로 안내하는 ProofHQ 아이콘이 전역 탐색 모음에 표시됩니다.

이 옵션은 기본적으로 활성화되어 있지 않습니다. 이 옵션을 활성화하려면 Workfront 기술 지원에 문의하고 시스템의 모든 증명 사용자에 대해 이 액세스 권한을 요청하십시오.

자세한 내용은 [Adobe Workfront에서 Workfront 증명 액세스](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md) 위치:  [Adobe Workfront에서 Workfront 증명 액세스](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

이 변경 이전에는 Workfront 관리자만 Workfront 인터페이스에서 ProofHQ 사이트에 직접 액세스할 수 있었습니다.

## 발신 메일에 대한 TLS 보안 연결에 대한 새로운 옵션(Workfront)

이제 고유한 이메일 서버를 사용하여 Workfront 통신을 관리하도록 선택하면 보내는 메일이 TLS 보안 연결을 사용하도록 설정할 수 있습니다.

이 개선 이전에는 SSL 보안 연결을 통해서만 발신 메일을 활성화할 수 있었습니다.

보내는 메일 구성에 대한 자세한 내용은 을(를) 참조하십시오.

## 미리보기 샌드박스 환경에서 이메일을 관리하기 위한 새 필드

이제 Workfront은 미리보기 샌드박스 환경 및 사용자 정의 새로 고침 환경에서 모든 이메일 통신을 비활성화합니다. 미리보기 샌드박스 또는 사용자 정의 새로 고침 환경에서 이메일 알림을 수신하려면 사용자 설정에서 이 기능을 활성화해야 합니다.

자세한 내용은 다음 정보를 참조하십시오.

* [Adobe Workfront 미리보기 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 위치: [Adobe Workfront 미리보기 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).

* 의 &quot;사용자 정의 새로 고침 샌드박스에서 이메일 수신&quot; [Adobe Workfront 사용자 지정 새로 고침 샌드박스 환경](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)

## Office 365용 Outlook(Workfront)

이제 Outlook 365용 Workfront 추가 기능을 사용할 수 있습니다. 

추가 기능 사용에 대한 자세한 내용은 [Outlook for Office 365에서 Workfront 추가 기능 사용](https://support.workfront.com/hc/en-us/sections/205046167)

## 모바일 앱에서 검색(Workfront)

웹 애플리케이션에서 검색하는 것과 유사하게, 이제 모바일 앱 내에서 개체를 검색할 수 있습니다. 새 검색 기능은 먼저 최근 항목 목록의 항목과 모바일 장치에 이전에 다운로드한 개체를 찾습니다. 최근 항목 목록은 웹 응용 프로그램에 표시되는 것과 동일한 목록입니다.

>[!NOTE]
>
>이 기능은 2017년 5월 첫째 주에 사용할 수 있습니다.

모바일 앱에 대한 자세한 내용은 의 &quot;모바일 검색&quot; 섹션을 참조하십시오.  

## 모바일 앱의 도움말: Tutorials(Workfront)

4월 모바일 릴리스부터 모바일 경험을 안내하는 새로운 튜토리얼 화면이 표시됩니다. 모바일 앱에 처음 로그인하고 기능을 처음 사용하는 경우 기능의 작동 방식을 설명하는 간단한 자습서가 표시됩니다. 자습서는 특정 기능을 처음 사용할 때 한 번만 표시됩니다.

모바일 앱에 대한 자세한 내용은 을 참조하십시오.

## PDF 문서에서 검색(ProofHQ)

이제 PDF 문서, Office 문서 및 정적 웹 페이지에서 검색을 수행할 수 있습니다.

자세한 내용은  [증명 내 콘텐츠 검색](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/search-in-a-proof.md).

## 업데이트된 전역 탐색 바(ProofHQ)

Workfront과 통합된 ProofHQ Premium 계정에는 이제 ProofHQ 내의 전역 탐색 표시줄에 대한 다음과 같은 개선 사항이 표시됩니다.

* 새 사용자 프로필 사진 
* 업데이트된 모양 및 느낌

## 사용자 정의 보기에 추가 정보 포함(ProofHQ)

이제 사용자 지정 보기에 다음 추가 정보를 포함할 수 있습니다.

* **수신자 수준 데이터**\
  수신자 수준 데이터와 관련된 역할, 위치, 이메일 경고, 내 기한, 증명에 추가된 날짜 및 수신자 검색과 같은 열을 포함하도록 사용자 지정 보기를 구성할 수 있습니다.\
  자세한 내용은 [Workfront Proof에서 사용자 정의 보기 만들기 및 관리](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **증명 데이터**\
  댓글 수 (모든 버전), 디스크의 크기, 증명 유형, 버전당 파일 수, 댓글 첨부 파일 데이터 (디스크의 크기, 파일 이름) 및 하위 폴더별 필터링과 같은 증명 데이터와 관련된 열을 포함하도록 사용자 정의 보기를 구성할 수 있습니다.\
  자세한 내용은 [Workfront Proof에서 사용자 정의 보기 만들기 및 관리](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).
* **자동화된 워크플로 관련 단계 수준 데이터**\
  SOCD 상태, 단계 기한, 활성 단계 이름, 다음 단계 이름, 단계 이름 및 템플릿과 같은 자동화된 워크플로의 개별 단계와 관련된 열을 포함하도록 사용자 지정 보기를 구성할 수 있습니다.\
  자세한 내용은 [Workfront Proof에서 사용자 정의 보기 만들기 및 관리](../../../../workfront-proof/wp-work-proofsfiles/manage-your-work/create-and-manage-custom-views.md).

## 증명 보고서(이전 Analytics) 개선 사항(ProofHQ)

보고 기능(이전의 Analytics)에는 다음과 같은 개선 사항이 포함되어 있습니다.

* 새로운 기본 보고서 유형:

   * 증명 반환 시간
   * 지연 승인 백분율
   * 첫 번째 활동 시간 증명
   * 댓글 및 답글 수

* 보고서 인쇄
* 업데이트된 모양 및 느낌

## 미리보기 환경(ProofHQ)에서 ProofHQ 기능 보기

ProofHQ에 릴리스된 기능은 프로덕션 환경에 릴리스하기 전에 미리보기 환경에서 테스트할 수 있습니다.

프로덕션 이전 미리 보기에 대한 기능을 릴리스하는 이 새로운 워크플로우를 통해 ProofHQ 프로덕션 환경에 대한 향후 업데이트에 보다 잘 대비할 수 있습니다.

ProofHQ 미리보기 환경에 대한 자세한 내용은 [샌드박스 테스트 환경 미리보기 - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md).
