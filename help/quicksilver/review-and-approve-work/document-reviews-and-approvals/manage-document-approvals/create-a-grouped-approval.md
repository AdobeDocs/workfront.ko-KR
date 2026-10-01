---
product-area: documents
navigation-topic: approvals
title: 그룹화된 승인 만들기
description: 여러 에셋을 단일 승인 워크플로로 번들로 묶어 동일한 단계를 함께 진행할 수 있습니다.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: f55042154ac3d93544c152b7b1ad26746a209772
workflow-type: tm+mt
source-wordcount: '1173'
ht-degree: 1%
---

# 그룹화된 승인 만들기

<span class="preview">Frame.io 통합을 사용할 수 없으므로 미리 보기 샌드박스 환경에서 이 페이지의 정보를 사용할 수 없습니다. 이 기능은 2026년 10월 14일과 15일에 프로덕션 환경에서 사용할 수 있습니다.</span>

그룹화된 승인은 단일 승인 작업 과정 아래에 여러 자산을 번들로 묶습니다. 단일 자산 승인과 마찬가지로 그룹화된 승인이 있는 기본 및 고급 모드, 여러 단계 및 병렬 경로를 사용할 수 있습니다.

그룹화된 승인은 조직이 Adobe 클라우드 스토리지를 사용할 때 표시되는 새 문서 영역에서만 사용할 수 있습니다. 자세한 내용은 [Adobe 클라우드 저장소 개요](/help/quicksilver/review-and-approve-work/esm-overview.md)를 참조하십시오.

## 액세스 요구 사항

+++ 이 문서의 기능에 대한 액세스 요구 사항을 보려면 확장하십시오.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront 패키지</td>
   <td> <p>Adobe 클라우드 스토리지를 사용하여 승인을 관리하는 모든 워크플로우 패키지</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront 라이선스</td>
   <td>
   <p>기여자 이상</p>
   <p>검토 이상</p>
   <p>Adobe 클라우드 스토리지를 사용하는 오브젝트의 경우 표준 라이선스가 있어야 승인 워크플로우를 만들 수 있습니다.</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">액세스 수준 구성</td>
   <td> <p>프로젝트, 작업, 문제, 템플릿, 포트폴리오, 프로그램, 보고서, 대시보드, 캘린더 및 문서에 대한 보기 또는 상위 액세스 권한</p></td>
  </tr>
  <tr>
   <td role="rowheader">개체 권한</td>
   <td> <p>요청 또는 승인과 연관된 오브젝트에 대한 액세스 관리</p></td>
  </tr>
 </tbody>
</table>

자세한 내용은 [Workfront 설명서의 액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 기본적인 그룹 승인 만들기

단일 단계 그룹 승인을 만들려면 다음 작업을 수행하십시오.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.

1. 포함할 첫 번째 에셋을 클릭한 다음 Shift 키를 누른 상태에서 추가 에셋을 클릭하여 여러 에셋을 선택합니다.

1. 자산을 선택한 상태에서 하단 메뉴에서 **승인 요청**&#x200B;을 클릭합니다. **승인 요청** 대화 상자가 기본 모드에서 열립니다.

   ![그룹화된 승인 만들기](assets/requeset-grouped-approval.png)

1. 다음 세부 정보를 입력합니다.

   <table>
   <tr>
   <td><strong>승인 템플릿 사용(선택 사항)</strong></td>
   <td>템플릿 필드는 기본적으로 축소됩니다. 필드를 클릭하여 확장한 다음 드롭다운 메뉴에서 템플릿을 선택합니다. 템플릿에 하나의 경로와 스테이지가 있는 경우 기본 모드에서 적용됩니다. 템플릿에 둘 이상의 스테이지 또는 경로가 있는 경우 대화 상자가 자동으로 고급 모드로 전환되고 기본 모드에서 입력한 모든 입력은 템플릿의 콘텐츠로 대체됩니다.</td>
   </tr>
   <tr>
   <td><strong>미리 보기에 사람 또는 팀 추가</strong></td>
   <td><p>사용자 이름, 팀 또는 전자 메일 주소를 입력한 다음 <strong>승인자</strong> 또는 <strong>검토자</strong>인지 선택하세요. Workfront은 팀의 각 활성 멤버를 개별적으로 추가합니다.</p>
   <p>참고: 사용자가 이미 추가되었거나 사용자가 추가하는 둘 이상의 팀에 속해 있는 경우 한 번 포함됩니다.</p></td>
   </tr>
   <tr>
   <td><strong>필요한 결정은 단 하나입니다(선택 사항).</strong></td>
   <td>가장 먼저 결정을 내리는 사람이 단계를 완료합니다.</td>
   </tr>
   <tr>
   <td><strong>기한(선택 사항)</strong></td>
   <td>승인에 대한 기한을 설정하십시오. 사용자에게 이메일로 72시간이 통지된 후 지정된 기한 24시간 전에 통지됩니다.</td>
   </tr>
   <tr>
   <td><strong>사용자 지정 메시지 추가(선택 사항)</strong></td>
   <td><strong>사용자 지정 메시지 추가</strong> 텍스트 상자에 메시지를 입력하십시오. 이 메시지는 승인 이메일 알림과 Workfront의 승인 탭에 표시됩니다.</td>
   </tr>
   </table>

1. (선택 사항) **문서** 탭을 클릭하여 이 승인에 포함된 자산을 검토합니다.

1. **승인 요청**&#x200B;을 클릭합니다.

   ![기본 그룹 승인](assets/basic-group-approval.png)

## 고급 그룹 승인 만들기

고급 모드는 병렬 경로를 지원합니다. 각 경로는 독립적으로 실행되며 하나 이상의 순차적 단계를 포함합니다. 단계의 모든 필수 결정이 내려지면 해당 경로의 다음 단계가 시작되고 이전 단계가 잠기며 새 단계의 검토자 및 승인자가 이메일 알림을 받습니다.

작업 필요 결정은 해당 경로가 속한 경로를 중지하지만 다른 경로의 승인 워크플로에는 영향을 주지 않습니다.

<!--
You can configure up to 30 paths and 100 stages total.
-->

고급 그룹 승인을 만들려면 다음 작업을 수행하십시오.

1. 문서가 포함된 프로젝트, 작업 또는 문제로 이동한 다음 왼쪽 패널에서 **문서**&#x200B;을(를) 선택합니다.

1. 포함할 첫 번째 에셋을 클릭한 다음 Shift 키를 누른 상태에서 추가 에셋을 클릭하여 여러 에셋을 선택합니다.

1. 자산을 선택한 상태에서 하단 메뉴에서 **승인 요청**&#x200B;을 클릭합니다.

   ![그룹화된 승인 만들기](assets/requeset-grouped-approval.png)

1. **승인 요청** 대화 상자의 오른쪽 상단에서 **고급으로 이동**&#x200B;을 클릭합니다. 기본 모드로 입력한 모든 입력이 유지되어 **경로 1**, **단계 1**&#x200B;에 적용됩니다.

   >[!TIP]
   >
   >승인을 만드는 동안 오른쪽 상단의 **기본 모드로 이동**&#x200B;을 클릭하여 기본 모드로 돌아갈 수 있습니다. 승인 요청을 제출하면 **기본으로 이동** 옵션을 더 이상 사용할 수 없습니다.

1. 경로 1의 단계 1에 대한 세부 정보 입력:

   <table>
   <tr>
   <td><strong>단계 이름</strong></td>
   <td>단계 이름은 기본적으로 <em>단계 1</em>, <em>단계 2</em> 등으로 지정됩니다. <em>초기 검토</em> 또는 <em>최종 승인</em>과 같이 보다 설명적인 단계로 단계 이름을 바꾸십시오.</td>
   </tr>
   <tr>
   <td><strong>미리 보기에 사람 또는 팀 추가</strong></td>
   <td><p>사용자 이름, 팀 또는 전자 메일 주소를 입력한 다음 <strong>승인자</strong> 또는 <strong>검토자</strong>인지 선택하세요. Workfront은 팀의 각 활성 멤버를 개별적으로 추가합니다.</p>
   <p>참고: 사용자가 이미 추가되었거나 사용자가 추가하는 둘 이상의 팀에 속해 있는 경우 한 번 포함됩니다.</p></td>
   </tr>
   <tr>
   <td><strong>필요한 결정은 단 하나입니다(선택 사항).</strong></td>
   <td>가장 먼저 결정을 내리는 사람이 단계를 완료합니다.</td>
   </tr>
   <tr>
   <td><strong>기한(선택 사항)</strong></td>
   <td>각 경로의 첫 번째 단계는 절대 기한을 지원합니다. 경로의 후속 각 단계는 상대적 기한(해당 단계가 열린 날짜로부터 경과된 일 수)을 지원합니다. 사용자에게 72시간 전에 이메일로 알린 후 기한으로부터 24시간 전에 알려 줍니다.</td>
   </tr>
   <tr>
   <td><strong>사용자 지정 메시지 추가(선택 사항)</strong></td>
   <td><strong>사용자 지정 메시지 추가</strong> 텍스트 상자에 메시지를 입력하십시오. 이 메시지는 승인 이메일 알림과 Workfront의 승인 탭에 표시됩니다.<p>두 번째 단계를 추가하면 기본적으로 <strong>모든 단계에서 이 메시지 표시</strong>가 선택됩니다. 모든 단계에서 동일한 메시지를 사용하도록 선택한 상태로 둡니다. 각 단계에 대해 다른 메시지를 사용하려면 <strong>모든 단계에서 이 메시지 표시</strong>의 선택을 취소한 다음 각 단계의 <strong>사용자 지정 메시지 추가</strong> 텍스트 상자에 단계별 메시지를 입력하십시오.</p></td>
   </tr>
   </table>

1. (선택 사항) 경로 1에 단계를 더 추가합니다.
   1. 현재 경로에 다른 단계를 추가하려면 **단계 추가**&#x200B;를 클릭하십시오. 경로 내의 단계는 나열된 순서대로 순차적으로 실행됩니다.
   1. 새 단계에 대한 세부 사항을 입력한 다음 이 단계를 반복하여 필요에 따라 단계를 더 추가합니다.

      >[!NOTE]
      >
      >한 경로에서 다른 경로로 단계를 이동할 수는 없지만 경로 내의 단계를 재정렬할 수는 있습니다. 각 경로에는 서로 다른 스테이지 수가 있을 수 있습니다.


1. (선택 사항) 병렬 경로를 추가합니다.
   1. 화면 왼쪽의 **병렬 경로**&#x200B;에서 **경로 추가**&#x200B;를 클릭하여 다른 경로를 추가합니다.
   1. 동일한 단계에 따라 단계와 참가자를 새 경로에 추가합니다. 각 경로는 독립적으로 실행되므로 각 경로의 단계 수와 참여자가 다를 수 있습니다.

1. (선택 사항) 경로를 제거하려면 경로 레이블을 마우스로 가리키고 휴지통 아이콘을 클릭합니다. **경로 1**&#x200B;을(를) 제거할 수 없으며 경로의 순서를 변경할 수 없습니다. 경로 내의 스테이지가 잠겨 있지 않거나 완료된 경우에만 다른 경로를 제거할 수 있습니다.

1. (선택 사항) 모든 경로와 단계를 지우고 다시 시작하려면 오른쪽 상단 모서리에서 **재설정**&#x200B;을 클릭합니다.

1. (선택 사항) **문서** 탭을 클릭하여 이 승인에 포함된 자산을 검토합니다.

1. **승인 요청**&#x200B;을 클릭합니다.

   ![고급 그룹 승인](assets/advanced-group-approval.png)


<!--

## Add additional documents to a grouped approval

You can add additional documents to a grouped approval after the approval has been created as long as the first stage has not been completed. 

To add an additional document to a grouped approval:

1. Click any document in the grouped approval, then click **Manage Approval** in the bottom menu.
1. Click **Documents on this approval**, then click **Add**.

   ![add document grouped approval](assets/add-document-to-grouped-approval.png)
1. Choose the documents you want to add, then click **Add to approval**. 
1. Once you add all of the documents, click **Edit approval**. The new documents are added to the grouped approval and all participants are notified of the change.

-->

## 알려진 제한 사항

* 현재, 만든 후에는 그룹화된 승인 워크플로에서 문서를 추가하거나 제거할 수 없습니다. 이 기능은 향후 릴리스에서 제공될 예정입니다.
* 그룹화된 승인은 일시적으로 그룹당 3개의 경로 및 25개의 자산으로 제한됩니다.