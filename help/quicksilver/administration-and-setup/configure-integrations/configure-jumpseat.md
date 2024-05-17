---
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
title: JumpSeat 통합 구성
description: 다음을 통합할 수 있습니다. [!DNL JumpSeat] 포함 [!DNL Workfront] 을 사용하여 맞춤형 제품 내 지침을 제작할 수 있습니다.
feature: System Setup and Administration, Workfront Integrations and Apps
role: Admin
exl-id: 23edb48b-8cad-47be-8ace-5238a5869677
source-git-commit: 530c4451f4720a1710350f8e822e343794b63e87
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# JumpSeat 통합 구성

다음을 통합할 수 있습니다. [!DNL JumpSeat] 포함 [!DNL Workfront] 을 사용하여 맞춤형 제품 내 지침을 제작할 수 있습니다.

## 액세스 요구 사항

이 문서의 단계를 수행하려면 다음 액세스 권한이 있어야 합니다.

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
   <td>활성 상태가 있어야 합니다. [!DNL JumpSeat] 계획.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>액세스 수준 구성*</strong></td> 
   <td> <p> 다음이어야 합니다: [!DNL Workfront] 관리자. 다음에 대한 정보: [!DNL Workfront] 관리자, 참조 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">사용자에게 전체 관리 액세스 권한 부여</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유 중인 플랜, 라이선스 유형 또는 액세스 권한을 알아보려면 [!DNL Workfront] 관리자.

## 전제 조건

시작하기 전에 다음을 수행해야 합니다

* 추가 및 활성화 [!DNL Workfront] 의 애플리케이션으로 [!DNL JumpSeat]. 자세한 내용은 [응용 프로그램 추가 또는 삭제 방법](https://support.jumpseat.io/article/how-to-add-an-application/).

## 구성 [!DNL JumpSeat] 통합

다음을 설정하는 것이 좋습니다. [!DNL JumpSeat] 미리보기 및 프로덕션 환경 모두에서 통합됩니다.

>[!TIP]
>
>두 개의 별도 계정을 추가하고 활성화해야 합니다. [!DNL Workfront] 의 애플리케이션 [!DNL JumpSeat]- 미리보기 및 프로덕션용 다음을 참조하십시오 [응용 프로그램 추가 또는 삭제 방법](https://support.jumpseat.io/article/how-to-add-an-application/) 추가 정보.

을(를) 구성하려면 다음을 수행하십시오. [!DNL JumpSeat] 통합:

1. 다음을 클릭합니다. **[!UICONTROL 메인 메뉴]** 아이콘 ![](assets/main-menu-icon.png) 의 오른쪽 위 모서리 [!DNL Adobe Workfront]을 클릭한 다음 을 클릭합니다 **[!UICONTROL 설정]**.
1. 왼쪽 패널에서 **[!UICONTROL 시스템]** > **[!UICONTROL [!DNL JumpSeat]통합]**.
1. 다음을 입력하십시오. **[!UICONTROL [!DNL JumpSeat]URL]**: 의 확장 아이콘에서 찾을 수 있습니다. [!DNL JumpSeat].

   **예:** [!DNL https]://{mycompanyname}.jumpseat.io

1. 다음을 입력합니다. **[!UICONTROL [!DNL JumpSeat]통합 토큰]**. 다음에서 찾을 수 있습니다. **[!UICONTROL 구성]** 페이지 위치 [!DNL JumpSeat].

   **예:** $2y$10$BevsKeQ8....OYR.LurSg2U64O

1. 클릭 **[!UICONTROL 구성 테스트]**.
1. 통합을 원하는 경우 선택합니다. **[!UICONTROL 활성]** 또는 **[!UICONTROL 비활성]**.

   >[!IMPORTANT]
   >
   >통합을 활성화하려면 5단계에서 수행한 구성 테스트를 통과해야 합니다.

   ![JumpSeat 통합 페이지](assets/jumpseat-integration-page.png)

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.

>[!TIP]
>
>구성에 대한 자세한 내용은 [!DNL JumpSeat] 통합하려면 다음을 참조하십시오. [!DNL JumpSeat] 설명서 [JumpSeat+Workfront](https://jumpseat.io/landing-page/jumpseat-workfront/).
