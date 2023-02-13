---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: JumpSeat 통합 구성
description: 통합할 수 있습니다 [!DNL JumpSeat] with [!DNL Workfront] 를 클릭하여 사용자 지정, 제품 내 지침을 만듭니다.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 2f840ea68c9efb78acb4c24346c6775671ed0334
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 2%

---

# JumpSeat 통합 구성

통합할 수 있습니다 [!DNL JumpSeat] with [!DNL Workfront] 를 클릭하여 사용자 지정, 제품 내 지침을 만듭니다.

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 플랜*</strong></td> 
   <td> <p>[!UICONTROL Enterprise] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 라이센스*</strong></td> 
   <td>[!UICONTROL 계획]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>제품</strong></td> 
   <td>활성 상태여야 합니다. [!DNL JumpSeat] 계획.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p> 넌 [!DNL Workfront] 관리자 에 대한 자세한 정보 [!DNL Workfront] 관리자 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리자 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;어떤 계획, 라이센스 유형 또는 액세스 권한을 보유하고 있는지 확인하려면 [!DNL Workfront] 관리자

## 전제 조건

시작하기 전에

* 추가 및 활성화 [!DNL Workfront] 의 응용 프로그램으로 [!DNL JumpSeat]. 자세한 내용은 [응용 프로그램을 추가하거나 삭제하는 방법](https://support.jumpseat.io/article/how-to-add-an-application/).

## 구성 [!DNL JumpSeat] 통합

을 설정하는 것이 좋습니다 [!DNL JumpSeat] 미리 보기 및 프로덕션 환경에서 모두 통합.

>[!TIP]
>
>두 개의 별도 [!DNL Workfront] 응용 프로그램 [!DNL JumpSeat]- 미리보기(Preview)용 1개 및 프로덕션에 대한 1개. 자세한 내용은 [응용 프로그램을 추가하거나 삭제하는 방법](https://support.jumpseat.io/article/how-to-add-an-application/) 추가 정보.

를 구성하려면 [!DNL JumpSeat] 통합:

1. 을(를) 클릭합니다. **[!UICONTROL 기본 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리에서 [!DNL Adobe Workfront]를 클릭한 다음 **[!UICONTROL 설정]**.
1. 왼쪽 패널에서 **[!UICONTROL 시스템]** > **[!UICONTROL [!DNL JumpSeat]통합]**.
1. 을(를) 입력합니다. **[!UICONTROL [!DNL JumpSeat]URL]**.

   **예:** [!DNL https]://{mycompanyname}.jumseat.io

1. 을(를) 입력합니다. **[!UICONTROL [!DNL JumpSeat]통합 토큰]**. 여기에서 확인할 수 있습니다 **[!UICONTROL 구성]** 페이지 [!DNL JumpSeat].

   **예:** $2y$10$BevsKeQ8...OYR.LurSg2U64O

1. 클릭 **[!UICONTROL 구성 테스트]**.
1. 통합을 원하는 경우 선택합니다 **[!UICONTROL 활성]** 또는 **[!UICONTROL 비활성]**.

   >[!IMPORTANT]
   >
   >통합을 활성화하려면 5단계에서 수행된 구성 테스트가 전달되어야 합니다.

   ![JumpSeat 통합 페이지](assets/jumpseat-integration-page.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
