---
title: Операция AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: Операция AddEntityFeedback возвращает сведения об ошибках, соответствующие ошибкам на стороне сервера.
ms.openlocfilehash: d4322bcc075c8c68b1f3d5f2ae22badea02be452
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546828"
---
# <a name="addentityfeedback-operation"></a>Операция AddEntityFeedback

Операция **AddEntityFeedback** возвращает сведения об ошибках, соответствующие ошибкам на стороне сервера. 
  
Эта операция зависит от типа регистрируется событие. Одним из наиболее важных событий **является EntityAdded,** соответствующее выбранному объекту. Эта операция является пакетной, поэтому ее можно использовать для журнала пакетов записей в одном запросе. 
  
## <a name="findpeople-request-examples"></a>Примеры запросов FindPeople

Операция **AddEntityFeedback** позволяет клиентам зайти в журнал сведений о взаимодействии с объектами, возвращенными службой. Это может быть использовано в качестве сигнала для повышения актуальности за кулисами для каждого клиента. Например, клиенты могут использовать эту операцию для предоставления отзывов о лицах людей, возвращающихся из **FindPeople.**
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
            <m:EntityFeedbackEntries>
                  <t:EntityFeedbackEntry>
                        <t:ClientEventTimeUTC> 2015-07-05T22:16:18+00:00</t:ClientEventTimeUTC>
                        <t:ClientEventTimeLocal> 2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
                        <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
                        <t:ClientVersion>15.01.0101.01</t:ClientVersion>
                        <t:ClientId>Web</t:ClientId>
                        <t:TransactionId>123456789</t:TransactionId>
                        <t:EventType>EntityAdded</t:EventType>
                        <t:TargetEntityList>["a","b","c"]</t:TargetEntityList>
                        <t:SourceOfEntityAdded></t:SourceOfEntityAdded>
                        <t:JSONPropertyBag></t:JSONPropertyBag>
                  </t:EntityFeedbackEntry>
                  <t:EntityFeedbackEntry>
                  …
                  </t:EntityFeedbackEntry>
            </m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

### <a name="the-request-soap-body-contents"></a>Содержимое тела SOAP запроса

Запрос на мыло содержит один элемент **EntityFeedbackEntries.** Это, в свою очередь, содержит массив объектов **EntityFeedbackEntry.** Каждая запись в массиве может содержать следующие элементы. 
  
|**Параметры запроса**|**Обязательный**|**Описание**|**Тип**|
|:-----|:-----|:-----|:-----|
|**ClientEventTimeUtc** <br/> |Да  <br/> |Время UTC, когда событие произошло на стороне клиента.  <br/> |Даты и время  <br/> |
|**ClientEventTimeLocal** <br/> |Да  <br/> |Локальное время, когда событие происходило на стороне клиента.  <br/> |Даты и время  <br/> |
|**ClientId** <br/> |Да  <br/> |Тип клиента (например, Outlook, OWA и т.д.).  <br/> |Список clientIDType  <br/> |
|**ClientSessionId** <br/> |Да  <br/> |GUID, определяющий идентификацию сеанса. Созданный на клиенте.  <br/> |GUID  <br/> |
|**ClientVersion** <br/> |Да  <br/> |Версия клиента (например, 15.01.0101.000).  <br/> |String  <br/> |
|**EntityAddSource** <br/> |Нет  <br/> |Источник для EntityAded (например, EntityRelevanceAPI, типы, вклейка).  <br/> |EntityAddSource Enumeration  <br/> |
|**EntrySequenceNumber** <br/> |Да  <br/> |Инкрементное integer для каждого клиентского сеанса. Используется для обнаружения потери данных.  <br/> |Целое  <br/> |
|**EventType** <br/> |Да  <br/> |Тип события (например, добавленная сущность, удаление сущности).  <br/> |String  <br/> |
|**JSONPropertyBag** <br/> |Нет  <br/> |Дополнительные свойства, связанные с событием (BLOB JSON пар ключа и значения).  <br/> |JSON Blob  <br/> |
|**TargetEntityList** <br/> |Нет  <br/> |Список сущностями, связанными с событием.  <br/> |Строка JSON  <br/> |
|**TransactionId** <br/> |Нет  <br/> |ID (GUID) соотносится с ID в журналах запросов.  <br/> |String  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>Успешный ответ операции AddEntityFeedback

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a>Тело SOAP ответа содержит следующие элементы

#### <a name="errors"></a>Ошибки 
  
API может входить в журнал пакет записей обратной связи, мы внося все, что можем. Это поле представляет количество записей об ошибках, которые не были зарегистрированы.
    
#### <a name="errordetails"></a>ErrorDetails
  
Сведения, относящиеся к ошибкам, которые были выше, разделяются по `;` .
    
### <a name="currently-supported-values"></a>Поддерживаемые в настоящее время значения

|**Список ClientIdType**|
|:-----|
|Версия для настольного компьютера  <br/> |
|Exchange  <br/> |
|IMAP4  <br/> |
|Lync  <br/> |
|MacMail  <br/> |
|MacOutlook  <br/> |
|Мобильная версия  <br/> |
|Другие  <br/> |
|Outlook  <br/> |
|OutlookService  <br/> |
|POP3  <br/> |
|Tablet  <br/> |
|Веб  <br/> |
   
|**EntityAddSource Enumeration**|
|:-----|
|ActiveDirectory  <br/> |
|EntityRelevanceApi  <br/> |
|EntityRelevanceApiCache  <br/> |
|ExplicitTyping  <br/> |
|LocalCache  <br/> |
|LocalCacheAndEntityRelevanceAPI  <br/> |
|Нет  <br/> |
|Другие  <br/> |
|Вставить  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a>Ответ на ошибку операции AddEntityFeedback

Коды ошибок, которые являются общими для EWS, см. [в рубрике ResponseCode.](responsecode.md)
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>Пример AddEntityFeedback совместно с FindPeople

#### <a name="findpeople-request"></a>Запрос FindPeople
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
<soap:Body >
    <m:FindPeople>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:QueryString>user1</m:QueryString>
      <m:SearchPeopleSuggestionIndex>true</m:SearchPeopleSuggestionIndex>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>    
    
```

#### <a name="findpeople-response"></a>Ответ FindPeople

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
                    <PersonaId Id="AAUQAFjZ4UxX8SZCqSPFsmh0cSo=" />
                    <PersonaType>Person</PersonaType>
                    <CreationTime>2015-10-02T23:25:42</CreationTime>
                    <DisplayName>user2</DisplayName>
…
                  </Persona>
            </People>
            <TotalNumberOfPeopleInView>0</TotalNumberOfPeopleInView>
            <FirstMatchingRowIndex>0</FirstMatchingRowIndex>
            <FirstLoadedRowIndex>0</FirstLoadedRowIndex>
            <TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</TransactionId>
        </FindPeopleResponse>
    </s:Body>
</s:Envelope>

```

#### <a name="addentityfeedback-request"></a>Запрос AddEntityFeedback

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:AddEntityFeedback>
<m:EntityFeedbackEntries>
<t:EntityFeedbackEntry>
         <t:ClientEventTimeUtc>2015-07-05T22:16:18+00:00</t:ClientEventTimeUtc>
         <t:ClientEventTimeLocal>2015-07-05T22:16:18+00:00</t:ClientEventTimeLocal>
         <t:ClientSessionId>00000000-0000-0000-0000-000000000012</t:ClientSessionId>
         <t:ClientVersion>15.01.0101.01</t:ClientVersion>
         <t:ClientId>Web</t:ClientId>
         <t:TransactionId>b56ad16e-5d5a-4574-90f8-b8dd57382be6</t:TransactionId>
         <t:EventType>EntityAdded</t:EventType>
         <t:TargetEntityList>["user1@ms7.com"]</t:TargetEntityList>
         <t:SourceOfEntityAdded>EntityRelevanceApi</t:SourceOfEntityAdded>
         <t:JSONPropertyBag></t:JSONPropertyBag>
</t:EntityFeedbackEntry>
</m:EntityFeedbackEntries>
      </m:AddEntityFeedback>
   </soap:Body>
</soap:Envelope>

```

> [!NOTE]
> Использование ID транзакции отклика FindPeople в качестве ID запроса addEntityFeedback. 
  
#### <a name="addentityfeedback-response"></a>Ответ AddEntityFeedback

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


