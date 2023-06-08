---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: 워크스트림 보드에서 백로그 구성
description: 워크스트림의 보드에 백로그 열을 표시하도록 선택하고, 워크스트림 카드 목록에서 보드 백로그로 가져온 카드에 대한 질의를 정의할 수 있습니다.
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: fffbf47e75e5ff1b6cd7ce37e0198a07459006da
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# 워크스트림 보드에서 백로그 구성

워크스트림의 보드에 백로그 열을 표시하도록 선택하고, 워크스트림 카드 목록에서 보드 백로그로 가져온 카드에 대한 질의를 정의할 수 있습니다.

>[!NOTE]
>
>쿼리 기준과 일치하지 않는 새 카드를 백로그 열에 추가하면 보드를 새로 고칠 때 카드가 백로그에서 사라지고 카드 목록에서만 사용할 수 있습니다. 언제든지 쿼리를 변경하여 백로그 열에 표시되는 카드를 조정할 수 있습니다.

독립형 보드에서 백로그 열 및 쿼리를 사용할 수 없습니다. 독립 실행형 보드에 접수 열 추가에 대한 자세한 내용은 [보드에 접수 열 추가](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 워크스트림 보드에서 백로그 구성

{{step1-to-boards}}

1. 작업할 워크스트림을 엽니다. 작업 스트림을 열려면 다음을 클릭합니다. [!UICONTROL **작업 스트림 보기**].
1. 작업 스트림에서 보드를 클릭하여 엽니다.
1. 클릭 [!UICONTROL **구성**] 보드 오른쪽에서 Configure 패널을 엽니다.
1. 켜기 [!UICONTROL **이 보드에 백로그 열 포함**].

   백로그 열이 보드 왼쪽에 추가됩니다. 쿼리를 적용할 때까지 비어 있습니다.

1. 확장 [!UICONTROL **백로그 쿼리**].

   >[!NOTE]
   >
   >상태가 완료가 아닌 카드 목록의 모든 작업 항목을 표시하는 기본 쿼리가 이미 백로그에 적용되었을 수 있습니다.

1. 클릭 [!UICONTROL **조건 추가**] 그리고 &quot;빈&quot; 필드를 클릭합니다.
1. 쿼리할 필드를 선택합니다.

   선택할 수 있는 필드는 카드의 기본 필드입니다.

1. 쿼리 수정자를 선택합니다.

   수정자 옵션은 적용할 수 있는 필드에 따라 다릅니다. 예를 들어 &quot;name&quot; 필드에는 &quot;greater than&quot; 또는 &quot;less than&quot;이 수정자 선택 항목으로 지정되어 있지 않습니다. 해당 수정자는 숫자에만 적용되기 때문입니다.

1. 값을 선택합니다.

   한정자로 &quot;exists&quot; 또는 &quot;not exists&quot;를 사용하는 경우에는 값을 사용할 수 없습니다.

   예를 들어 &quot;만기일&quot; 및 &quot;존재함&quot;을 선택하면 백로그에는 만기일이 지정된 카드가 표시됩니다. 기한이 없는 카드는 백로그에 가져오지 않습니다.

1. (선택 사항) [!UICONTROL **조건 추가**] 을 눌러 다른 조건을 쿼리에 추가합니다.

   ![백로그 쿼리](assets/backlog-query-wrkstrm-board.png)

1. (선택 사항) [!UICONTROL **그룹 만들기**] OR 연산자를 사용하여 첫 번째 조건에 연결된 조건 그룹을 추가합니다.
1. 클릭 [!UICONTROL **쿼리 저장**].

   쿼리가 적용되고 기준을 충족하는 카드가 백로그 열에 나타납니다.
