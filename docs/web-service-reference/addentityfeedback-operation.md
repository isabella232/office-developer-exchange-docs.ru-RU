---
title: Операция AddEntityFeedback
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: Операция AddEntityFeedback возвращает сведения об ошибке, соответствующее проблем на сервере.
ms.openlocfilehash: b695806f543827d78aea139ffcbd7e4af58b9fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761343"
---
# <a name="addentityfeedback-operation"></a>Операция AddEntityFeedback

Операция **AddEntityFeedback** возвращает сведения об ошибке, соответствующее проблем на сервере. 
  
Эта операция зависит от типа ведущих запись в журнал событий. Одной из самых важных событиях является **EntityAdded**, соответствующий выбранной сущности. Это пакет, поэтому его можно использовать для записи в журнал пакетов записей в одном запросе. 
  
## <a name="findpeople-request-examples"></a>Примеры запросов FindPeople

Операция **AddEntityFeedback** позволяет клиентам входить сведений взаимодействия с сущностями, возвращенных службой. Это можно использовать в качестве сигнала для улучшения релевантности в фоновом режиме для каждого клиента. Например клиенты могут использовать эту операцию для оставьте свой отзыв на сущности людей, возвращенный из **FindPeople**.
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                             xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="the-request-soap-body-contents"></a>Содержимое текста запроса SOAP

Запрос soap содержит один элемент **EntityFeedbackEntries**. В свою очередь содержит массив объектов **EntityFeedbackEntry** . Каждая запись в массиве может содержать следующие элементы. 
  
|**Параметры запроса**|**Обязательное**|**Описание**|**Тип**|
|:-----|:-----|:-----|:-----|
|**ClientEventTimeUtc** <br/> |Да  <br/> |Время в формате UTC произошло событие на стороне клиента.  <br/> |DateTime  <br/> |
|**ClientEventTimeLocal** <br/> |Да  <br/> |Местное время возникновения события на стороне клиента.  <br/> |DateTime  <br/> |
|**ClientId** <br/> |Да  <br/> |Тип клиента (например, Outlook, OWA, и т.д.).  <br/> |Перечисление ClientIDType  <br/> |
|**ClientSessionId** <br/> |Да  <br/> |Идентификатор GUID, идентифицирующий идентификатор сеанса. Созданный на стороне клиента.  <br/> |GUID  <br/> |
|**ClientVersion** <br/> |Да  <br/> |Версия клиента (например, 15.01.0101.000).  <br/> |Строка  <br/> |
|**EntityAddSource** <br/> |Нет  <br/> |Источник EntityAded (например, EntityRelevanceAPI, типы, вставляемую).  <br/> |Перечисление EntityAddSource  <br/> |
|**EntrySequenceNumber** <br/> |Да  <br/> |Целое число добавочного на сеанс клиента. Используется для выявления потери данных.  <br/> |Int  <br/> |
|**EventType** <br/> |Да  <br/> |Тип события (например добавлена сущности, сущность удалена).  <br/> |Строка  <br/> |
|**JSONPropertyBag** <br/> |Нет  <br/> |Дополнительные свойства, связанные с событием (JSON больших двоичных объектов из пары "ключ значение").  <br/> |JSON больших двоичных объектов  <br/> |
|**TargetEntityList** <br/> |Нет  <br/> |Список сущностей, связанный с событием.  <br/> |Строка JSON  <br/> |
|**TransactionId** <br/> |Нет  <br/> |Идентификатор (GUID) сопоставления идентификатора журнала запросов.  <br/> |Строка  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>Успешные операции ответа AddEntityFeedback

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                                MinorVersion="1" 
                                MajorBuildNumber="228" 
                                MinorBuildNumber="0" 
                                Version="V2_49" 
                                xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                                xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" 
                                                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                                              xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                                                              xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope> 

```

### <a name="the-response-soap-body-contains-the-following-elements"></a>Ответ SOAP body содержит следующие элементы

#### <a name="errors"></a>Ошибки 
  
API-Интерфейс может войти в пакет записей свои отзывы и предложения, мы все, что мы можем журналов. Это поле представляет номер записи об ошибках, которые не были зарегистрированы.
    
#### <a name="errordetails"></a>ErrorDetails
  
Сведения, относящиеся к ошибкам выше отделяет, `;`.
    
### <a name="currently-supported-values"></a>В настоящее время поддерживаются значения

|**Перечисление ClientIdType**|
|:-----|
|Настольный ПК  <br/> |
|Exchange  <br/> |
|IMAP4  <br/> |
|Lync  <br/> |
|MacMail  <br/> |
|MacOutlook  <br/> |
|Мобильная версия  <br/> |
|Other (другие)  <br/> |
|Outlook  <br/> |
|OutlookService  <br/> |
|ПРОТОКОЛ POP3  <br/> |
|Планшетный ПК  <br/> |
|"Web" (Интернет);  <br/> |
   
|**Перечисление EntityAddSource**|
|:-----|
|ActiveDirectory  <br/> |
|EntityRelevanceApi  <br/> |
|EntityRelevanceApiCache  <br/> |
|ExplicitTyping  <br/> |
|LocalCache  <br/> |
|LocalCacheAndEntityRelevanceAPI  <br/> |
|Нет  <br/> |
|Other (другие)  <br/> |
|Вставить  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a>Ошибка операции AddEntityFeedback ответа

Коды ошибок, которые являются общими для веб-служб Exchange в разделе [ResponseCode](responsecode.md).
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>Пример AddEntityFeedback в сочетании с FindPeople

#### <a name="findpeople-request"></a>Запрос на FindPeople
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

#### <a name="findpeople-response"></a>FindPeople ответа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <FindPeopleResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <People>
                <Persona xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

#### <a name="addentityfeedback-request"></a>Запрос на AddEntityFeedback

```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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
> С помощью FindPeople код ответа транзакций в качестве транзакций запрос AddEntityFeedback по идентификатору. 
  
#### <a name="addentityfeedback-response"></a>AddEntityFeedback ответа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" MinorVersion="1" MajorBuildNumber="302" MinorBuildNumber="0" Version="V2_68" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body>
        <AddEntityFeedbackResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
            <ResponseCode>NoError</ResponseCode>
            <ErrorCount>0</ErrorCount>
            <ErrorDetails />
        </AddEntityFeedbackResponse>
    </s:Body>
</s:Envelope>

```


