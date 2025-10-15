---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 기존 증명에 대한 자동화된 워크플로 만들기 또는 편집
description: 프로세스가 복잡하거나 검토용 콘텐츠를 동일한 사용자 그룹에 정기적으로 전송하는 경우 자동화된 워크플로를 사용하면 검토 프로세스를 보다 쉽게 관리할 수 있습니다. 자동화된 워크플로로 증명을 만들 때 최종 승인까지 증명이 단계 간에 이동합니다. 참가자가 문서를 검토할 차례가 되면 알림을 받습니다.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '1142'
ht-degree: 1%

---

# 기존 증명에 대한 자동화된 워크플로 만들기 또는 편집

프로세스가 복잡하거나 검토용 콘텐츠를 동일한 사용자 그룹에 정기적으로 전송하는 경우 자동화된 워크플로를 사용하면 검토 프로세스를 보다 쉽게 관리할 수 있습니다. 자동화된 워크플로로 증명을 만들 때 최종 승인까지 증명이 단계 간에 이동합니다. 참가자가 문서를 검토할 차례가 되면 알림을 받습니다.

새 증명에 대한 자동화된 워크플로를 만드는 방법에 대한 자세한 내용은 [자동화된 워크플로를 사용하여 고급 증명 만들기](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)를 참조하십시오.

## 액세스 요구 사항

+++ 을 확장하여 이 문서의 기능에 대한 액세스 요구 사항을 봅니다.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront 패키지</td> 
   <td> <p>임의</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront 라이선스</td> 
   <td>
   <p>표준</p>
   <p>작업 또는 계획</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">교정쇄 권한 프로필 </td> 
   <td>관리자 이상</td> 
  </tr> 
  <tr> 
   <td role="rowheader">액세스 수준 구성</td> 
   <td> <p>문서에 대한 액세스 편집</p></td> 
  </tr> 
 </tbody> 
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기존 증명에 대한 자동화된 워크플로 만들기 또는 편집:

1. 문서 영역의 문서 위로 마우스를 가져간 다음 증명 워크플로 를 클릭합니다.

   또는

   증명 뷰어에서 증명을 검토하고 있는 경우 왼쪽 패널에서 **워크플로** ![워크플로 아이콘](assets/workflow-icon-proofing-viewer.png)을 클릭한 다음 편집 아이콘 ![편집 아이콘](assets/edit-icon-proofing-viewer.png)을 클릭하여 증명에 대한 자동 워크플로 설정을 엽니다.

1. (조건부) 증명이 현재 단계 없이 기본 워크플로를 사용하고 있는 경우 표시되는 화면에서 **자동화된 워크플로로 변환**&#x200B;을 클릭합니다.

   >[!NOTE]
   >
   >기본 워크플로우에서 자동화된 워크플로우로 변환할 때 첫 번째 단계를 편집할 수는 없지만 새 단계를 추가하고 구성할 수는 있습니다.

1. 조건부) Adobe Workfront 관리자가 만들고 사용자와 공유한 자동화된 워크플로 템플릿을 사용하려면 **템플릿 추가**&#x200B;를 클릭하고 나타나는 상자에서 템플릿을 선택한 다음 **템플릿 추가**&#x200B;를 클릭합니다.

   자세한 내용은 이 문서에서 [자동화된 워크플로 템플릿 사용 정보](#about-using-automated-workflow-templates)를 참조하십시오.

1. 자동화된 워크플로우에 단계 추가:

   1. 오른쪽 상단 근처에 있는 **새 단계**&#x200B;를 클릭합니다.
   1. 표시되는 상자에 스테이지의 **이름**&#x200B;을(를) 입력합니다.
   1. (선택 사항) 단계의 기한을 설정합니다.
   1. **단계 활성화** 섹션에서 단계를 활성화할 방법을 선택하십시오.


      <table>
      <tbody>
      <tr>
      <td><strong>증명 생성 시</strong></td>
      <td>증명이 이미 생성되었기 때문에 스테이지가 자동으로 활성화됩니다.</td>
      </tr>
      <tr>
      <td><strong>이전 단계 최종 기한이 지난 경우</strong></td>
      <td><strong>상위 단계</strong> 드롭다운 목록에서 이전 단계를 클릭합니다.</td>
      </tr>
      <tr>
      <td><strong>특정 날짜 및 시간에</strong></td>
      <td><strong>날짜</strong> 상자를 클릭하여 날짜를 선택한 다음 오른쪽에 있는 상자를 클릭하여 시간을 선택합니다.</td>
      </tr>
      <tr>
      <td><strong>모든 결정은 상위 단계에서 변경 사항과 함께 승인됨 또는 승인됨 상태입니다.</strong></td>
      <td><strong>상위 단계</strong> 드롭다운 목록에서 상위 단계를 클릭합니다.</td>
      </tr>
      <tr>
      <td><strong>모든 결정은 상위 단계에서 승인됩니다.</strong></td>
      <td><strong>상위 단계</strong> 드롭다운 목록에서 상위 단계를 클릭합니다.</td>
      </tr>
      <tr>
      <td><strong>모든 결정은 내려집니다.</strong></td>
      <td><strong>상위 단계</strong> 드롭다운 목록에서 상위 단계를 클릭합니다.</td>
      </tr>
      </tbody>
      </table>


   1. 연락처 이름 또는 이메일 주소를 입력하고 단계에 대한 검토자 설정을 구성합니다.

      검토자를 추가하는 방법에 대한 자세한 내용은 이 문서에서 [단계에 검토자 추가 정보](#about-adding-reviewers-to-a-stage)를 참조하십시오.

   1. 다음 옵션 중 하나를 사용하여 단계를 추가로 구성합니다.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>기한 옵션</strong> </td>
         <td><p>단계의 기한을 설정하려면 <strong>기한 옵션</strong> 드롭다운 목록에서 옵션을 클릭하십시오. <strong>기한</strong>에서 다음 중 하나를 실행하십시오.</p>
          <ul>
           <li><strong>특정 날짜 설정</strong>을 선택한 경우: 원하는 기한 날짜 및 시간을 선택하십시오.</li>
           <li><strong>단계 활성화 날짜부터 계산</strong>을 선택한 경우: 단계 활성화 날짜에 추가할 영업일 수를 선택하여 기한을 결정하십시오.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">스테이지 잠금</td>
         <td>스테이지를 잠글 수 있는 시기를 지정합니다. </td>
        </tr>
        <tr>
         <td role="rowheader">주요 의사 결정자</td>
         <td><p>단계의 기본 의사 결정자를 선택합니다(승인자 이상의 증명 역할을 가진 사용자를 단계에 하나 이상 추가한 후에만 사용 가능). 기본 의사 결정자를 선택하면 이 단계에서 <strong>필요한 하나의 의사 결정만</strong> 옵션이 비활성화됩니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">한 명의 승인만 필요</td>
         <td>의사 결정자 중 한 명이 결정을 내리면 전체 검토 프로세스를 종료합니다.<p><strong>기본 의사 결정자</strong> 드롭다운 메뉴에서 사용자를 지정한 경우에는 이 옵션을 사용할 수 없습니다.</p></td>
        </tr>
        <tr>
         <td role="rowheader">비공개 단계</td>
         <td>수퍼바이저, Adobe Workfront 관리자 및 Workfront Proof 관리자만 이 단계에서 주석 및 의사 결정을 볼 수 있습니다.</td>
        </tr>
        <tr>
         <td role="rowheader">사람들에게 이메일로 알림</td>
         <td>증명을 작업할 차례가 되면 이메일 알림으로 검토자에게 경고합니다.</td>
        </tr>
       </tbody>
      </table>

   1. **단계 추가**&#x200B;를 클릭합니다.

1. 필요에 따라 이전 단계를 반복하여 단계를 더 추가합니다.

   자동화된 워크플로에 단계를 추가하면 화면에 해당 단계를 나타내는 다이어그램 양식이 표시됩니다.

   ![워크플로 다이어그램](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. 단계를 모두 추가했으면 **완료**&#x200B;를 클릭합니다.

## 자동화된 워크플로우 템플릿 사용 정보 {#about-using-automated-workflow-templates}

자동화된 워크플로우 템플릿을 사용할 때는 다음 사항을 고려하십시오.

1. 자동화된 워크플로 템플릿의 설정은 증명에 대한 자동화된 워크플로로 수행할 수 있는 작업을 결정합니다. 예를 들어, 템플릿에서 단계 추가 버튼이 비활성화되어 있는 경우 증명에 대한 자동화된 워크플로 설정으로 작업할 때 이 버튼이 표시되지 않습니다.
1. 어떤 사람이 자동화된 워크플로 템플릿의 단계에 추가되었지만 증명에서 검토자로 이미 존재하는 경우 템플릿을 적용하면 검토자가 단계에서 제거됩니다. 스테이지에 다른 검토자를 추가하지 않으면 하나를 추가하라는 메시지가 표시됩니다.
1. 자동화된 워크플로 템플릿을 수정하는 기능은 의 설명과 같이 Workfront 관리자가 구성한 템플릿 설정에 따라 다릅니다. 템플릿 수정 기능이 비활성화된 경우 템플릿 소유자만 수정할 수 있습니다.

## 단계에 검토자 추가 정보 {#about-adding-reviewers-to-a-stage}

단계에 검토자를 추가할 때는 다음 사항을 고려하십시오.

* 단계에 사용자를 추가한 후 증명 역할 및 사용자가 보유해야 하는 추가 권한과 사람들이 증명에 대한 댓글과 결정을 내릴 때 받게 되는 이메일 경고 유형과 같은 증명에 대한 해당 사용자에 대한 설정을 구성할 수 있습니다.
* 한 스테이지에서 다른 스테이지로 한 명 이상의 사용자를 드래그할 수 있습니다. 사용자를 직접 다른 단계로 끌어 놓거나 사용자를 **단계** 다이어그램의 단계로 끌어 놓을 수 있습니다. 여러 사용자를 선택하려면 Shift+Ctrl(Windows) 또는 Shift+Command(Mac)를 누릅니다.
* 증명에 한 번만 검토자를 추가할 수 있습니다. 즉, 증명의 두 단계 이상에 동일한 사용자를 추가할 수 없습니다.
* 비공개 단계에 추가되지 않은 검토자는 해당 단계에서 수행한 증명 또는 주석에서 해당 단계를 볼 수 없습니다.
* 기본적으로 단계에 사용자를 추가하면 해당 사용자는 증명을 만든 시점부터 증명을 볼 수 있는 액세스 권한이 부여됩니다.

  Workfront 관리자는 워크플로가 사용자가 추가된 단계에 들어갈 때까지 사용자가 증명에 액세스하지 못하도록 제한할 수 있습니다. 자세한 내용은  에 있습니다.
