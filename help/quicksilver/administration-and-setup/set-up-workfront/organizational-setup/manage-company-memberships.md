---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 회사 멤버십 관리
description: 설정의 [!UICONTROL 회사] 영역에서 회사 구성원을 추가하고 제거할 수 있습니다. 사용자 프로필을 편집하여  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] 시스템에 등록하도록 상기할 수도 있습니다.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '839'
ht-degree: 1%

---

# 회사 멤버십 관리

[!UICONTROL 설정]의 [!UICONTROL 회사] 영역에서 회사 구성원을 추가하고 제거할 수 있습니다. 사용자 프로필을 편집하여 [!DNL Workfront]에 등록하도록 알리고, [!DNL Workfront]에서 비활성화하고, [!DNL Workfront] 시스템에서 제거할 수도 있습니다.

새 회사 만들기에 대한 자세한 내용은 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)을 참조하세요.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto">
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] 패키지</p> </td> 
   <td><p>임의</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] 라이센스</p> </td> 
   <td><p>[!UICONTROL 계획]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr>
  <tr> 
   <td>액세스 수준 구성</td> 
  <td> <p>다음 중 하나가 있어야 합니다.</p> 
    <ul> 
     <li> <p>시스템에서 회사를 편집할 수 있는 [!UICONTROL 시스템 관리자] 액세스 수준입니다.</p> </li> 
     <li> <p>회사 관리에 대한 관리 액세스 권한으로, 시스템에서 모든 회사를 편집할 수 있습니다.</p> </li> 
    </ul> <p><b>참고</b>:  
     <ul> 
      <li> <p>그룹 관리자로 할당된 모든 그룹과 연결된 회사를 관리할 수도 있습니다.</p> </li> 
      <li> <p>[!DNL Workfront] 시스템에서 사용자를 추가하고 제거하려면 다음 중 하나가 있어야 합니다.</p> 
       <ul> 
        <li> <p>[!UICONTROL 시스템 관리자] 액세스 수준입니다. </p> </li> 
        <li> <p>액세스 수준의 <b>[!UICONTROL 사용자]</b> 설정이 <b>[!UICONTROL 편집]</b> 액세스로 구성되었으며, <b>[!UICONTROL 만들기]</b>와(과) <b>[!UICONTROL 사용자 관리]</b> <b>에서 두 개의 </b>[!UICONTROL 사용자 관리]<img src="assets/gear-icon-in-access-levels.png"> 옵션 중 하나 이상을 사용할 수 있습니다. </p> <p> <img src="assets/access-req-users.png"> </p> <p>이 두 옵션 중 <b>[!UICONTROL 사용자 관리자(그룹 사용자)]</b>이(가) 활성화된 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td>
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 회사 멤버십 관리

{{step-1-to-setup}}

1. **[!UICONTROL 회사]**&#x200B;를 클릭합니다.
1. 회사 이름을 클릭합니다.
1. 왼쪽 패널에서 **[!UICONTROL 회사 구성원]**&#x200B;을 클릭합니다.
1. 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">구성원 추가</td> 
      <td> <p><b>[!UICONTROL 멤버 추가]</b>를 클릭한 다음 표시되는 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.</p> 
       <ul> 
        <li> <p><b>[!UICONTROL 새 사용자]</b>: [!DNL Workfront]에 아직 추가되지 않은 사용자를 추가합니다.</p> <p>[!DNL Workfront]에 사용자를 추가하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">사용자 추가</a> 및 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>을 참조하십시오.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: 편집할 수 있는 액세스 권한이 있는 기존 사용자를 시스템에 추가합니다.</p> <p><b>중요</b>: 사용자가 이미 다른 회사의 구성원인 경우 새 할당이 이전 할당보다 우선합니다. 사용자는 이전 회사와 공유한 항목에 대한 액세스 권한을 상실하고 이 회사와 공유한 항목에 대한 액세스 권한을 갖게 됩니다.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>: 스프레드시트 가져오기 파일을 업로드하여 사용자를 가져옵니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">사용자 가져오기</a>를 참조하십시오.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">구성원 편집</td> 
      <td> 
       <ol> 
        <li value="1"> <p>사용자를 한 명 이상 선택한 다음 도구 모음에서 [!UICONTROL 편집] 아이콘 <img src="assets/edit-icon.png">을(를) 클릭합니다.</p> </li> 
        <li value="2"> <p>표시되는 <b>[!UICONTROL 사용자 편집]</b> 상자에서 옵션을 구성합니다.</p> <p>이러한 옵션에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>을 참조하십시오.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">멤버 복사</td> 
      <td> <p>기존 구성원을 복사하여 회사 구성원을 생성할 수 있습니다. </p> <p><b>참고</b>:  <p>이러한 방식으로 사용자를 생성하면 다음을 제외한 모든 정보가 원래 사용자의 새 생성 사용자에게 복사됩니다.</p> 
        <ul> 
         <li>[!UICONTROL 개인 정보] 섹션의 정보입니다.</li> 
         <li>[!UICONTROL 로그인할 때 표시]: 이 상자에서 액세스 수준에 대한 기본 랜딩 탭이 선택됩니다.</li> 
         <li>[!UICONTROL 직접 보고서]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>사용자를 선택한 다음 [!UICONTROL Copy] 아이콘 <img src="assets/copy-icon.png">을(를) 클릭합니다. </p> </li> 
        <li value="2"> <p>표시되는 <b>[!UICONTROL 새 사용자]</b> 상자에서 새 사용자가 사용할 수 있는 필드를 편집합니다.</p> <p>사용자와 관련된 모든 필드에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>을 참조하세요.</p> </li> 
        <li value="3"> <p><strong>[!UICONTROL 이 사용자 추가]</strong>를 클릭합니다.</p> <p>또는</p> <p>새 사용자를 저장하고 다른 사용자를 추가하려면 <strong>[!UICONTROL 사용자 추가 및 다른 사용자 시작]</strong>을(를) 클릭합니다.</p> </li> 
       </ol> <p>[!DNL Workfront]에서 사용자의 새 계정을 만듭니다.</p> <p>사용자에게 초대를 보내는 옵션을 선택한 경우 해당 사용자는 링크를 따라 [!DNL Workfront] 암호를 만들 수 있는 전자 메일을 받게 됩니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 제거</td> 
      <td> 
       <div> 
        <p>사용자를 한 명 이상 선택하고 <b>[!UICONTROL 사용자 제거]</b>를 클릭한 다음 표시되는 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL 회사에서 제거]</b>: 회사에서 사용자를 제거합니다.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: [!DNL Workfront] 시스템에서 사용자를 삭제합니다.</p> <p><b>중요</b>: 시스템에서 사용자를 삭제하면 유지할 사용자와 관련된 정보도 삭제됩니다. 사용자를 삭제하는 대신 비활성화하는 것이 좋습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>를 참조하십시오.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 및 [!UICONTROL 업데이트] 영역에 주석 보내기</td> 
      <td> 
       <ol> 
        <li value="1"> <p>사용자를 한 명 이상 선택한 다음 도구 모음에서 <b>사용자에게 업데이트 보내기</b>를 클릭합니다.</p> </li> 
        <li value="2"> <p>사용자 및 해당 사용자 프로필의 [!UICONTROL 업데이트] 영역에 보낼 설명을 입력합니다.</p>
         <p>자세한 내용은 <a href="/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md">다른 사용자에게 다이렉트 메시지 보내기</a>를 참조하십시오.</p></li> 
       </ol>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">회사 구성원 목록 내보내기</td> 
      <td> <p>도구 모음에서 [!UICONTROL 내보내기] 아이콘 <img src="assets/export.png">을(를) 클릭한 다음 내보낸 파일에 사용할 형식을 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">시스템에서 멤버 비활성화</td> 
      <td> <p>사용자를 한 명 이상 선택하고 도구 모음에서 [!UICONTROL More] 아이콘 <img src="assets/more-icon.png">을(를) 클릭한 다음 <b>[!UICONTROL Deactivate]</b>을(를) 선택합니다.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>를 참조하십시오.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">사용자에게 시스템에 등록하도록 알림</td> 
      <td> <p> <b>[!UICONTROL 이름]</b> 열에서 <b>[!UICONTROL 등록되지 않음]</b>이(가) 등록되지 않은 각 사용자의 이름 옆에 표시됩니다. 이러한 사용자에게 시스템에 등록하도록 알리려면 사용자를 선택하고 도구 모음에서 [!UICONTROL 자세히] 아이콘 <img src="assets/more-icon.png">을(를) 클릭한 다음 <b>[!UICONTROL 사용자에게 등록하도록 알림]</b>을(를) 선택합니다.</p> </td> 
     </tr> 
    </tbody> 
   </table>
