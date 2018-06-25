---
title: Операция GetUserRetentionPolicyTags
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 57c6ff23-5c2c-42ee-824b-5a1b6dafab8c
description: Найдите сведения о веб-служб Exchange GetUserRetentionPolicyTags операции.
ms.openlocfilehash: 2b1267ce6822c7bad05ad2ef88547ba75c632ab0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833700"
---
# <a name="getuserretentionpolicytags-operation"></a>Операция GetUserRetentionPolicyTags

Найдите сведения о **GetUserRetentionPolicyTags** операции веб-служб Exchange. 
  
Операция **GetUserRetentionPolicyTags** возвращает список всех по умолчанию, системная папка и личных тегов, которые связаны с пользователем с помощью политики системы или, были ли применены пользователем. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-getuserretentionpolicytags-operation"></a>С помощью операции GetUserRetentionPolicyTags

Эта операция возвращает отображаемое имя, идентификатор хранения, срок хранения данных, тип хранения, действие хранения и описание теги и значения для свойства **IsVisible**, **OptedInto**и **IsArchive** . 
  
### <a name="getuserretentionpolicytags-operation-soap-headers"></a>Заголовки SOAP GetUserRetentionPolicyTags операции

Операция **GetUserRetentionPolicyTags** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Это применимо к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Это применимо для ответа.  <br/> |
   
## <a name="getuserretentionpolicytags-operation-request-example"></a>Пример запроса GetUserRetentionPolicyTags операции

В следующем примере запрос операции **GetUserRetentionPolicyTags** показано, как получить список тегов для текущего пользователя. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetUserRetentionPolicyTags />
   </soap:Body>
</soap:Envelope>
```

Запрос SOAP body содержит следующий элемент:
  
- [GetUserRetentionPolicyTags](getuserretentionpolicytags.md)
    
## <a name="successful-getuserretentionpolicytags-operation-response"></a>Успешные операции ответа GetUserRetentionPolicyTags

В следующем примере показано успешного ответа на запрос операции **GetUserRetentionPolicyTags** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="179" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetUserRetentionPolicyTagsResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <RetentionPolicyTags>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>1 Year Delete</DisplayName>
               <RetentionId>e66252f9-794f-4b36-b55e-d6d95fdf87a3</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>true</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Personal 1 year move to archive</DisplayName>
               <RetentionId>b2a29464-649c-4174-932b-6aaac9811c89</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>MoveToArchive</RetentionAction>
               <Description/>
               <IsVisible>true</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>true</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Sent Items</DisplayName>
               <RetentionId>b0d32f1b-fbd0-4c1d-ba3e-ddd1086ea1d3</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>SentItems</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Default 1 year delete</DisplayName>
               <RetentionId>29fc9b9d-98b0-4c01-acf8-3996e2afce98</RetentionId>
               <RetentionPeriod>365</RetentionPeriod>
               <Type>All</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Two Year Retention</DisplayName>
               <RetentionId>a1a38957-2557-404e-9f32-53d77c948f62</RetentionId>
               <RetentionPeriod>730</RetentionPeriod>
               <Type>Personal</Type>
               <RetentionAction>DeleteAndAllowRecovery</RetentionAction>
               <Description>Use this tag for all items to be retained for two years.</Description>
               <IsVisible>true</IsVisible>
               <OptedInto>true</OptedInto>
               <IsArchive>false</IsArchive>
            </RetentionPolicyTag>
            <RetentionPolicyTag xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <DisplayName>Default two year move to archive</DisplayName>
               <RetentionId>75bc8dbe-a0e8-4e09-9fa3-fd4c21f49318</RetentionId>
               <RetentionPeriod>730</RetentionPeriod>
               <Type>All</Type>
               <RetentionAction>MoveToArchive</RetentionAction>
               <Description/>
               <IsVisible>false</IsVisible>
               <OptedInto>false</OptedInto>
               <IsArchive>true</IsArchive>
            </RetentionPolicyTag>
         </RetentionPolicyTags>
      </GetUserRetentionPolicyTagsResponse>
   </s:Body>
</s:Envelope>

```

Ответ SOAP body содержит следующие элементы:
  
- [GetUserRetentionPolicyTagsResponse](getuserretentionpolicytagsresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [RetentionPolicyTags](retentionpolicytags.md)
    
- [RetentionPolicyTag](retentionpolicytag.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
- [RetentionId](retentionid.md)
    
- [RetentionPeriod](retentionperiod.md)
    
- [Тип (ElcFolderType)](type-elcfoldertype.md)
    
- [RetentionAction](retentionaction.md)
    
- [Описание](description.md)
    
- [IsVisible](isvisible.md)
    
- [OptedInto](optedinto.md)
    
- [IsArchive](isarchive.md)
    
## <a name="getuserretentionpolicytags-operation-error-response"></a>Ошибка операции GetUserRetentionPolicyTags ответа

Коды ошибок, которые являются общими для веб-служб Exchange в разделе [ResponseCode](responsecode.md).
  
## <a name="see-also"></a>См. также



[Политики хранения в веб-служб Exchange](http://msdn.microsoft.com/library/a132872f-0228-4bcb-aac2-bf64fb07e58e%28Office.15%29.aspx)

