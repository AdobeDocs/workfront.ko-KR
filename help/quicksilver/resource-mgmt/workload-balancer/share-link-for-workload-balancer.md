---
product-area: resource-management
navigation-topic: the-workload-balancer
title: 링크와 작업 로드 밸런서 공유
description: 작업 로드 밸런서를 사용 가능한 리소스 영역이 없을 수 있는 다른 사용자와 공유할 수 있습니다. 작업 로드 밸런서 사용에 대한 자세한 내용은 작업 로드 밸런서 탐색 을 참조하십시오.
author: Alina
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: a74cc358c547e11a55cce728ad5330712ed0bd49
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# 링크와 작업 로드 밸런서 공유

작업 로드 밸런서를 사용 가능한 리소스 영역이 없을 수 있는 다른 사용자와 공유할 수 있습니다. 작업 로드 밸런서 사용에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>모든 계획</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>계획 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>다음 항목에 대한 액세스 권한 보기 이상:</p> 
    <ul> 
     <li> <p>리소스 관리</p> </li> 
     <li> <p>프로젝트</p> </li> 
     <li> <p>작업</p> </li> 
     <li> <p>문제</p> </li> 
    </ul> <p><b>메모</b>

여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 변경하는 방법에 대한 자세한 내용은 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">개체 권한</td> 
   <td> <p>프로젝트, 작업 및 문제에 대한 권한 보기 이상 </p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이선스 유형 또는 액세스 권한을 보유하고 있는지 알아보려면 Workfront 관리자에게 문의하십시오.

## 공유 링크에서 작업 로드 밸런서에 포함된 정보를 볼 때

다른 사용자와 작업 로드 밸런서에 대한 링크를 공유하면 공유 링크에 다음 정보가 포함됩니다.

* 작업 로드 밸런서의 지정된 작업 영역입니다.
* 프로젝트, 작업, 사용자 정보 여기에는 사용자 할당 정보가 포함됩니다.
* 선택한 필터에 따라 정보가 표시됩니다.

   >[!IMPORTANT]
   >
   >링크를 공유한 후 필터를 삭제하면 링크에서 작업 로드 밸런서를 보는 사용자에게 필터가 삭제되었다는 경고가 표시됩니다. 할당된 작업 영역의 모든 사용자를 봅니다. 작업 로드 밸런서의 기본 보기입니다.

* 이전에 선택한 주 수입니다.

공유 링크에서 작업 로드 밸런서를 보는 사용자는 다음 옵션을 사용하여 업데이트할 수 있습니다.

* 다음 타임라인 선택:

   * 오늘
   * 뒤로 및 전달 아이콘
   * 달력 선택

* 일, 주 및 월 아이콘
* 설정 아이콘
* 할당 표시 아이콘

   이러한 옵션 사용에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* 역할 할당 표시 아이콘

   프로젝트의 작업 로드 밸런서에만 사용할 수 있습니다.

공유 링크를 받은 사용자는 이 링크에서 작업 로드 밸런서에서 다음을 수행할 수 없습니다.

* 사용자에게 작업 항목 할당
* 사용자 할당 관리
* 원래 적용된 필터를 새로 만들거나 업데이트합니다

## 공유 링크에서 작업 로드 밸런서에서 정보를 보는 데 필요한 액세스

공유 링크에서 작업 로드 밸런서의 정보를 보려면 다음 액세스 권한이 필요합니다.

* 유효한 Adobe Workfront 라이센스이며 Workfront에 로그인해야 합니다.
* 적어도 액세스 수준에서 리소스 관리에 대한 액세스 권한을 봅니다. 리소스 관리 액세스 권한 부여에 대한 자세한 내용은 [리소스 관리에 대한 액세스 권한 부여](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* 작업 로드 밸런서에 표시된 프로젝트, 작업, 문제 및 사용자에 대한 권한을 봅니다.

## 링크에서 다른 사용자와 작업 로드 밸런서를 공유합니다

1. 작업 로드 밸런서로 이동

   작업 로드 밸런서 액세스에 대한 자세한 내용은 [작업 로드 밸런서 탐색](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (선택 사항) 다음 중 하나 이상을 수행합니다.

   * 기간 선택을 업데이트합니다.
   * 클릭 **일, 주**, 또는 **월** 일별, 주별 또는 월별 정보를 보려면

      ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * 지정되지 않음 및 지정된 작업 영역에 필터를 적용합니다.

      작업 로드 밸런서의 필터링 정보에 대한 자세한 내용은 [작업 로드 밸런서에서 정보 필터링](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. 을(를) 클릭합니다. **링크 아이콘** ![](assets/wb-shearable-link-icon-small.png).

   그러면 링크가 클립보드에 추가됩니다.

1. 다음 중 하나를 수행하여 링크를 다른 사용자와 공유합니다.

   * 전자 메일, 채팅 메시지 또는 기타 응용 프로그램에 붙여넣고 다른 사용자와 공유합니다.
   * 사용자 지정 섹션에 외부 페이지로 추가하고, 사용자 프로필에 사용자 지정 섹션을 추가하거나, 레이아웃 템플릿에 추가한 다음 사용자, 팀, 작업 역할 또는 그룹과 레이아웃 템플릿을 공유합니다.

      외부 페이지 만들기에 대한 내용은 [대시보드에 외부 웹 페이지 포함](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). 레이아웃 템플릿에 사용자 지정 섹션 추가에 대한 내용은 [레이아웃 템플릿을 사용하여 왼쪽 패널 사용자 정의](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

      >[!IMPORTANT]
      >
      >작업 로드 밸런서를 객체의 사용자 지정 섹션에 추가하면 작업 로드 밸런서의 정보가 객체에 의해 필터링되지 않습니다. 작업 로드 밸런서는 원래 적용된 필터로 필터링된 정보를 표시합니다.
