---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: avoiding-spam-filters
title: 일반 이메일 클라이언트에 대한 스팸 설정 구성
description: ' [!DNL Workfront Proof] 이메일이 스팸 폴더로 전송되지 않도록 이메일 클라이언트를 구성할 수 있습니다.'
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 41517540-c5a8-4bf5-997b-e7a605337e73
source-git-commit: c989687e9adaf12a31a920921bf8fb69425ca1c5
workflow-type: tm+mt
source-wordcount: '1480'
ht-degree: 0%

---

# 일반 이메일 클라이언트에 대한 스팸 설정 구성

>[!IMPORTANT]
>
>이 문서는 독립 실행형 제품 [!DNL Workfront Proof]의 기능을 참조합니다. [!DNL Adobe Workfront] 내부의 증명에 대한 자세한 내용은 [증명](../../../review-and-approve-work/proofing/proofing.md)을 참조하십시오.

[!DNL Workfront Proof]개의 이메일이 스팸 폴더로 전송되지 않도록 이메일 클라이언트를 구성할 수 있습니다.

다음 섹션에서는 다양한 이메일 클라이언트에 대한 이 프로세스를 설명합니다.

## [!DNL Gmail]

이 섹션에서 다음을 수행합니다.

* [!DNL Gmail]의 [!UICONTROL 연락처] 목록에 두 개의 [!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 주소를 추가하거나 [!UICONTROL Gmail]이(가) 해당 주소에서 [!UICONTROL 스팸] 폴더로 전자 메일을 라우팅하지 못하도록 필터를 만듭니다
* [!UICONTROL 스팸] 폴더에서 기존 [!DNL Workfront Proof]개의 전자 메일을 제거하고 [!DNL Workfront Proof]개의 메시지를 휴지통으로 라우팅하는 필터를 변경하십시오

### 새 [!DNL Workfront Proof]개 전자 메일

[!DNL Gmail]의 [!UICONTROL 연락처] 목록에 두 개의 [!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 주소를 추가하거나 [!DNL Gmail]에서 [!DNL Workfront Proof] 전자 메일이 [!UICONTROL 스팸] 폴더로 라우팅되지 않도록 전자 메일 필터를 만드십시오. [!UICONTROL 연락처] 목록에 두 개의 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소를 추가하려면:

1. Gmail 페이지의 왼쪽 상단 모서리에서 **[!UICONTROL 메일]** 아래의 **[!UICONTROL 연락처]**&#x200B;를 클릭합니다.

1. [!UICONTROL 연락처] 및 [!UICONTROL 작업]을 표시하려면 [!UICONTROL 메일] 다음에 더하기(+) 기호를 클릭해야 할 수 있습니다. 더하기 기호가 나타나지 않으면 커서를 [!UICONTROL 메일] (으)로 이동하면 더하기 기호가 나타납니다.
1. 연락처 목록 및 연락처 메일 주소 위에 있는 **[!UICONTROL 내 연락처에 추가]** 단추를 클릭합니다.
1. 첫 번째 &quot;[!UICONTROL from]&quot; 주소를 복사하여 레이블이 지정되지 않은 전자 메일 주소 대화 상자에 붙여넣습니다.
1. 대화 상자 아래의 **[!UICONTROL 추가]**&#x200B;를 클릭합니다. 주소가 연락처 목록에 추가됩니다.
1. 두 번째 &quot;[!UICONTROL from]&quot; 주소에 대해 2-4단계를 반복합니다.

또는 두 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소 각각에 대한 전자 메일 필터를 만들려면:

1. Gmail 페이지 상단의 **[!UICONTROL 검색]** 단추 옆에 있는 **[!UICONTROL 필터 만들기]**&#x200B;를 클릭합니다.

1. 첫 번째 &quot;[!UICONTROL from]&quot; 주소를 복사하여 **[!UICONTROL 필터 만들기]** 상자의 **[!UICONTROL From]** 필드에 붙여넣습니다.

1. **[!UICONTROL 다음 단계]** 단추를 클릭합니다.
1. **[!UICONTROL 작업 선택]** 목록에서 **[!UICONTROL 스팸으로 보내지 않음]**&#x200B;을 선택합니다.

1. **[!UICONTROL 필터 만들기]** 단추를 클릭합니다. 필터가 [!UICONTROL 설정] 페이지의 필터 목록에 추가됩니다.
1. 두 번째 &quot;[!UICONTROL from]&quot; 주소에 대해 설정 페이지 하단의 **[!UICONTROL 필터 만들기]**&#x200B;를 클릭하고 2~5단계를 반복합니다.

### 기존 [!DNL Workfront Proof]개 전자 메일

[!DNL Gmail]이(가) 마지막으로 지운 이후 [!UICONTROL 스팸] 폴더에 저장한 [!DNL Workfront Proof]개의 전자 메일을 제거하려면:

1. Gmail 페이지 왼쪽의 폴더 목록에서 **[!UICONTROL 스팸]**&#x200B;을 클릭합니다.
1. [!UICONTROL 스팸] 폴더에서 [!DNL Workfront Proof]개의 전자 메일을 선택합니다.
1. [!UICONTROL 스팸] 목록 위에 있는 **[!UICONTROL 스팸 아님]** 단추를 클릭합니다.\
   이제 받은 편지함에서 [!DNL Workfront Proof]개의 전자 메일을 찾을 수 있습니다.

[!DNL Workfront Proof]개의 전자 메일을 휴지통으로 보내는 필터를 변경하려면:

1. Gmail 페이지 상단의 [!UICONTROL 검색] 단추 옆에 있는 **[!UICONTROL 필터 만들기]**&#x200B;를 클릭합니다.
1. [!UICONTROL 필터 만들기] 대화 상자 아래쪽에 있는 **[!UICONTROL 현재 필터 표시]**&#x200B;를 클릭합니다. 기존 필터는 설정 페이지에 필드(보낸 사람), 이름 또는 주소로 나열됩니다.
1. [!UICONTROL 기존 [!DNL Workfront Proof] 주소에 대해 이 작업 수행] 필터가 [!UICONTROL 삭제]인 경우 **[!UICONTROL 편집]**&#x200B;을 클릭하세요.
1. **[!UICONTROL 다음 단계]** 단추를 클릭합니다.
1. **[!UICONTROL 삭제]** 옵션을 선택 취소하고 **[!UICONTROL 스팸으로 보내지 않음]**&#x200B;을 선택합니다.

1. **[!UICONTROL 필터 업데이트]** 단추를 클릭합니다.\
   [!UICONTROL 설정] 페이지가 다시 표시됩니다.

1. 추가 [!DNL Workfront Proof] 주소 필터가 나열되면 각 필터에 대해 3-6단계를 반복합니다.

## [!DNL Microsoft Outlook] 2003 - 2007

이 섹션에서 다음을 수행합니다.

* 두 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소를 [!DNL Outlook]의 [!UICONTROL 수신 허용 - 보낸 사람] 목록에 추가합니다.
* [!UICONTROL 정크 메일] 폴더에서 기존 [!DNL Workfront Proof]개의 전자 메일을 제거하고 [!UICONTROL 수신 거부] 목록에서 &quot;[!UICONTROL 발신]&quot;개의 주소를 제거합니다.

### 새 [!DNL Workfront Proof]개 전자 메일

Outlook의 수신 허용 - 보낸 사람 목록에 두 개의 [!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 주소를 추가하려면:

1. **[!UICONTROL 도구]** 메뉴에서 **[!UICONTROL 옵션]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 기본 설정]** 탭의 **[!UICONTROL 메일]**&#x200B;에서 **[!UICONTROL 정크 메일]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 수신 허용 - 보낸 사람]** 탭에서 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.

1. **[!UICONTROL 주소 또는 도메인 추가]** 상자에서 첫 번째 &quot;[!UICONTROL from]&quot; 주소 또는 도메인 이름(@ 기호 뒤에 있는 나머지 이름)만 복사하여 붙여 넣으십시오.
1. **[!UICONTROL 확인]**&#x200B;을 클릭합니다. 주소가 목록에 추가됩니다.
1. 두 번째 &quot;[!UICONTROL from]&quot; 주소에 대해 3-5단계를 반복합니다.

### 기존 [!DNL Workfront Proof]개 전자 메일

[!DNL Outlook]이(가) 마지막으로 지운 이후 [!UICONTROL 정크 메일] 폴더에 저장한 [!DNL Workfront Proof]개의 전자 메일을 제거하려면:

1. 탐색 창에서 **[!UICONTROL 정크 메일]** 폴더를 클릭합니다.
1. 폴더에 [!DNL Workfront Proof]개의 전자 메일이 있는 경우 각 전자 메일을 마우스 오른쪽 단추로 클릭하고 [!UICONTROL 정크 메일]을 선택한 다음 **[!UICONTROL 정크 메일이 아닌 것으로 표시]**&#x200B;를 클릭합니다.
1. 이제 받은 편지함에서 [!DNL Workfront Proof]개의 전자 메일을 찾을 수 있습니다.

[!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소가 수신 거부 목록에 있는지 확인하려면:

1. **[!UICONTROL 도구]** 메뉴에서 **[!UICONTROL 옵션]**&#x200B;을 클릭합니다

1. **[!UICONTROL 기본 설정]** 탭의 **[!UICONTROL 메일]**&#x200B;에서 **[!UICONTROL 정크 메일]**&#x200B;을 클릭합니다.

1. **[!UICONTROL 수신 거부]** 탭을 클릭합니다.
1. 목록에 [!DNL Workfront Proof]개의 주소가 있으면 각 주소를 클릭한 다음 **[!UICONTROL 제거]**&#x200B;를 클릭합니다.

## [!DNL Windows Live Hotmail]

이 섹션에서 다음을 수행합니다.

* [!DNL Windows Live Hotmail]의 [!UICONTROL 수신 허용 - 보낸 사람] 목록에 두 개의 [!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 주소를 추가하십시오.
* 정크 메일 폴더에서 기존 [!DNL Workfront Proof]개의 전자 메일을 제거하고 [!UICONTROL 수신 거부] 목록에서 &quot;[!UICONTROL 보낸 사람]&quot;개의 주소를 제거합니다.

### 새 [!DNL Workfront Proof]개 전자 메일

[!DNL Windows Live Hotmail]의 [!UICONTROL 수신 허용 - 보낸 사람] 목록에 두 [!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 주소를 추가하려면:

1. 사서함 페이지의 오른쪽 상단에 있는 **[!UICONTROL 옵션]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 추가 옵션]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 정크 메일]**&#x200B;에서 **[!UICONTROL 수신 허용 및 수신 거부]**&#x200B;을 클릭하세요.

1. **[!UICONTROL 수신 허용 - 보낸 사람]**&#x200B;을 클릭하세요.
1. 처음 &quot;[!UICONTROL from]&quot; 주소나 도메인 이름(@ 기호 뒤에 있는 나머지 이름)만 복사하여 [!UICONTROL Sender] 또는 도메인에 복사하여 안전한 필드로 표시합니다.
1. **[!UICONTROL 목록에 추가]** 단추를 클릭합니다. 주소가 목록에 나타납니다.
1. 두 번째 &quot;[!UICONTROL from]&quot; 주소에 대해 4-6단계를 반복합니다.

### 기존 [!DNL Workfront Proof]개 전자 메일

[!DNL Windows Live Hotmail]이(가) 마지막으로 지운 이후 [!UICONTROL 정크] 전자 메일 폴더에 저장한 [!DNL Workfront Proof]개의 전자 메일을 제거하려면:

1. 페이지 왼쪽의 **[!UICONTROL 폴더]**&#x200B;에서 **[!UICONTROL 정크]**&#x200B;를 클릭합니다.

1. 이 폴더에 [!DNL Workfront Proof]개의 전자 메일이 있는 경우 각 전자 메일을 열고 **[!UICONTROL 정크 메일 아님]** 링크를 클릭하세요.
1. 이제 받은 편지함에서 [!DNL Workfront Proof]개의 전자 메일을 찾을 수 있습니다.

[!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 주소가 [!UICONTROL 수신 거부] 목록에 있는지 확인하려면:

1. 사서함 페이지의 오른쪽 상단에 있는 **[!UICONTROL 옵션]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 추가 옵션]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 정크 메일]**&#x200B;에서 **[!UICONTROL 수신 허용 및 수신 거부]**&#x200B;을 클릭하세요.

1. **[!UICONTROL 수신 거부]**&#x200B;를 클릭합니다.
1. 목록에 [!DNL Workfront Proof]개의 주소가 있는 경우 각 주소를 선택하고 **[!UICONTROL 목록에서 제거]** 단추를 클릭합니다.

## [!DNL Yahoo Mail]

이 섹션에서 다음을 수행합니다.

* [!DNL Yahoo Mail]에서 받은 편지함으로 [!DNL Workfront Proof] 전자 메일을 보내도록 [!DNL Workfront Proof] &quot;[!UICONTROL 부터]&quot; 주소 두 개를 필터에 추가합니다.
* [!UICONTROL 스팸] 폴더에서 기존 [!DNL Workfront Proof]개 전자 메일 제거

### 새 [!DNL Workfront Proof]개 전자 메일

[!DNL Yahoo Mail]에서 각 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소의 새 필터를 만들려면:

1. 메일 페이지의 오른쪽 상단에 있는 **[!UICONTROL 옵션]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 추가 옵션]**&#x200B;을 클릭합니다.
1. 페이지 왼쪽의 **[!UICONTROL 필터]**&#x200B;를 클릭합니다.
1. **[!UICONTROL 필터 만들기 또는 편집]**&#x200B;을 클릭합니다.
1. 필터 페이지에서 **[!UICONTROL 추가]**&#x200B;를 클릭합니다.
1. 필터에 이름을 지정합니다.
1. [!UICONTROL From header] 규칙의 경우 **[!UICONTROL contains]** 옵션을 선택하고 첫 번째 &quot;[!UICONTROL from]&quot; 주소나 도메인 이름(@ 기호 뒤의 나머지 이름)만 복사하여 붙여 넣으십시오.
1. **[!UICONTROL 폴더 선택]**&#x200B;을 클릭하고 **[!UICONTROL 받은 편지함]**&#x200B;을 선택합니다.

1. *[!UICONTROL *필터 추가]** 단추를 클릭합니다. 필터가 필터 목록에 나타납니다.
1. 두 번째 &quot;[!UICONTROL from]&quot; 주소의 경우 5-9단계를 반복합니다.

### 기존 [!DNL Workfront Proof]개 전자 메일

[!DNL Yahoo Mail]이(가) 마지막으로 지운 이후 [!UICONTROL 스팸] 폴더로 라우팅한 [!DNL Workfront Proof]개의 전자 메일을 제거하려면:

1. [!UICONTROL 메일] 페이지 왼쪽에서 **[!UICONTROL 스팸]** 폴더를 선택하십시오.
1. 폴더에 [!DNL Workfront Proof]개의 전자 메일이 있는 경우 각 전자 메일을 선택하고 **[!UICONTROL 스팸 아님]** 단추를 클릭합니다.
1. 이제 받은 편지함에서 해당 이메일을 찾을 수 있습니다.

차단된 주소 목록에서 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소를 제거하려면:

1. 메일 페이지의 오른쪽 상단에 있는 **[!UICONTROL 옵션]**&#x200B;을 클릭합니다.
1. **[!UICONTROL 추가 옵션]**&#x200B;을 클릭합니다.
1. 페이지 왼쪽에서 **[!UICONTROL 스팸]**&#x200B;을 클릭합니다.
1. [!DNL Workfront Proof] 주소 또는 도메인 이름이 스팸 페이지의 **[!UICONTROL 차단된 전자 메일 주소]** 섹션에 나타나면 각 항목을 선택하고 **[!UICONTROL 제거]** 단추를 클릭하십시오.

## [!DNL Aol]

이 섹션에서 다음을 수행합니다.

* 두 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소를 [!DNL Aol] [!UICONTROL 주소록]에 추가합니다.
* [!DNL Aol] [!UICONTROL 스팸] 폴더에서 기존 [!DNL Workfront Proof] 전자 메일을 제거하고 [!DNL Aol] [!UICONTROL 스팸] 필터의 차단된 주소 목록에서 [!DNL Workfront Proof] &quot;[!UICONTROL 보낸 사람]&quot; 주소를 제거합니다.

### 새 [!DNL Workfront Proof]개 전자 메일

두 [!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소를 [!DNL Aol] [!UICONTROL 주소록]에 추가하려면:

1. **[!UICONTROL 메일]** 메뉴를 클릭합니다.
1. **[!UICONTROL 주소록]**&#x200B;을(를) 선택하십시오.
1. [!UICONTROL 주소록] 창 아래쪽에 있는 [!UICONTROL 추가] 단추를 클릭합니다.
1. **[!UICONTROL 새 연락처의 주소 카드]** 창에서 첫 번째 &quot;[!UICONTROL 보낸 사람]&quot; 주소를 복사하여 [!UICONTROL 기타 전자 메일] 필드에 붙여 넣고 해당 필드 옆에 있는 [!UICONTROL 기본 전자 메일] 라디오 단추를 확인하세요.
1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
1. 두 번째 &quot;[!UICONTROL from]&quot; 주소에 대해 3-5단계를 반복합니다.

### 기존 [!DNL Workfront Proof]개 전자 메일

[!DNL Aol]이(가) 마지막으로 지운 이후 [!UICONTROL 스팸] 폴더로 라우팅한 [!DNL Workfront Proof]개의 전자 메일을 제거하려면:

1. [!UICONTROL 메일] 메뉴를 클릭합니다.
1. **[!UICONTROL 스팸]** 폴더를 선택하십시오.
1. 폴더에 [!DNL Workfront Proof]개의 전자 메일이 있는 경우 한 번에 하나씩 각 전자 메일을 열고 **[!UICONTROL 스팸이 아님]** 단추를 클릭합니다.
1. 이제 받은 편지함에서 [!DNL Workfront Proof]개의 전자 메일을 찾을 수 있습니다.

[!DNL Workfront Proof] &quot;[!UICONTROL from]&quot; 주소가 [!DNL Aol] [!UICONTROL 스팸] 필터에서 차단되었는지 확인하려면:

1. **[!UICONTROL [!DNL Aol]키워드: 메일 컨트롤]**(으)로 이동하여 [!UICONTROL 스팸 설정] 페이지를 표시합니다.

1. [!DNL Aol] [!UICONTROL 키워드]은(는) [!DNL Aol] 소프트웨어만의 기능입니다. [!DNL Aol] [!UICONTROL Webmail] 또는 [!DNL Aol] [!UICONTROL 데스크톱]에서 [!UICONTROL 스팸 설정] 페이지에 액세스하는 데 필요한 지침이 필요한 경우 [!DNL Aol] 도움말을 참조하세요.
1. **[!UICONTROL 보낸 사람 필터]** 필드에서 **[!UICONTROL 지정한 주소에서 메일 차단]**&#x200B;을 선택하고 차단된 주소 목록에 [!DNL Workfront Proof] 주소 또는 도메인 이름이 포함된 경우 목록에서 해당 주소를 각각 삭제하십시오.

1. **[!UICONTROL 저장]**&#x200B;을 클릭합니다.
