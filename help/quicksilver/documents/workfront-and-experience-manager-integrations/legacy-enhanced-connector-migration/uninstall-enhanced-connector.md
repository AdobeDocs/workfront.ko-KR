---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Workfront for Adobe Experience Manager 강화 커넥터 제거
description: Workfront 및 Adobe Experience Manager Assets as a Cloud Service을 연결하는 최신 기본 통합으로 Workfront with Adobe Experience Manager 강화 커넥터를 제거해야 합니다.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 9673009f12509b5e7051ee91e142d311f333f215
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Workfront with Adobe Experience Manager 강화 커넥터 제거

Workfront 및 Adobe Experience Manager Assets as a Cloud Service을 연결하는 최신 기본 통합으로 Workfront with Adobe Experience Manager 강화 커넥터를 제거해야 합니다.

## 전제 조건

* (선택 사항) 필요한 경우 Workfront 방화벽 구성 및 AEM Dispatcher 설정에 대한 변경 사항을 되돌립니다.

## 향상된 커넥터 제거

1. AEM Cloud Manager에서 as a Cloud Service 저장소에 액세스하고 복제합니다.

1. 복제된 git 저장소를 선택한 IDE에서 엽니다.

1. 향상된 커넥터가 설치된 분기를 체크아웃합니다.

1. 다음 경로로 이동하여 향상된 커넥터 zip 파일을 제거합니다.

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. 프로젝트 루트의 pom.xml 파일에서 다음 종속성을 제거합니다.

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >위의 코드 블록에서 참조된 버전(예: 1.8.0)이 코드에서 제거 중인 버전을 반영하는지 확인하십시오.

1. 이름이 인 프로젝트의 하위 모듈에 있는 pom.xml 파일에서 다음 종속성을 제거합니다. **모두**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. 이름이 all인 프로젝트의 하위 모듈에 있는 pom.xml 파일에서 다음과 같은 포함된 을 제거합니다.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (조건부) 프로젝트 루트의 pom.xml 파일에서 저장소 구성을 제거합니다.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (조건부) 다음 경로에 있는 settings.xml에서 서버 구성을 제거합니다.프로젝트 루트의 /cloudmanager/maven/settings.xml

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. 변경 사항을 커밋하고 코드를 Cloud Manager 저장소에 푸시합니다.

1. Cloud Manager 파이프라인을 실행하여 Cloud Services 인스턴스에 변경 사항 배포
