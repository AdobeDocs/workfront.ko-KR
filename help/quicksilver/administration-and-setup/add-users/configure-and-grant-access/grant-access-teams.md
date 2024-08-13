---
title: 팀에 액세스 권한 부여
description: Adobe Workfront 관리자는 액세스 수준을 사용하여 Workfront의 팀에 대한 사용자의 액세스 권한을 정의할 수 있습니다
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: c887569d59c7751210671cab97c492ee1752fffc
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 5%

---

# 팀에 액세스 권한 부여

Adobe Workfront 관리자는 [액세스 수준 개요](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)에 설명된 대로 액세스 수준을 사용하여 Workfront의 팀에 대한 사용자의 액세스 권한을 정의할 수 있습니다.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜</td> 
   <td>임의</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>플랜</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>Workfront 관리자여야 합니다.</p> <p><b>참고</b>: 아직 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에 추가 제한을 설정했는지 문의하세요. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">사용자 지정 액세스 수준 만들기 또는 수정</a>을 참조하십시오.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## 사용자 정의 액세스 수준을 사용하여 사용자 편집에 대한 사용자 액세스 구성

1. [사용자 지정 액세스 수준 만들기 또는 수정](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)에 설명된 대로 액세스 수준을 만들거나 편집하십시오.
1. 팀 오른쪽의 **보기** 또는 **편집** 단추에서 톱니바퀴 아이콘 ![](assets/gear-icon-settings.png)을(를) 클릭한 다음 **설정을 미세 조정**&#x200B;에서 부여할 기능을 선택합니다.

   * **보기**: 라이선스가 있는 사용자가 팀을 볼 수 있는 방법을 구성하는 경우 다음 옵션을 변경하십시오.

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">내 그룹과 관련된 팀 보기</td>
         <td>
          <p><b>사용</b>: 사용자가 미리 팀 유형 필드에 있는 팀을 찾으면 사용자는 자신이 팀원인지 여부에 관계없이 해당 그룹과 연결된 팀을 볼 수 있습니다. </p>
          <p><b>사용 안 함</b>: 사용자가 미리 팀 유형 필드에서 팀을 찾을 때 사용자는 자신이 팀원인 경우에만 해당 그룹과 연결된 팀을 볼 수 있습니다</p><p>이 옵션은 기본적으로 활성화되어 있습니다.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">모든 팀 보기</td>
         <td><p>이 옵션을 활성화하고 사용자가 팀 유형 미리 필드에서 팀을 찾으면 모든 팀을 보고 선택할 수 있습니다.</p><p>이 옵션은 기본적으로 활성화되어 있습니다. </p></td>
        </tr>
       </tbody>
      </table>

   * **편집**: 플랜 라이선스와 작업 라이선스가 있는 사용자가 팀을 관리하는 방법을 구성하는 경우 다음 옵션 중 하나를 변경하십시오.

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">만들기</td>
         <td><p>플랜 라이선스 또는 작업 라이선스가 있는 사용자가 팀을 만들 수 있도록 허용합니다.</p><p>이 옵션은 기본적으로 활성화되어 있습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">삭제</td>
         <td><p> 플랜 라이선스가 있는 사용자가 편집할 수 있는 액세스 권한이 있는 팀을 삭제할 수 있도록 허용합니다(작업 라이선스가 있는 사용자는 사용할 수 없음).</p><p>이 옵션은 기본적으로 활성화되어 있습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">내가 관리하는 그룹의 팀 편집(그룹 관리자 전용)</td>
         <td><p>그룹 관리자로 지정된 플랜 라이선스 사용자가 자신이 관리하는 그룹과 관련된 팀을 편집할 수 있도록 허용합니다.</p><p>이 옵션은 기본적으로 활성화되어 있습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">내가 속한 팀 편집</td>
         <td><p>플랜 라이선스 또는 작업 라이선스에서 사용자가 멤버인 팀을 편집할 수 있도록 허용합니다.</p><p>이 옵션은 기본적으로 비활성화되어 있습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">내 그룹과 관련된 팀 보기</td>
         <td>
         <p><b>활성화됨</b> 사용자가 미리 팀 유형 필드에 있는 팀을 찾으면 사용자가 팀원인지 여부에 관계없이 해당 그룹과 연결된 팀을 볼 수 있습니다. </p>
         <p><b>사용 안 함</b>: 사용자가 미리 팀 유형 필드에서 팀을 찾을 때 사용자는 자신이 팀원인 경우에만 해당 그룹과 연결된 팀을 볼 수 있습니다</p><p>이 옵션은 기본적으로 활성화되어 있습니다.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">모든 팀 보기</td>
         <td><p>이 옵션을 활성화하고 사용자가 팀 유형 미리 필드에서 팀을 찾으면 모든 팀을 보고 선택할 수 있습니다.</p><p>이 옵션은 기본적으로 활성화되어 있습니다. </p></td>
        </tr>
       </tbody>
      </table>

1. X를 클릭하여 **설정을 미세 조정** 상자를 닫습니다.
1. (선택 사항) 작업 중인 액세스 수준의 다른 개체 및 영역에 대한 액세스 설정을 구성하려면 [Adobe Workfront에 대한 액세스 구성](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md)에 나열된 문서 중 하나를 계속 사용하십시오(예: [작업에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) 및 [재무 데이터에 대한 액세스 권한 부여](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)).
1. 완료되면 **저장**&#x200B;을 클릭하세요.

>[!NOTE]
>
>* 다음은 액세스 수준 설정에 관계없이 true입니다.
>
>   * 팀 소유자는 항상 팀을 보고 편집할 수 있습니다.
>   * 사용자는 항상 자신이 속한 팀을 볼 수 있는 액세스 권한을 가집니다.
>
>* 액세스 수준에서 [편집] 대신 [보기] 또는 [보기] 대신 [편집]을 선택하기로 결정한 경우 보기 및 편집 모두에서 사용할 수 있는 옵션(예: &quot;내 그룹과 연결된 팀 보기&quot;)의 구성이 유지됩니다.
>

## 라이선스 유형별 팀에 액세스

각 액세스 수준의 사용자가 문제에 대해 수행할 수 있는 작업에 대한 자세한 내용은 문서 [각 개체 유형에 사용할 수 있는 기능](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md)의 [팀](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) 섹션을 참조하십시오.
