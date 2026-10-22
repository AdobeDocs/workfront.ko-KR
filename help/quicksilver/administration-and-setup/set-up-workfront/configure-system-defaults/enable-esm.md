---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: 조직에 Adobe 클라우드 스토리지 활성화
description: 조직에서 모든 Adobe 제품에 통합 스토리지 솔루션을 사용하도록 Adobe 클라우드 스토리지를 활성화할 수 있습니다.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 5d487a068f747eb538775846cca80ab5a3a612bf
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 3%

---
# 조직에 Adobe 클라우드 스토리지 활성화

Adobe 클라우드 스토리지는 Adobe 엔터프라이즈 제품 전반에 걸쳐 에셋의 중앙 저장소 역할을 하는 통합 클라우드 기반 스토리지 솔루션입니다. 이 문서에서는 전체 조직 또는 특정 그룹에 대한 기본 저장소 옵션으로 Adobe 클라우드 저장소를 활성화하는 방법에 대해 설명합니다.

>[!IMPORTANT]
>
>Workfront의 설정 영역에서 Adobe 클라우드 스토리지를 활성화할 때까지 환경이 변경되지 않습니다.<br>
>Adobe 클라우드 스토리지를 활성화하면 새 프로젝트만 Frame.io 뷰어 및 통합 승인이 포함된 Adobe 클라우드 스토리지를 사용합니다. 기존 프로젝트는 현재 스토리지를 계속 사용하며 그대로 유지됩니다.

타이밍을 제어하므로 누구나 작업을 하기 전에 경험을 테스트하고, Workfront Fusion 시나리오를 업데이트하고, 변경 사항 보고를 위한 계획을 세울 수 있습니다. 차이점 및 롤아웃 계획 방법에 대한 자세한 내용은 [Adobe 클라우드 저장소에서 Workfront으로 이동](/help/quicksilver/review-and-approve-work/workfront-storage.md)을 참조하십시오.

## Adobe 클라우드 스토리지에서 승인이 작동하는 방식

Adobe 클라우드 스토리지는 프로젝트가 사용하는 승인 서비스를 결정합니다. Adobe 클라우드 스토리지를 지원하는 Workfront 버전으로 이동해도 전체 조직이 통합 승인으로 자동 전환되지는 않습니다. 대신, 승인 서비스는 각 프로젝트의 스토리지 모델에 따라 다릅니다.

* **Adobe 클라우드 저장소 프로젝트**&#x200B;는 기본적으로 Frame.io 뷰어에서 검토 및 승인과 함께 통합 승인을 사용합니다.
* **기존 Workfront 저장소 프로젝트**&#x200B;에서 이미 사용 중인 승인 서비스를 유지합니다. 조직에 따라 통합 승인 또는 기존 문서 승인일 수 있습니다.

Adobe 클라우드 스토리지의 검토 및 승인 경험에 대한 자세한 내용은 [Adobe 클라우드 스토리지의 Workfront으로 이동](/help/quicksilver/review-and-approve-work/workfront-storage.md)을 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td><p>모든 워크플로우 패키지</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td><p>표준</p> <p>플랜</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td>Workfront 관리자여야 합니다. </td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 조직에 Adobe 클라우드 스토리지 활성화

조직에 Adobe 클라우드 스토리지를 활성화하려면 다음을 수행하십시오.

{{step-1-to-setup}}

1. 왼쪽 탐색에서 **시스템**&#x200B;을 선택한 다음 **기본 설정**&#x200B;을 선택하십시오.
1. **저장소 환경 설정** 섹션까지 아래로 스크롤합니다.
1. 기본 드롭다운 메뉴에서 **Adobe 클라우드 저장소**&#x200B;를 선택합니다.
1. (선택 사항) Adobe 클라우드 저장소와 레거시 Workfront 저장소를 함께 사용하려면 **사용자가 저장소 공급자를 선택할 수 있도록 허용** 확인란을 선택하십시오.

   >[!NOTE]
   >
   >이 옵션을 활성화하면 사용자가 새 프로젝트를 만들 때 스토리지 공급자를 선택할 수 있습니다. Adobe 클라우드 스토리지는 기본 스토리지 제공업체이므로 &quot;새 프로젝트&quot;로 레이블이 지정됩니다. 레거시 Workfront 스토리지는 &quot;레거시 프로젝트&quot;로 레이블이 지정됩니다.
   >
   >![새 프로젝트 및 레거시 프로젝트 옵션](assets/new-esm-project.png)

1. 적용 대상 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.

   * **전체 조직**: 이 옵션은 기본 저장소 공급자를 전체 Workfront 환경에 적용합니다. 사용자가 새 프로젝트를 만들 때마다 기본 저장소 공급자가 사용됩니다.
   * **특정 그룹**: 이 옵션은 조직 내의 특정 그룹에만 기본 저장소 공급자를 적용합니다. 지정된 그룹의 사용자가 새 프로젝트를 만들 때마다 기본 저장소 공급자가 사용됩니다.

     ![저장소 환경 설정 그룹](assets/configure-storage-preference.png)

1. **저장**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >기존 프로젝트는 생성된 스토리지 모델을 유지합니다. 예를 들어 Adobe 클라우드 스토리지를 사용하는 프로젝트는 기본 스토리지 환경 설정을 변경한 후에도 Adobe 클라우드 스토리지를 계속 사용합니다.



## 샌드박스 환경의 Adobe 클라우드 스토리지

Adobe 클라우드 스토리지는 [!DNL Workfront] 샌드박스 환경에서 사용할 수 있으므로 프로덕션에서 롤아웃하기 전에 이 문서에 설명된 기능을 테스트할 수 있습니다. 그러나 Frame.io 뷰어는 샌드박스에서 사용할 수 없으므로 프로덕션에서 전체 통합 검토 및 승인 환경을 확인해야 합니다.

사용자 지정 새로 고침 샌드박스가 있는 경우 Adobe 클라우드 스토리지를 지원하는 Workfront 버전으로 업그레이드한 후 샌드박스를 새로 고쳐야 합니다. 새로 고침을 통해 샌드박스에 Adobe 클라우드 스토리지 기능에 대한 액세스 권한을 부여하므로 테스트를 시작할 수 있습니다. 자세한 내용은 [사용자 지정 새로 고침 샌드박스 환경](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)을 참조하십시오. [!DNL Adobe Workfront] 
