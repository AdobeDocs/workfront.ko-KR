---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 기존 증명을 위한 자동화된 워크플로우 만들기 또는 편집
description: 자동화된 워크플로우를 사용하면 프로세스가 복잡하거나 검토를 위해 컨텐츠를 동일한 사용자 그룹에 정기적으로 보내는 경우 검토 프로세스를 보다 쉽게 관리할 수 있습니다. 자동화된 워크플로우로 증명을 만들 때 증명은 스테이지에서 최종 승인까지 이동합니다. 참가자는 문서를 검토할 차례가 되면 통지됩니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 0%

---

# 기존 증명을 위한 자동화된 워크플로우 만들기 또는 편집

자동화된 워크플로우를 사용하면 프로세스가 복잡하거나 검토를 위해 컨텐츠를 동일한 사용자 그룹에 정기적으로 보내는 경우 검토 프로세스를 보다 쉽게 관리할 수 있습니다. 자동화된 워크플로우로 증명을 만들 때 증명은 스테이지에서 최종 승인까지 이동합니다. 참가자는 문서를 검토할 차례가 되면 통지됩니다.

새 증명을 위한 자동화된 워크플로우 만들기에 대한 자세한 내용은 [자동화된 워크플로우를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## 액세스 요구 사항

이 문서의 절차를 수행하려면 다음 액세스 권한이 있어야 합니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 플랜*</td> 
   <td> <p>현재 계획: Pro 이상</p> <p>또는</p> <p>기존 계획: Premium</p> <p>다양한 계획에 따른 언어 교정에 대한 자세한 내용은 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront에서 언어 교정 기능에 액세스</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스*</td> 
   <td> <p>현재 계획: 작업 또는 계획</p> <p>기존 계획: 모두(사용자가 교정을 사용하도록 설정되어 있어야 함)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">증명 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성*</td> 
   <td> <p>문서 액세스 편집</p> <p>참고: 여전히 액세스 권한이 없는 경우 Workfront 관리자에게 액세스 수준에서 추가 제한 사항을 설정하는지 문의하십시오. Workfront 관리자가 액세스 수준을 수정하는 방법에 대한 자세한 내용은 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">사용자 정의 액세스 수준 만들기 또는 수정</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;보유하고 있는 계획, 역할 또는 증명 권한 프로필을 알아보려면 Workfront 또는 Workfront 증명 관리자에게 문의하십시오.

## 기존 증명을 위한 자동화된 워크플로우 만들기 또는 편집:

1. 문서 영역에서 문서 위로 마우스를 가져간 다음 교정 워크플로우를 클릭합니다.

   또는

   교정 뷰어에서 증명을 검토하는 경우 **워크플로우** ![](assets/workflow-icon-proofing-viewer.png) 왼쪽 패널에서 편집 아이콘을 클릭합니다 ![](assets/edit-icon-proofing-viewer.png) 증명을 위한 자동화된 워크플로우 설정을 엽니다.

1. (조건부) 현재 증명의 기본 워크플로우를 사용 중인 경우(단계 없이) **자동화된 워크플로우로 변환** 표시됩니다.

   >[!NOTE]
   >
   >기본 워크플로우에서 자동화된 워크플로우로 변환하는 경우 첫 번째 단계를 편집할 수는 없지만 새 단계를 추가하고 구성할 수는 있습니다.

1. 조건부) Adobe Workfront 관리자가 만들고 사용자와 공유한 자동화된 워크플로우 템플릿을 사용하려면 을 클릭합니다 **템플릿 추가**&#x200B;을 클릭하고 표시되는 상자에서 템플릿을 선택한 다음 를 클릭합니다. **템플릿 추가**.

   자세한 내용은 [자동화된 워크플로우 템플릿 사용 정보](#about-using-automated-workflow-templates) 참조하십시오.

1. 자동 워크플로우에 스테이지 추가:

   1. 클릭 **새로운 단계** 오른쪽 상단 근처에 있습니다.
   1. 표시되는 상자에 **이름** 무대에서요
   1. (선택 사항) 스테이지의 기한을 설정합니다.
   1. 에서 **단계 활성화** 섹션에서 스테이지를 활성화할 방법을 선택합니다.


      <table>
      <tbody>
      <tr>
      <td><strong>증명 작성 시</strong></td>
      <td>증명을 이미 만들었으므로 스테이지가 자동으로 활성화됩니다.</td>
      </tr>
      <tr>
      <td><strong>이전 단계 마감일이 경과하면</strong></td>
      <td>에서 이전 단계를 클릭합니다. <strong>상위 단계</strong> 드롭다운 목록 .</td>
      </tr>
      <tr>
      <td><strong>특정 날짜 및 시간에</strong></td>
      <td>을(를) 클릭합니다. <strong>설정</strong> 상자를 클릭하여 날짜를 선택한 다음 오른쪽에 있는 상자를 클릭하여 시간을 선택합니다.</td>
      </tr>
      <tr>
      <td><strong>모든 결정은 상위 단계에서 변경 사항이 있는 승인됨 또는 승인됨 입니다</strong></td>
      <td>에서 상위 스테이지를 클릭합니다. <strong>상위 단계</strong> 드롭다운 목록.</td>
      </tr>
      <tr>
      <td><strong>모든 결정은 상위 단계에서 승인됩니다</strong></td>
      <td>에서 상위 스테이지를 클릭합니다. <strong>상위 단계</strong> 드롭다운 목록.</td>
      </tr>
      <tr>
      <td><strong>모든 결정이 내려집니다</strong></td>
      <td>에서 상위 스테이지를 클릭합니다. <strong>상위 단계</strong> 드롭다운 목록.</td>
      </tr>
      </tbody>
      </table>


   1. 연락처 이름 또는 전자 메일 주소를 입력하고 스테이지의 검토자에 대한 설정을 구성합니다.

      검토자 추가에 대한 자세한 내용은 [스테이지에 검토자 추가 정보](#about-adding-reviewers-to-a-stage) 참조하십시오.

   1. 다음 옵션 중 하나를 사용하여 스테이지를 추가로 구성합니다.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>최종 기한 옵션</strong> </td>
         <td><p>스테이지의 기한을 설정하려면 <strong>최종 기한 옵션</strong> 드롭다운 목록. 그런 다음 <strong>기한</strong>다음 중 하나를 수행합니다.</p>
          <ul>
           <li>선택한 경우 <strong>특정 날짜 설정</strong>: 원하는 마감 날짜 및 시간을 선택합니다.</li>
           <li>선택한 경우 <strong>단계 활성화 날짜에서 계산</strong>: 단계 활성화 날짜에 추가할 비즈니스 일수를 선택하여 마감일을 결정합니다.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">스테이지 잠금</td>
         <td>스테이지를 잠글 수 있는 시기를 지정합니다. </td>
        </tr>
        <tr>
         <td role="rowheader">주요 의사 결정자</td>
         <td><p>스테이지에서 기본 의사 결정자를 선택합니다(승인자 이상의 증명 역할이 있는 단계에 한 명 이상의 사람을 추가한 후에만 사용 가능). 1차 결정자를 선택하면 <strong>한 가지 결정만 필요합니다</strong> 이 단계에서 옵션을 사용할 수 없습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">필요한 결정은 단 하나입니다.</td>
         <td>의사 결정권자 중 한 명이 결정을 내리면 전체 검토 프로세스를 종료합니다.<p>에서 사용자를 지정한 경우에는 이 옵션을 사용할 수 없습니다 <strong>주요 의사 결정권자</strong> 드롭다운 메뉴</p></td>
        </tr>
        <tr>
         <td role="rowheader">비공개 단계</td>
         <td>다음 사용자만 이 단계 동안 수행된 댓글 및 결정을 볼 수 있습니다. 감독, Adobe Workfront 관리자 및 Workfront 증명 관리자</td>
        </tr>
        <tr>
         <td role="rowheader">전자 메일로 사람들에게 알림</td>
         <td>증명에서 작업할 때 검토자에게 이메일 알림을 보냅니다.</td>
        </tr>
       </tbody>
      </table>

   1. 클릭 **단계 추가**.

1. 단계를 더 추가하려면 필요한 경우 이전 단계를 반복합니다.

   자동화된 워크플로우에 단계를 추가하면 화면에 다이어그램 양식이 표시됩니다.

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. 단계 추가를 마치면 를 클릭합니다 **완료**.

## 자동화된 워크플로우 템플릿 사용 정보 {#about-using-automated-workflow-templates}

자동화된 워크플로우 템플릿을 사용할 때는 다음 사항을 고려하십시오.

1. 자동화된 워크플로우 템플릿의 설정은 증명을 위해 자동화된 워크플로우를 사용하여 수행할 수 있는 작업을 결정합니다. 예를 들어 템플릿에서 스테이지 추가 단추가 비활성화된 경우 증명의 자동화된 워크플로우 설정을 사용하여 작업할 때에는 표시되지 않습니다.
1. 사용자가 자동화된 워크플로우 템플릿의 용지에 추가되지만, 증명에 검토자로 이미 있으면 템플릿을 적용하면 검토자가 스테이지에서 제거됩니다. 스테이지에 다른 검토자를 추가하지 않으면 메시지를 통해 검토자를 추가하라는 메시지가 표시됩니다.
1. 자동화된 워크플로우 템플릿을 수정하는 기능은 에 설명된 대로 Workfront 관리자가 구성한 템플릿 설정에 따라 다릅니다. 템플릿을 수정하는 기능이 비활성화되어 있으면 템플릿 소유자만 수정할 수 있습니다.

## 스테이지에 검토자 추가 정보 {#about-adding-reviewers-to-a-stage}

스테이지에 검토자를 추가할 때는 다음 사항을 고려하십시오.

* 사용자를 스테이지에 추가한 후에는 증명 역할과 권한이 있어야 하는 모든 추가 권한 및 사람들이 증명에 대한 댓글 및 결정을 할 때 받게 될 이메일 경고 유형과 같은 증명의 해당 사용자에 대한 설정을 구성할 수 있습니다.
* 한 단계에서 다른 스테이지로 하나 이상의 사용자를 드래그할 수 있습니다. 사용자를 다른 스테이지로 직접 드래그하거나 사용자를 스테이지로 드래그할 수 있습니다 **단계** 다이어그램. 여러 사용자를 선택하려면 Shift+Ctrl(Windows의 경우) 또는 Shift+Command(Mac의 경우)를 누릅니다.
* 한 번만 검토자를 증표에 추가할 수 있습니다. 이는 동일한 사람을 증명의 두 단계 이상에 추가할 수 없음을 의미합니다.
* 비공개 단계에 추가되지 않은 검토자는 해당 단계에서 작성한 증명 또는 댓글에 해당 단계를 볼 수 없습니다.
* 기본적으로 스테이지에 사용자를 추가하면 사용자가 증명을 만들 때부터 증명을 볼 수 있는 액세스 권한을 부여합니다.

   Workfront 관리자는 워크플로우가 사용자가 추가된 단계에 들어갈 때까지 사용자에게 증명 액세스를 제한할 수 있습니다. 자세한 내용은 의 를 참조하십시오.
