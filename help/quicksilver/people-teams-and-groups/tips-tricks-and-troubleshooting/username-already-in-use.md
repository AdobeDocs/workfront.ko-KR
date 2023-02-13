---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: 이미 사용 중인 사용자 이름
description: 사용자 이름이 이미 사용되고 있을 때 오류가 발생하면 다음 팁을 읽어 보십시오.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# 이미 사용 중인 사용자 이름

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜</strong></td> 
   <td> <p>모든</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이선스</strong></td> 
   <td> <p>[!UICONTROL 계획]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성</strong></td> 
   <td> <p>[!UICONTROL System 관리자]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 질문

새 사용자를 만들 때 [!UICONTROL 우프] 사용자 이름이 이미 사용되었다는 오류가 표시됩니다. 시스템에 이 이메일에 대한 다른 항목이 없습니다. 표시되는 이유는 무엇입니까?

## 솔루션

이 문제는 사용자 이름 또는 이메일 주소가 현재 고유하지 않기 때문에 발생할 수 있습니다 [!DNL Adobe Workfront] 인스턴스. 사용자는 별도의 인스턴스에 동일한 사용자 이름 또는 이메일 주소를 사용할 수 있습니다. 예를 들어 사용자 A는 다음과 같은 이메일 주소를 [!DNL Workfront] 계정: usera@company1.com 및 usera@company2.com에서 확인하십시오.

>[!NOTE]
>
>기본 [!DNL Workfront] 동일한 클러스터에서 별도의 Workfront 인스턴스에 있는 관리자는 동일한 사용자 이름 또는 이메일 주소를 가질 수 없습니다.
>
>인스턴스가 서로 다른 클러스터에 있는 경우 기본 관리자는 동일한 사용자 이름 또는 이메일 주소를 가질 수 있습니다. 인스턴스가 있는 클러스터를 아래에 볼 수 있습니다 [!UICONTROL 설정] > [!UICONTROL 시스템] > [!UICONTROL 고객 정보].

### 인스턴스에서 사용자 이름이 고유한지 확인합니다

사용자 이름과 전자 메일 주소가 현재 사이트에서 고유한지 확인합니다 [!DNL Workfront] 인스턴스:

1. 로서의 [!DNL Workfront] administrator에서 **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 사용자]**.
1. 사람 목록에서 **[!UICONTROL 이메일]** 열에 중복 이메일이 없는지 확인합니다.
1. 사용자 이름 열을 보기에 추가합니다.

   1. 에서 **[!UICONTROL 보기]** 드롭다운 메뉴에서 **[!UICONTROL 보기 사용자 지정]**.
   1. 클릭 **[!UICONTROL 열 추가]**.
   1. 검색 필드에 을 입력합니다 *[!UICONTROL 사용자 이름]*.
   1. 선택 **[!UICONTROL 사용자]** > **[!UICONTROL 사용자 이름]**.
   1. 보기를 저장합니다.\
      이렇게 하면 중복 항목을 찾을 수 있는 사용자 이름을 표시하는 보기가 표시됩니다.

1. 사람 목록에서 **[!UICONTROL 사용자 이름]** 열이 포함되어 있습니다.
