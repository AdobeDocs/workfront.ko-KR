---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 회사 멤버십 관리
description: 에서 [!UICONTROL 회사] 영역에서 회사 구성원을 추가하고 제거할 수 있습니다. 사용자 프로필을 편집하고 등록하도록 알림 [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront] 시스템.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# 회사 멤버십 관리

에서 [!UICONTROL 회사] 영역 [!UICONTROL 설정]를 눌러 회사 구성원을 추가하고 제거할 수 있습니다. 사용자 프로필을 편집하고 등록하도록 알림 [!DNL Workfront]을 비활성화하는 경우 [!DNL Workfront]를 제거하고 [!DNL Workfront] 시스템.

새 회사 만들기에 대한 내용은 [회사 만들기 및 편집](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

## 액세스 요구 사항

에서 회사를 관리하려면 다음 항목이 있어야 합니다 [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] 플랜*</p> </td> 
   <td>[!UICONTROL Team] 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] 라이센스*</p> </td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong> </td> 
   <td> <p>다음 중 하나를 수행합니다.</p> 
    <ul> 
     <li> <p>시스템의 회사를 편집할 수 있는 [!UICONTROL 시스템 관리자] 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>. </p> </li> 
     <li> <p>회사 관리에 대한 관리자 액세스 권한을 부여하여 시스템에서 모든 회사를 편집할 수 있습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">특정 영역에 대한 관리자 액세스 권한 부여</a>.</p> </li> 
    </ul> <p><b>메모</b>:  
     <ul> 
      <li> <p>그룹 관리자로 지정된 그룹과 연관된 회사를 관리할 수도 있습니다.</p> </li> 
      <li> <p>에 사용자를 추가하고 제거하려면 [!DNL Workfront] 시스템, 다음 중 하나가 있어야 합니다.</p> 
       <ul> 
        <li> <p>[!UICONTROL 시스템 관리자] 액세스 수준입니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>. </p> </li> 
        <li> <p>액세스 수준에서 [!UICONTROL 사용자] 설정에 대해 [!UICONTROL 편집]을 선택해야 합니다. 또한 [!UICONTROL Users] 설정의 경우 [!UICONTROL 설정 세부 조정]에서 설정을 조정합니다. <img src="assets/gear-icon-in-access-levels.png"> , [!UICONTROL 만들기] 옵션과 두 [!UICONTROL 사용자 관리] 옵션 중 하나 이상을 활성화해야 합니다. </p> <p> <img src="assets/access-req-users.png"> </p> <p>[!UICONTROL 사용자 관리(그룹 사용자)] 옵션을 사용하는 경우 사용자가 멤버인 그룹의 그룹 관리자여야 합니다.</p> </li> 
       </ul> <p>액세스 수준의 사용자 설정에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">사용자에게 액세스 권한 부여</a>.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유한 계획, 라이센스 유형 또는 액세스 수준 구성을 확인하려면 [!DNL Workfront] 관리자

## 회사 멤버십 관리

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]** ![](assets/gear-icon-settings.png).

1. 클릭 **[!UICONTROL 회사]**.
1. 회사 이름을 클릭합니다.
1. 사용 **[!UICONTROL 회사 구성원]** 왼쪽 패널에서 선택한 섹션에서 다음 중 하나를 수행합니다.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">구성원 추가</td> 
      <td> <p>클릭 <b>[!UICONTROL 멤버 추가]</b>을 선택한 다음 표시되는 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.</p> 
       <ul> 
        <li> <p><b>[!UICONTROL 새 사용자]</b>: 아직 추가되지 않은 사용자 추가 [!DNL Workfront].</p> <p>사용자 추가에 대한 정보 [!DNL Workfront]를 참조하십시오. <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">사용자 추가</a> 및 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>: 편집할 수 있는 액세스 권한이 있는 사용자를 시스템에 이미 있습니다.</p> <p><b>중요 사항</b>: 사용자가 이미 다른 회사의 멤버인 경우 새 할당은 이전 발령보다 우선합니다. 사용자는 이전 회사와 공유된 항목에 액세스할 수 없으며 이 회사와 공유된 항목에 액세스할 수 있습니다.</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>: 스프레드시트 가져오기 파일을 업로드하여 사용자를 가져옵니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">사용자 가져오기</a>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">구성원 편집</td> 
      <td> 
       <ol> 
        <li value="1"> <p>사용자를 한 명 이상 선택한 다음 [!UICONTROL 편집] 아이콘을 클릭합니다 <img src="assets/edit-icon.png"> 클릭합니다.</p> </li> 
        <li value="2"> <p>에서 옵션을 구성합니다 <b>[!UICONTROL 사용자 편집]</b> 표시되는 상자.</p> <p>이러한 옵션에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">멤버 복사</td> 
      <td> <p>기존 구성원을 복사하여 회사 구성원을 만들 수 있습니다. </p> <p><b>메모</b>:  <p>이러한 방식으로 사용자를 만들면 다음을 제외하고 원래 사용자의 모든 정보가 새로 생성된 사용자에게 복사됩니다.</p> 
        <ul> 
         <li>[!UICONTROL 개인 정보] 섹션의 정보입니다.</li> 
         <li>[!UICONTROL 로그인하면 show]: 이 상자에서 액세스 수준의 기본 랜딩 탭이 선택됩니다.</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>사용자를 선택한 다음 [!UICONTROL Copy] 아이콘을 클릭합니다 <img src="assets/copy-icon.png">. </p> </li> 
        <li value="2"> <p>에서 <b>[!UICONTROL 새 사용자]</b> 표시되는 상자에서 새 사용자가 사용할 수 있는 필드를 편집합니다.</p> <p>사용자와 연결된 모든 필드에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">사용자 프로필 편집</a>.</p> </li> 
        <li value="3"> <p>클릭 <strong>[!UICONTROL 이 사용자 추가]</strong>.</p> <p>또는</p> <p>클릭 <strong>[!UICONTROL 개인 사용자 추가 및 다른 사용자 시작]</strong> 새 사용자를 저장하고 다른 사용자를 추가하려면</p> </li> 
       </ol> <p>그러면 에서 새 계정이 만들어집니다 [!DNL Workfront] 참조하십시오.</p> <p>사용자에게 초대를 보내는 옵션을 선택한 경우 사용자는 링크를 따라 사용자를 만들 수 있는 이메일을 받게 됩니다 [!DNL Workfront] 암호.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 제거</td> 
      <td> 
       <div> 
        <p>사용자를 한 명 이상 선택하고 <b>[!UICONTROL 사용자 제거]</b>을 선택한 다음 표시되는 드롭다운 메뉴에서 다음 옵션 중 하나를 선택합니다.</p> 
        <ul> 
         <li> <p><b>[!UICONTROL 회사에서 제거]</b>: 회사에서 사용자 또는 사용자를 제거합니다.</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>: 에서 사용자 또는 사용자를 삭제합니다. [!DNL Workfront] 시스템.</p> <p><b>중요 사항</b>: 시스템에서 사용자를 삭제하면 유지할 사용자와 관련된 정보도 삭제됩니다. 사용자를 삭제하는 대신 비활성화하는 것이 좋습니다. 자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">사용자 및 해당 [!UICONTROL 업데이트] 영역에 주석을 보냅니다.</td> 
      <td> 
       <ol> 
        <li value="1"> <p>사용자를 한 명 이상 선택한 다음 [!UICONTROL Comment] 아이콘을 클릭합니다 <img src="assets/comment-icon.png"> 클릭합니다.</p> </li> 
        <li value="2"> <p>사용자에게 보낼 주석과 사용자 프로필의 [!UICONTROL 업데이트] 영역에 설명을 입력합니다.</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">회사 구성원 목록 내보내기</td> 
      <td> <p>[!UICONTROL Export] 아이콘을 클릭합니다. <img src="assets/export.png"> 도구 모음에서 내보낸 파일에 사용할 형식을 선택합니다.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">시스템의 구성원 비활성화</td> 
      <td> <p>사용자를 한 명 이상 선택하고 [!UICONTROL 자세히] 아이콘을 클릭합니다 <img src="assets/more-icon.png"> 도구 모음에서 를 선택한 다음 <b>[!UICONTROL Deactivate]</b>.</p> <p>자세한 내용은 <a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">사용자 비활성화 또는 다시 활성화</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">사용자에게 시스템에 등록하도록 알림</td> 
      <td> <p> 에서 <b>[!UICONTROL Name]</b> column, <b>[!UICONTROL Unregister]</b> 에는 등록되지 않은 각 사용자의 이름 옆에 이 표시됩니다. 이러한 사용자에게 시스템에 등록하도록 하려면 사용자를 선택하고 [!UICONTROL 자세히] 아이콘을 클릭합니다 <img src="assets/more-icon.png"> 도구 모음에서 를 선택한 다음 <b>[!UICONTROL 사용자에게 등록 알림]</b>.</p> </td> 
     </tr> 
    </tbody> 
   </table>
