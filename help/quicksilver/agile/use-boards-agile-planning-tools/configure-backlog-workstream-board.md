---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: 작업 스트림 보드에서 백로그 구성
description: 작업 스트림의 보드에 백로그 열을 표시하고 작업 스트림 카드 목록에서 보드 백로그로 가져오는 카드에 대한 쿼리를 정의할 수 있습니다.
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 75bb5af9564947a39e1cb46f9d6be2c03eb07acc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# 작업 스트림 보드에서 백로그 구성

작업 스트림의 보드에 백로그 열을 표시하고 작업 스트림 카드 목록에서 보드 백로그로 가져오는 카드에 대한 쿼리를 정의할 수 있습니다. 이 옵션은 독립 실행형 보드에서 사용할 수 없습니다. 독립형 보드에 취침 열 추가에 대한 자세한 내용은 [보드에 흡기 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td> <p>[!UICONTROL Request] 이상</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 작업 스트림 보드에서 백로그 구성

{{step1-to-boards}}

1. 작업할 작업 스트림을 엽니다. 작업 스트림을 열려면 [!UICONTROL **작업 스트림 보기**].
1. 작업 스트림의 보드를 클릭하여 엽니다.
1. 클릭 [!UICONTROL **구성**] 보드 오른쪽의 구성 패널을 엽니다.
1. 켜기 [!UICONTROL **이 보드에 백로그 열을 포함합니다.**].

   보드 왼쪽에 백로그 열이 추가됩니다. 쿼리를 적용할 때까지 비어 있습니다.

1. 확장 [!UICONTROL **백로그 쿼리**].

   >[!NOTE]
   >
   >백로그에 기본 쿼리가 이미 적용되어 반복되지 않고 완료 상태가 아닌 카드 목록의 모든 작업 항목이 표시됩니다.

1. 클릭 [!UICONTROL **조건 추가**] 을 클릭하고 &quot;empty&quot; 필드를 클릭합니다.
1. 쿼리할 필드를 선택합니다.

   선택할 수 있는 필드는 카드의 기본 필드입니다.

1. 쿼리 수정자를 선택합니다.

   수정자 옵션은 적용할 수 있는 필드에 따라 다릅니다. 예를 들어 &quot;name&quot; 필드에는 &quot;보다 큼&quot; 또는 &quot;보다 작음&quot;을 수정자 선택 항목으로 사용할 수 없습니다. 이러한 수정자는 숫자만 적용되기 때문입니다.

1. 값을 선택합니다.

   이 값은 수정자로 &quot;존재함&quot; 또는 &quot;존재하지 않음&quot;을 사용하는 경우 사용할 수 없습니다.

   예를 들어 &quot;기한&quot; 및 &quot;존재함&quot;을 선택하면 백로그에 지정된 만기 날짜가 있는 카드가 표시됩니다. 만기 날짜가 없는 카드는 백로그로 가져오지 않습니다.

1. (선택 사항) [!UICONTROL **조건 추가**] 을 눌러 쿼리에 다른 조건을 추가합니다.

   ![백로그 쿼리](assets/backlog-query-wrkstrm-board.png)

1. (선택 사항) [!UICONTROL **그룹 만들기**] OR 연산자로 첫 번째 조건에 연결된 조건 그룹을 추가합니다.
1. 클릭 [!UICONTROL **쿼리 저장**].

   쿼리가 적용되고 조건을 충족하는 카드가 백로그 열에 나타납니다.
