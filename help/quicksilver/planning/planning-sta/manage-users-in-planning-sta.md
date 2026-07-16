---
title: Adobe Workfront Planning에서 사용자를 독립 실행형 제품으로 관리
description: 이 문서에서는 Planning을 독립형 제품으로 구입할 때 Adobe Workfront Planning에서 사용자 및 팀을 관리하는 방법에 대해 설명합니다.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: ee260723331ddff4e8d89f7d9ca2b807835d6130
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 0%

---


# Adobe Workfront Planning에서 사용자를 독립 실행형 제품으로 관리

>[!IMPORTANT]
>
>이 문서의 정보는 독립 실행형 제품으로 구입한 경우 Adobe Workfront Planning에 적용됩니다. 귀사에서 Adobe Workfront Planning 전용 패키지를 구매했지만 Workfront Workflow 패키지를 구매하지 않은 경우 이 문서를 참조하십시오.
>
>Workfront 패키지와 함께 구입한 경우 Adobe Workfront Planning에 대한 자세한 내용은 [Adobe Workfront Planning 시작](/help/quicksilver/planning/general/planning-overview.md)을 참조하십시오.

Adobe Workfront에서 관리하는 것과 유사한 방식으로 Adobe Workfront Planning에서 사용자를 독립형 제품으로 관리할 수 있습니다.

Workfront Planning에서 사용자를 할당할 수 있는 액세스 수준에는 몇 가지 제한이 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning 패키지</p></td> 
   <td> 
<p>모든 Workfront Planning을 독립형 패키지로</p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>계획 수립 관리자</p>
   </td> 
  </tr>

</tbody> 
</table>

독립 실행형 패키지로 Workfront에 필요한 액세스에 대한 자세한 내용은 [독립 실행형 제품으로 Adobe Workfront Planning에 필요한 액세스](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md)를 참조하십시오.
+++    

## Adobe Workfront Planning의 액세스 수준

독립형 제품으로 구입할 경우 Workfront Planning의 사용자에게 다음 액세스 수준을 할당할 수 있습니다.

* 계획 수립 관리자
* 계획 수립 표준

각 액세스에 포함된 기능에 대한 자세한 내용은 [독립 실행형 제품으로서 Adobe Workfront Planning에 필요한 액세스](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md)를 참조하십시오.

독립 실행형 제품으로 Workfront Planning에서 액세스 수준을 사용할 때 다음 사항을 고려하십시오.

* Workfront Planning에서는 액세스 수준을 생성하거나 수정할 수 없습니다. 사전 구성되어 있습니다.

* Adobe Admin Console에 사용자를 Workfront 제품의 관리자로 추가하면 해당 사용자는 Workfront Planning의 이 액세스 수준에 자동으로 할당되고 Planning에서 해당 액세스 수준을 편집할 수 없습니다.
* Admin Console에 사용자를 추가한 후 Planning의 사용자만 Planning Standard 액세스 레벨을 할당할 수 있습니다. 이 액세스 수준은 사용자에게 수동으로 할당할 수 있는 유일한 액세스 수준입니다.

## Workfront Planning에서 사용자를 독립 실행형 제품으로 관리

1. Planning 관리자는 다음 중 하나를 수행합니다.

   * 새로운 Workfront Planning 고객인 경우 Adobe Workfront에서 이제 Adobe Workfront에 계정이 있음을 알리는 이메일을 받게 됩니다. 이메일의 링크를 사용하여 Admin Console에 로그인합니다.

   * 기존 Workfront Planning 관리자이고 다른 사용자를 계정에 추가하려면 Admin Console에 로그인합니다.

   자세한 내용은 [Adobe Admin Console에서 사용자 관리](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md)를 참조하십시오.

1. Admin Console에서 다음 탭 중 하나에서 사용자 추가를 시작합니다.

   * **관리자**: 사용자가 Planning에서 Planning 관리자 사용자로 자동으로 만들어집니다.
   * **사용자**: Workfront Planning에서 액세스 수준을 할당해야 합니다.

1. (조건부) Adobe CX 엔터프라이즈 홈에서 Workfront에 로그인합니다.

   Workfront Planning이 열립니다.
1. **기본 메뉴** > **사용자** > **새 사용자**&#x200B;를 클릭합니다.

   ![독립 실행형 Planning의 새 사용자 상자](assets/new-user-box-planning-sta.png)

1. **새 사용자** 상자에서 다음 정보를 업데이트합니다.

   * **이름**: Admin Console에 추가한 이름과 동일한 이름.
   * **성**: Admin Console에 추가한 것과 같은 이름.
   * **전자 메일 주소(사용자 이름)**: Admin Console에 추가한 전자 메일과 동일합니다.
   * **사용자가 활성 상태입니다**: 사용자가 활성 상태이고 Workfront Planning에 로그인할 수 있으며 레코드에 할당할 수 있음을 나타내려면 설정을 켜십시오.
   * **액세스 수준**: 관리자가 아닌 사용자의 Planning Standard를 선택하십시오. 이것이 유일한 옵션입니다.

     >[!TIP]
     >
     >Admin Console에서 관리자로 이미 설정된 사용자를 추가하면 해당 사용자에 Planning 관리자 액세스 레벨이 자동으로 추가됩니다. 이 은(는) 편집할 수 없습니다.

   * **팀**: 드롭다운 메뉴에서 사용자와 연결할 팀을 선택합니다. 팀을 사용자에게 할당하려면 먼저 팀을 만들어야 합니다.

     자세한 내용은 [팀 관리](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md)를 참조하십시오.

1. **지금 업로드**&#x200B;를 클릭하여 프로필 사진을 추가한 다음 **저장**&#x200B;을 클릭합니다.

1. 사용자를 저장하고 다른 사용자를 추가하려면 **저장** 또는 **사용자 추가 및 다른 사용자 시작**&#x200B;을 클릭하세요.

   사용자가 추가되고 Workfront Planning에 로그인하기 위한 이메일을 받게 됩니다.
1. (선택 사항) 기존 사용자를 편집하려면 다음 중 하나를 수행합니다.

   * 마우스로 목록의 사용자 이름을 가리킨 다음 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png) > **사용자 편집**&#x200B;을 클릭합니다
   * 목록에서 사용자를 선택한 다음 페이지 하단의 파란색 도구 모음에서 **사용자 편집**&#x200B;을 클릭합니다.
1. (선택 사항) 사용자를 삭제하려면 다음 중 하나를 수행합니다.

   * 마우스로 목록의 사용자 이름을 가리킨 다음 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png) > **사용자 삭제**&#x200B;를 클릭합니다
   * 목록에서 팀을 선택한 다음 페이지 하단의 파란색 도구 모음에서 **사용자 삭제**&#x200B;를 클릭합니다
1. 확인하려면 **삭제**&#x200B;를 클릭하세요.
1. (선택 사항) 사용자를 비활성화하려면 다음 중 하나를 수행합니다.

   * 마우스로 목록의 사용자 이름을 가리킨 다음 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png) > **비활성화**&#x200B;를 클릭합니다
   * 목록에서 팀을 선택한 다음 페이지 하단의 파란색 도구 모음에서 **비활성화**&#x200B;를 클릭합니다
1. 확인하려면 **비활성화**&#x200B;를 클릭하세요.

   작업 기록 레코드를 유지하려면 사용자를 삭제하는 대신 비활성화하는 것이 좋습니다.



