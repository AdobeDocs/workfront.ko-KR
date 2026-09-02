---
title: 레코드 유형 비즈니스 규칙 구성
description: 필드 값에 따라 레코드에 특정 작업을 적용할 수 있는 레코드 유형 비즈니스 규칙을 구성할 수 있습니다.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 757cbfd2ae74da7a649bee4d93da862d986ee5a2
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 1%

---


# 레코드 유형 비즈니스 규칙 구성

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Adobe Workfront Planning 레코드 유형에 대한 비즈니스 규칙을 구성하여 해당 유형의 레코드에 대한 작업이 허용되거나 금지되기 전에 특정 필드가 필요함을 나타낼 수 있습니다.

규칙 작성 방법에 따라 정의된 비즈니스 규칙이 충족되는 경우 레코드에 대해 다음 작업을 허용할 수 있습니다.

* 레코드 편집 또는 편집 안 함
* 레코드 삭제 또는 삭제 안 함

## 액세스 요구 사항

+++ 을 확장하여 액세스 요구 사항을 보고 이 문서의 단계를 수행하십시오.  

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
   <td role="rowheader"><p>Adobe Workfront 패키지</p></td> 
   <td> 
<ul> 
<li><p>Planning 패키지가 있는 모든 Workfront 또는 워크플로우</p></li>
또는
<li><p>독립 실행형 제품으로 구입할 경우 모든 Planning 패키지</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Adobe Workfront 라이선스</p></td> 
   <td><p>워크플로우 표준</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Adobe Planning 라이선스</p></td> 
   <td><p>계획 수립 표준</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>액세스 수준 구성</p></td> 
   <td> <p>워크플로우와 Planning 패키지가 모두 있는 경우 액세스 레벨에 워크플로우와 Planning 라이선스 유형을 모두 추가해야 합니다.</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>개체 권한</p></td> 
   <td>   <p>작업 공간 및 레코드 유형에 대한 권한 관리</p>  
   <p>시스템 관리자는 만들지 않은 작업 영역을 포함하여 모든 작업 영역에 대한 권한을 가집니다</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfront 액세스 요구 사항에 대한 자세한 내용은 Workfront 설명서의 [액세스 요구 사항](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)을 참조하십시오.

+++

## 비즈니스 규칙 구성 시 고려 사항

* 비즈니스 규칙은 필드 변경 또는 레코드 삭제에 조건을 첨부합니다. 규칙은 필드가 규칙에서 구성하는 필드 값으로 변경되려고 할 때라는 한 가지 특정 의도적인 순간에만 실행됩니다.

* 규칙은 일반 언어로 다음과 같습니다. &quot;이 레코드를 편집하려면 먼저 캠페인 요약 필드에 값이 있어야 합니다.&quot;

  필드가 비어 있으면 레코드 편집이 차단되고 앞으로 진행하기 전에 해결해야 하는 사항을 설명하는 명확한 메시지가 표시됩니다. 필수 필드를 업데이트하고 다시 시도하면 변경이 허용됩니다.

* 규칙은 기록 생성을 차단하지 않습니다. 사용자는 여전히 레코드를 만들 수 있지만 필수 필드가 비어 있거나 지정된 값이 포함되어 있지 않은지 확인해야 합니다.
* 규칙은 레코드를 자동으로 편집하거나 삭제하지 않습니다. 변경은 사용자가 신중하고 트리거해야 합니다.
* 규칙은 소급 적용되지 않습니다. 이전 레코드는 영향을 받지 않습니다. 규칙 검사는 다음에 누군가가 레코드를 편집하거나 삭제하려고 할 때만 실행됩니다.
* 기본 또는 보조 작업 영역의 글로벌 레코드 유형에 비즈니스 규칙을 추가할 수 없습니다.
* 다음을 제외한 모든 필드 유형을 참조하는 비즈니스 규칙에 대한 조건을 만들 수 있습니다.
  * 공식 필드
  * 조회 필드
  * 참조 필드
* 규칙은 레코드를 편집하거나 삭제할 수 있는 모든 사용자에게 적용됩니다.
* 레코드 유형에 대해 둘 이상의 비즈니스 규칙을 가질 수 있습니다.  <!--Syuzanna is checking this because it should be just ONE rule per action: one per edit and one per delete - see this: https://workfront.slack.com/archives/C0BHWEUSJCU/p1788281638322049?thread_ts=1787924876.280359&cid=C0BHWEUSJCU-->

  모든 규칙이 동시에 확인되며 오류 메시지에 한 명령문에서 누락된 모든 필드가 표시됩니다.

## 비즈니스 규칙 구성

1. 레코드 유형 페이지로 이동합니다.
1. 모든 보기에서 레코드 종류 이름의 오른쪽에 있는 **기타** 메뉴 ![기타 메뉴](assets/more-menu.png)를 클릭한 다음 **비즈니스 규칙**&#x200B;을 클릭합니다.

   비즈니스 규칙 페이지가 열립니다.
1. **새 비즈니스 규칙**&#x200B;을 클릭합니다.
1. **새 비즈니스** 규칙 상자에서 사용 가능한 첫 번째 필드에 비즈니스 규칙의 이름을 추가합니다. 필수 필드입니다.
1. (선택 사항) 비즈니스 규칙을 정의하는 설명을 추가한 다음 **저장**&#x200B;을 클릭합니다.
1. 비즈니스 규칙 설정 양식의 **If** 섹션에서 특정 규칙에 따라 제한하거나 허용할 작업을 선택합니다. 다음 중 선택: <!--check UI text-->
   * **레코드 편집**: 이 규칙에 정의된 조건이 충족되면 사용자는 레코드를 편집하거나 편집할 수 없습니다.
   * **레코드 삭제**: 이 규칙에 정의된 조건이 충족되면 사용자는 레코드를 삭제하거나 삭제하지 않을 수 있습니다.
     <!--add screen shot when UI text is final-->
1. **수식 필드**&#x200B;에서 비즈니스 규칙을 추가합니다. 오른쪽 패널의 **수식 표현식** 섹션에서 규칙에 대한 연산자를 선택하십시오.

   예를 들어 **기타** 필드 섹션에서 **IF**&#x200B;을(를) 선택하거나 &quot;IF&quot;를 입력한 다음 제안 목록에 표시될 때 클릭할 수 있습니다.

   >[!TIP]
   >
   >규칙 구문을 올바르게 유지하려면 제안 목록에서 필드와 연산자를 선택하는 것이 좋습니다.
1. 이 레코드 유형의 레코드를 편집하거나 삭제할 수 있도록 필수로 지정할 및 필드를 선택합니다.

   예를 들어 다음 문을 입력하여 **캠페인 요약** 필드를 필수 항목으로 만들 수 있습니다.

   ```
      IF(ISBLANK({Campaign summary}),"Campaign summary is a required field. You cannot edit this record without a value for the Campaign summary.")
   ```

   >[!IMPORTANT]
   >
   >사용자가 레코드에서 수행하려는 작업이 허용되지 않는 경우를 사용자가 쉽게 이해할 수 있도록 다음 정보를 규칙 공식에 포함하는 것이 좋습니다.
   >
   >* 규칙이 설정된 정확한 필드.
   >* 규칙이 충족되지 않는 경우의 정확한 결과.

   필드 또는 식이 잘못된 경우 **수식** 필드에 표시기가 있습니다.  <!--add screen shot?-->

   비즈니스 규칙의 **Then** 섹션에서 규칙의 기능에 대한 설명을 볼 수 있습니다.

1. 이 레코드 종류에 대해 규칙을 활성화하려면 **활성화**&#x200B;를 클릭한 다음 **저장**&#x200B;을 클릭합니다.

   규칙은 활성화 즉시 적용되며 선택한 레코드 유형의 레코드를 편집하거나 삭제할 권한이 있는 모든 사용자가 따라야 합니다.
1. (선택 사항 및 권장) 페이지 헤더의 **비즈니스 규칙** 왼쪽에 있는 뒤로 화살표를 클릭하여 레코드 유형 페이지를 표시하고 테이블 보기로 이동하거나 레코드의 페이지를 연 다음 레코드를 편집하거나 삭제하여 방금 만든 규칙을 테스트합니다.

## 비즈니스 규칙 관리

기존 비즈니스 규칙을 편집, 삭제 또는 비활성화할 수 있습니다.

기존 규칙을 편집해도 기존 레코드는 변경되지 않습니다. 편집된 규칙은 누군가 기존 레코드를 편집하거나 삭제하려고 할 때만 적용됩니다.

1. 레코드 종류의 **비즈니스 규칙** 구성 페이지로 돌아갑니다.
1. 변경할 규칙을 찾습니다.
1. 규칙 이름 위로 마우스를 가져간 후 **추가** 메뉴 ![추가 메뉴](assets/more-menu.png)를 클릭한 후 다음 옵션 중 하나를 클릭하십시오.

   * **편집**: 비즈니스 규칙 설정 페이지가 열리고 비즈니스 규칙에 대한 정보를 편집할 수 있습니다.
   * **Deactivate**: <!--check this in the UI: right now, it says Disable--> 이렇게 하면 규칙이 트리거되는 것을 중지하지만 필요한 경우 나중에 계속 유지됩니다.
   * **삭제**: 규칙에 대한 모든 정보가 삭제됩니다. 삭제된 규칙은 복구할 수 없습니다.

   편집된 규칙 또는 규칙의 비활성화는 미래 기록에 대해서만 적용되며 소급 적용되지 않습니다.

   <!--add screen shot if UI is fixed with Deactivate-->


<!--

***********FROM CLAUDE - BELOW - MUST EDIT*******************


### What business rules actually do

Business rules attach a condition to a **status change**. Instead of enforcing complete data the moment someone creates a record (which would slow everyone down), the rule only kicks in at one specific, deliberate moment: when a status is about to change to a status you've configured.

A rule looks like this in plain language:

> "Before a record can move to **Ready for Execution**, the field **Brand** must have a value."

If the field is empty, the status change is blocked and the person gets a clear message telling them what to fix. Once they fill it in and try again, the change goes through.

A few important things this is *not*:

* **It doesn't block record creation.** People can still create a new record instantly and fill it in over time, exactly like today. 
* **It doesn't auto-fill anything or auto-change statuses.** A person always has to make the status change themselves.
* **It doesn't retroactively flag old records.** Records that are already sitting in the target status aren't affected — the check only runs the next time someone tries to move a record *into* that status.

### Step 1: Open the business rules configuration area

Business rules live alongside your other admin setup — you won't need to hunt for a separate "Planning" panel. From your workflow setup area:

1. Go to the main **workflow setup / admin configuration** area for your workspace.
2. Look for the **business rules** section for the record type you want to configure (for example, "Materials" or "Campaigns").


### Step 2: Choose the record type

Rules are configured per record type, so pick the one you want to add a rule to. For example, if you want to make sure every Materials record has key fields filled in before execution, select **Materials**.

### Step 3: Create a new rule

For each rule, you'll specify three things:

| What you set | Example |
|---|---|
| **Record type** | Materials |
| **Target status** | Ready for Execution |
| **Required field** | Brand |

In other words: "When a Materials record's status is changed to **Ready for Execution**, the field **Brand** must have a value."

You can add more than one rule for the same status. For example, you might require Brand, Therapeutic Area, Indication, and Estimated Launch Date all to be filled in before a record can move to "Ready for Execution" — each is its own rule, and all of them are checked together.

**What fields can you require?**

* Connected record fields (e.g., a linked Brand or Indication record) — the rule passes as soon as at least one record is linked.
* Standard text fields (single-line or paragraph) — the rule passes once there's any value.
* Date fields — the rule passes once a date is set.

**What you can't use yet:** formula fields and lookup fields aren't supported as rule targets in this release, since they're calculated in the background rather than filled in directly by a person.

### Step 4: Write the message people will see

When you create a rule, you'll also provide the message that shows up if someone tries to make the change without the field filled in. Keep it specific and actionable — something like:

> "Brand is required."

You don't need to worry about formatting a whole error banner — the system handles combining messages if multiple rules are violated at once (see below).

### Step 5: Save the rule

Once saved, the rule takes effect **immediately** for everyone in the workspace — no need to log out, refresh, or wait for a deployment. The very next time anyone tries to move a record into that status, the rule is checked.

### What your team will actually experience

Here's what changes for the people using Planning day to day, once a rule is live.

#### If a required field is empty

1. A planner opens a record and changes the status to the gated status (say, "Ready for Execution").
2. The system checks all rules tied to that status.
3. If a required field is empty, the change is **rejected** — the status reverts back to what it was.
4. A toast message appears, naming exactly which field(s) are missing:
   > *"Status change blocked: 'Brand' and 'Estimated Launch Date' must be populated before moving to 'Ready for Execution.'"*
5. The planner fills in the missing field(s) and tries the status change again.
6. This time, the rule passes, and the status updates normally.

#### If everything is already filled in

Nothing changes. The status updates instantly, with no extra steps or popups. Business rules are invisible until they're actually needed.

#### If several fields are missing at once

All the violated rules are checked together, and the message lists every missing field in one go — planners don't have to fix one field, try again, get told about the next one, and repeat.

### Step 6: Edit or remove a rule later

Rules aren't set in stone. To make changes:

1. Go back to the business rules configuration area for the record type.
2. Find the rule you want to change.
3. Edit the required field, target status, or message — or delete the rule entirely.
4. Save. The change applies immediately to future status changes.

Keep in mind: editing or deleting a rule **only affects transitions going forward.** Records that already made it into the target status before the change aren't reevaluated.
3## A few things worth knowing

* **This is separate from locking records after a status change.** Business rules (as described here) only check field completeness *before* a status change goes through. A different, related feature governs whether a record becomes fully locked from edits/deletion once it reaches a certain status — that's not what's covered here.
* **Bulk status changes** (changing status on many records at once) aren't fully defined yet for how they interact with business rules — if your team relies heavily on bulk actions, check with your Adobe contact on current behavior.
* **If a rule can't be evaluated** due to a system error, the transition is blocked rather than silently allowed through — you'll never end up with an incomplete record slipping past a rule because of a backend hiccup.
* **Turning the feature off** doesn't delete your configured rules — they're just paused. Turning it back on restores them exactly as they were, no reconfiguration needed.

### Quick reference: setting up your first rule

1. Confirm the feature is enabled for your tenant.
2. Go to workflow setup → business rules for your record type.
3. Choose the record type (e.g., Materials).
4. Create a rule: target status + required field.
5. Write a clear, specific error message.
6. Save — it's live immediately.
7. Repeat for each field you want to require.
8. Test it yourself: try changing a record's status with the field empty, confirm you see the expected message, fill in the field, and confirm the status change now goes through.

That's it — from here on, anyone converting a record forward will get a clear nudge if something's missing, instead of a downstream project quietly showing up incomplete.

-->