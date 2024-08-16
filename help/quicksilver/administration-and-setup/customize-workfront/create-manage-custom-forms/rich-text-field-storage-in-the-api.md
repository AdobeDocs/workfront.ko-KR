---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: API의 리치 텍스트 필드 스토리지
description: 프로젝트, 문제 또는 작업과 같은 오브젝트에 리치 텍스트가 포함된 경우 Workfront API를 통해 매개 변수 값으로 저장되고 액세스할 수 있습니다.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: 3f7f4557c18bbb91ece850f910350d926a9e84bf
workflow-type: tm+mt
source-wordcount: '174'
ht-degree: 0%

---

# API의 리치 텍스트 필드 스토리지

프로젝트, 문제 또는 작업과 같은 오브젝트에 리치 텍스트가 포함된 경우 Workfront API를 통해 매개 변수 값으로 저장되고 액세스할 수 있습니다.

서식 있는 텍스트가 포함된 프로젝트 개체에서 텍스트 정보를 요청하려면 필드 **parameterValues**&#x200B;을(를) 사용합니다.

예를 들어 간단한 HTTP 요청은 다음과 유사할 수 있습니다.

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

이 예제 프로젝트에 계산 필드, 단락 텍스트 및 서식 있는 1의 세 가지 사용자 정의 필드가 있는 사용자 정의 양식이 포함된 경우. 그러면 위의 요청은 다음과 유사한 응답을 반환합니다. 여기서 필드 &quot;rich 1&quot;은 리치 텍스트 매개 변수 필드이고 텍스트 값은 &quot;**Hello** *World!*&quot;입니다.

```
{
    Data: {
        ID: "xxxxxxxxxxxxxxxxxxxxxxx",
        name: "new project with rich text",
        objCode: "PROJ",
        - parameterValues: {
            DE:rich 1: "{
                "blocks":[
                {
                    "key":"7eibh",
                    "text":"Hello Word!",
                    "type":"unstyled",
                    "depth":0,
                    "inlineStyleRanges":[
                    {
                        "offset":0,
                        "length":6,
                        "style":"BOLD"
                    },
                    {
                        "offset":6,
                        "length":5,
                        "style":"ITALIC"
                    }
                    ],
                    "entityRanges":[
                    ],
                "data":{
                }
                }
                ],
            "entityMap":{
            }
        }",
        DE: paragraph text: "here is some paragraph text",
        DE: calc field: "here is a calc field entry",
        }
    }
}
```

서식 있는 텍스트 정보가 저장되고 Adobe Workfront API를 통해 검색할 수 있는 방법에 대한 자세한 내용은 [Adobe Workfront API의 서식 있는 텍스트 필드](../../../wf-api/general/rich-text-field-api.md)를 참조하십시오.
