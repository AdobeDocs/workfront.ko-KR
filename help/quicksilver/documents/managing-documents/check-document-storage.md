---
product-area: documents
navigation-topic: manage-documents
title: 문서 저장 공간 제한 확인
description: Adobe Workfront 관리자는 고객 정보 페이지에서 문서 스토리지 사용량 및 할당량을 볼 수 있습니다. 저장소 표시 방법은 조직이 기존 Workfront 저장소를 사용하는지 또는 Adobe 클라우드 저장소를 사용하는지에 따라 다릅니다.
author: Courtney
feature: Digital Content and Documents
exl-id: f5d1963e-b205-44b9-b2b6-b7de465c6977
last-update: 2026-04-29T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/vOjgBLxX5rFIGHBCHB2a6Q3Bs3KE5x-opXUMvANjI1E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 09dff59503604894e61f2a62af7ae1c2e8a39068
workflow-type: tm+mt
source-wordcount: 491
ht-degree: 3%

---

# 문서 저장 공간 제한 확인

사용자가 Workfront 인스턴스에 업로드할 수 있는 개별 파일의 유형과 크기에는 제한이 없지만 Workfront 플랜에는 총 스토리지 할당량이 포함됩니다. Workfront 관리자는 고객 정보 페이지의 설정 영역에서 사용량 및 할당량을 모니터링합니다.

저장소 표시 방법은 조직이 기존 Workfront 저장소를 사용하는지 Adobe 클라우드 저장소를 사용하는지에 따라 다릅니다.

* 기존 Workfront 저장소를 사용하는 경우 이 문서에서 [기존 Workfront 저장소](#legacy-workfront-storage)를 참조하십시오.
* Adobe 클라우드 저장소를 사용하는 경우 이 문서에서 [Adobe 클라우드 저장소](#adobe-cloud-storage)를 참조하십시오.

  Adobe 클라우드 저장소에 대한 자세한 내용은 [Adobe 클라우드 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Workfront 플랜</td> 
   <td> <p>레거시 저장소를 사용하여 문서를 관리하는 모든 Workfront 패키지</p>
      <p>Adobe 클라우드 스토리지를 사용하여 문서를 관리하는 모든 워크플로우 패키지</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> </td> 
  </tr> 
 </tbody> 
</table>

이 표의 정보에 대한 자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 이전 Workfront 스토리지

조직에서 기존 Workfront 스토리지를 사용하는 경우 고객 정보 페이지에 Workfront에 직접 업로드한 문서에 대한 단일 스토리지 할당량이 표시됩니다.

기존 Workfront 문서 저장소를 확인하려면:

{{step-1-to-setup}}

1. 왼쪽 패널에서 **시스템** > **고객 정보**&#x200B;를 클릭합니다.
1. **기본 정보** 섹션에서 **저장소 할당량**&#x200B;을(를) 찾으십시오. 여기에서 현재 사용 중인 스토리지 용량과 Workfront 플랜에 포함된 총 스토리지 용량을 확인할 수 있습니다.

스토리지 할당량은 최신 개수를 표시하기 위해 매일 새로 고쳐집니다.

>[!NOTE]
>
>이 제한은 다른 타사 서비스 공급자(SharePoint, Google 드라이브, Webdam, Box, Dropbox 또는 기타 문서 에셋 관리 공급자)로부터 Workfront에 연결하는 문서에는 적용되지 않습니다.

## Adobe 클라우드 스토리지


조직에서 Adobe 클라우드 스토리지를 사용하는 경우 스토리지 할당량은 Workfront 라이선스를 통해 프로비저닝된 스토리지와 Frame.io Enterprise 추가 기능을 통해 프로비저닝된 스토리지를 결합하는 단일 풀링된 할당으로 보고됩니다. 스토리지 사용량에 대한 하드 캡은 없습니다. 사용자는 사용량이 할당량을 초과하더라도 문서를 계속 업로드할 수 있습니다.

### 고객 정보에 대한 스토리지 사용량 보기

Adobe 클라우드 스토리지에서 문서를 확인하려면:

{{step-1-to-setup}}

1. 왼쪽 패널에서 **시스템** > **고객 정보**&#x200B;를 클릭합니다.
1. **저장소 개요** 섹션으로 이동합니다.
1. 사용량을 검토합니다. 스토리지 개요 는 풀링된 스토리지 할당량을 표시하고 사용량을 다음으로 나눕니다.

   * Workfront 레거시 프로젝트 및 Adobe 클라우드 스토리지 프로젝트가 파란색 막대에 표시됩니다.
   * 프레임 독립 실행형 프로젝트가 녹색 막대에 표시됩니다. 이러한 프로젝트는 Workfront과 별개이며 Frame.io Enterprise 라이선스가 있는 경우에만 사용할 수 있습니다.


고객 정보에 대한 ![Adobe 클라우드 저장소 사용](assets/storage-usage.png)

사용 수치는 정기적으로 새로 고쳐지므로 최신 수를 확인할 수 있습니다.

### 관리자용 이메일 알림

사용량이 스토리지 할당량의 75%, 90% 또는 100%를 초과하면 Workfront에서 시스템 관리자에게 이메일 알림을 보냅니다.
