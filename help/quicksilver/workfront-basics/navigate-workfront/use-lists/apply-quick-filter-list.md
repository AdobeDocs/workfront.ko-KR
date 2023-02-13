---
navigation-topic: use-lists
title: 목록에 빠른 필터 적용
description: 객체 목록의 빠른 필터를 사용하면 중요한 항목만 찾을 수 있으므로 신속하게 검토, 업데이트 또는 다른 사용자와 공유할 수 있습니다.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# 목록에 빠른 필터 적용

<!--
{{highlighted-preview}}
-->

객체 목록의 빠른 필터를 사용하면 중요한 항목만 찾을 수 있으므로 신속하게 검토, 업데이트 또는 다른 사용자와 공유할 수 있습니다.

>[!IMPORTANT]
>
>빠른 필터를 사용하여 검색어가 포함된 항목을 찾을 수 있습니다. 해당 항목이 실제로 화면에 표시되었는지 또는 페이지 하단으로 스크롤한 후 표시되는지를 확인할 수 있습니다. 브라우저의 검색 기능을 사용하는 경우 화면에 물리적으로 표시되는 항목만 찾을 수 있습니다. 목록에 여러 페이지가 있는 경우, 빠른 필터가 표시되지 않는 페이지에 있는 항목을 찾지 못합니다.

빠른 필터를 저장하려면 목록에 대한 영구 필터를 대신 만드는 것이 좋습니다.\
에서 필터를 빌드하는 방법에 대한 자세한 내용 [!DNL Adobe Workfront], 문서를 참조하십시오 [의 필터 개요 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

빠른 필터는 현재 다음 영역에서 사용할 수 있습니다


다음을 제외하고 모든 목록에서 임시 빠른 필터를 사용할 수 있습니다.

* 다음 [!UICONTROL 보고서] 영역
* 문서 목록 및 보고서
* 몇 개 [!UICONTROL 설정] 영역
   >[!NOTE]
   >
   >빠른 필터는 다음 설정 영역에서 사용할 수 있습니다. [!UICONTROL 그룹], [!UICONTROL 팀], [!UICONTROL 회사], [!UICONTROL 예약], [!UICONTROL 레이아웃 템플릿], 및 [!UICONTROL 사용자 지정 Forms].


목록에 빠른 필터를 적용할 때 다음 사항을 고려하십시오.

* 키워드를 사용하여 목록 보기에 표시되는 모든 필드를 필터링할 수 있습니다. 여기에는 사용자 지정 필드 또는 다음과 같은 복잡한 필드가 포함됩니다. [!UICONTROL 선행 작업], [!UICONTROL 지정], [!UICONTROL 배정] 및 [!UICONTROL 상태], [!UICONTROL 승인자] 및 [!UICONTROL 상태]등
* 목록이 축소된 경우 빠른 필터를 사용하면 자동으로 확장됩니다. 빠른 필터를 제거하면 그룹이 다시 축소됩니다.
* 그룹화는 적용된 빠른 필터 또는 목록의 객체에 대한 변경 사항에 관계없이 원래 목록의 집계된 정보를 유지합니다.
* 빠른 필터는 임시 필터입니다. 목록 그룹화, 보기, 필터 또는 정렬을 변경하면 빠른 필터 기준이 제거됩니다.
* 빠른 필터를 저장할 수 없습니다. 필터를 저장하여 다시 사용하려면 목록에 대한 영구 필터를 만드는 것이 좋습니다.
* 목록에 둘 이상의 그룹이 있고 빠른 필터가 한 그룹에서만 항목을 찾으면 해당 그룹만 찾은 항목으로 표시됩니다. 다른 모든 그룹은 숨겨져 있습니다.
* 작업 또는 하위 작업 목록에서 빠른 필터 결과가 표시되면 작업 계층 구조가 제거됩니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 플랜*</b></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] 라이센스*</b></td> 
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>액세스 수준 구성*</b></td> 
   <td> <p>목록이 있는 영역에 대한 액세스 보기</p> <p>예를 들어 프로젝트에 빠른 필터를 적용하려면 프로젝트에 대한 [!UICONTROL 보기] 액세스 권한이 필요합니다.</p> <p>참고: 여전히 액세스할 수 없는 경우 [!DNL Workfront] 관리자가 액세스 수준에서 추가 제한을 설정한 경우<br>자세한 내용은 [!DNL Workfront] 관리자는 액세스 수준을 변경할 수 있습니다. <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>개체 권한</b></td> 
   <td> <p>[!UICONTROL View]</p> <p>추가 액세스 요청에 대한 자세한 내용은 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">개체에 대한 액세스 요청 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 목록에 빠른 필터 적용

1. 빠른 필터를 지원하는 목록 또는 보고서로 이동한 다음 **[!UICONTROL 빠른 필터] 아이콘** ![](assets/qs-quick-filter-icon.png) 클릭합니다.

   또는

   운영 체제나 브라우저에 따라 표준 QWERTY 키보드를 사용할 때 다음 명령 세트를 눌러 빠른 필터를 실행합니다.

   * 용 ALT+F [!DNL Windows] 컴퓨터
   * ALT/ Option+F for [!DNL Mac] 컴퓨터

      >[!TIP]
      >
      >Ctrl+F 또는 CMD+F를 누르면 빠른 필터 옆에 도구 설명이 표시되어 이러한 명령을 알려줍니다. 이 명령은 빠른 필터 검색 상자 내에도 표시됩니다.

1. 에서 **[!UICONTROL 페이지 필터링]** 상자에서 필터링할 키워드를 입력합니다.

   현재 목록 보기에 표시되는 단어를 사용할 수 있습니다.

   >[!NOTE]
   >
   >목록의 다른 페이지에 표시될 수 있는 단어를 사용하는 경우 빠른 필터에서 결과를 찾지 못합니다.

   검색 기준과 일치하는 항목의 목록이 입력하는 동안 동적으로 목록에 표시되고 다른 모든 항목이 숨겨집니다. 검색에서 사용한 키워드는 모든 독립형 및 복잡한 필드에서 노란색으로 강조 표시됩니다. 복합 필드의 일부 예로는 공유 열 또는 다음 중 하나가 있습니다. [!UICONTROL 지정], [!UICONTROL 지정] 및 [!UICONTROL 상태], [!UICONTROL 완료율], [!UICONTROL 선행 작업], [!UICONTROL 승인자 및 상태], [!UICONTROL 리소스 관리자], [!UICONTROL 카테고리], [!UICONTROL 조건], [!UICONTROL 조건 업데이트]등

1. (선택 사항) 빠른 필터에서 찾은 항목을 벌크로 편집하려면 다음을 수행합니다.

   1. 목록에서 항목을 모두 또는 여러 개 선택한 다음 **[!UICONTROL 편집]** 항목을 벌크로 편집하려면
   1. 편집을 완료한 후 **[!UICONTROL 변경 내용 저장]**.

1. (선택 사항) 빠른 필터에서 찾은 항목을 내보내려면 목록에서 항목을 모두 또는 여러 개 선택한 다음 를 클릭합니다 **[!UICONTROL 내보내기]**.

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >빠른 필터 검색에서 찾은 항목만 선택한 파일로 내보냅니다. 목록을 내보내기 전에 항목을 선택하지 않으면 필터링되지 않은 전체 목록이 내보내집니다.\
   >자세한 내용은 [목록 내보내기](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (선택 사항) 필터링된 결과를 지우려면 **[!UICONTROL 빠른 필터]** 창의 오른쪽 위 모서리에 있는 아이콘.\
   또는\
   페이지를 새로 고칩니다.
