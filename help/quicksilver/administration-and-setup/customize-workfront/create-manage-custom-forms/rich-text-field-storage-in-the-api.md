---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: API의 리치 텍스트 필드 저장소
description: 프로젝트, 문제 또는 작업과 같은 개체에 리치 텍스트가 포함되어 있는 경우 Workfront API를 통해 매개 변수 값으로 저장되고 액세스할 수 있습니다.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2e4b18be-14bb-4d47-8e63-e2f4a5dc376f
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 0%

---

# API의 리치 텍스트 필드 저장소

프로젝트, 문제 또는 작업과 같은 개체에 리치 텍스트가 포함되어 있는 경우 Workfront API를 통해 매개 변수 값으로 저장되고 액세스할 수 있습니다.

서식 있는 텍스트가 포함된 프로젝트 개체에서 텍스트 정보 요청을 이 필드를 사용하여 수행할 수 있습니다 **parameterValues**.

예를 들어 간단한 HTTP 요청은 다음과 유사할 수 있습니다.

`https://your-company.workfront.com/attask/api/v11.0/project?ID=your-project-ID&fields=parameterValues:*`

이 예제 프로젝트에 사용자 지정 필드가 3개인 사용자 지정 양식이 포함된 경우: 계산 필드, 단락 텍스트 및 리치 1 그런 다음 위의 요청은 다음과 유사한 응답을 반환합니다. 여기서 &quot;rich 1&quot; 필드는 리치 텍스트 매개 변수 필드이고 텍스트 값은 &quot;입니다&#x200B;**Hello** *세상!*&quot;:

```
{
	Data: {
		ID: “xxxxxxxxxxxxxxxxxxxxxxx”,
		name: “new project with rich text”,
		objCode: “PROJ”,
		- parameterValues: {
			DE:rich 1: “{
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
		}”,
		DE: paragraph text: “here is some paragraph text”,
		DE: calc field: “here is a calc field entry”,
		}
	}
}
```

Adobe Workfront API를 통해 리치 텍스트 정보를 저장하고 검색할 수 있는 방법에 대한 자세한 내용은 [Adobe Workfront API의 리치 텍스트 필드](../../../wf-api/general/rich-text-field-api.md).
