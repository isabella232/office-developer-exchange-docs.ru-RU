---
title: Операция Аддентитифидбакк
manager: luken
ms.date: 4/18/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 00e40197-5794-4268-b937-bd65aa044890
description: Операция Аддентитифидбакк возвращает сведения об ошибке, соответствующие проблемам на стороне сервера.
ms.openlocfilehash: a1027a0a1ee06cf3e83833b1d84c13d77b07c0b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458441"
---
# <a name="addentityfeedback-operation"></a>Операция Аддентитифидбакк

Операция **аддентитифидбакк** возвращает сведения об ошибке, соответствующие проблемам на стороне сервера. 
  
Эта операция зависит от типа регистрируемого события. Одно из наиболее важных событий — **ентитяддед**, которое соответствует выбранному объекту. Эта операция является пакетной, поэтому ее можно использовать для записи пакетов записей в один запрос. 
  
## <a name="findpeople-request-examples"></a>Примеры запросов FindPeople

Операция **аддентитифидбакк** предоставляет клиентам возможность заносить в журнал сведения о взаимодействии с сущностями, возвращенными службой. Его можно использовать в качестве сигнала, чтобы увеличить релевантность для каждого клиента. Например, клиенты могут использовать эту операцию для предоставления отзывов о сущностях людей, возвращенных из **FindPeople**.
  
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

### <a name="the-request-soap-body-contents"></a>Содержимое SOAP в тексте запроса

SOAP – запрос содержит один элемент **ентитифидбаккентриес**. Это, в свою очередь, содержит массив объектов **ентитифидбаккентри** . Каждая запись в массиве может содержать следующие элементы. 
  
|**Параметры запроса**|**Обязательный**|**Описание**|**Тип**|
|:-----|:-----|:-----|:-----|
|**клиентевенттимеутк** <br/> |Да  <br/> |Время в формате UTC, в котором произошло событие на стороне клиента.  <br/> |DateTime  <br/> |
|**клиентевенттимелокал** <br/> |Да  <br/> |Местное время, в течение которого событие произошло на стороне клиента.  <br/> |DateTime  <br/> |
|**ClientId** <br/> |Да  <br/> |Тип клиента (например, Outlook, OWA и т. д.).  <br/> |Перечисление Клиентидтипе  <br/> |
|**клиентсессионид** <br/> |Да  <br/> |GUID, определяющий идентификатор сеанса. Создается на клиенте.  <br/> |Идентификатор GUID  <br/> |
|**ClientVersion** <br/> |Да  <br/> |Версия клиента (например, 15.01.0101.000).  <br/> |String  <br/> |
|**ентитяддсаурце** <br/> |Нет  <br/> |Источник для Ентитядед (например, Ентитирелеванцеапи, типы, вставленные).  <br/> |Перечисление Ентитяддсаурце  <br/> |
|**ентрисекуенценумбер** <br/> |Да  <br/> |Добавочное целое число на каждый сеанс клиента. Используется для обнаружения потери данных.  <br/> |Целое  <br/> |
|**EventType** <br/> |Да  <br/> |Тип события (например, добавленная сущность, Удаленная сущность).  <br/> |String  <br/> |
|**жсонпропертибаг** <br/> |Нет  <br/> |Дополнительные свойства, связанные с событием (BLOB-объект JSON пар "ключ-значение").  <br/> |Большой двоичный объект JSON  <br/> |
|**таржетентитилист** <br/> |Нет  <br/> |Список сущностей, связанных с событием.  <br/> |Строка JSON  <br/> |
|**трансактионид** <br/> |Нет  <br/> |ID (GUID), который сопоставляет идентификатор в журналах запросов.  <br/> |String  <br/> |
   
### <a name="successful-addentityfeedback-operation-response"></a>Успешный отклик операции Аддентитифидбакк

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

### <a name="the-response-soap-body-contains-the-following-elements"></a>Основной текст SOAP отклика содержит указанные ниже элементы.

#### <a name="errors"></a>Ошибки 
  
API может заносить в журнал пакет записей отзывов, которые мы можем выполнить. В этом поле представлено количество ошибочных операций, которые не были занесены в журнал.
    
#### <a name="errordetails"></a>еррордетаилс
  
Сведения, относящиеся к ошибкам, приведенным выше в разделе `;` .
    
### <a name="currently-supported-values"></a>Текущие поддерживаемые значения

|**Перечисление Клиентидтипе**|
|:-----|
|Desktop  <br/> |
|Exchange  <br/> |
|IMAP4  <br/> |
|Lync  <br/> |
|макмаил  <br/> |
|макаутлук  <br/> |
|Mobile  <br/> |
|Другое  <br/> |
|Outlook  <br/> |
|Откройте файл outlookservice  <br/> |
|Служба  <br/> |
|Tablet  <br/> |
|Web  <br/> |
   
|**Перечисление Ентитяддсаурце**|
|:-----|
|ActiveDirectory  <br/> |
|ентитирелеванцеапи  <br/> |
|ентитирелеванцеапикаче  <br/> |
|експлиЦиттипинг  <br/> |
|локалкаче  <br/> |
|локалкачеандентитирелеванцеапи  <br/> |
|Нет  <br/> |
|Другое  <br/> |
|Вставить  <br/> |
   
### <a name="addentityfeedback-operation-error-response"></a>Ответ об ошибке операции Аддентитифидбакк

Коды ошибок, являющиеся общими для EWS, представлены в разделе [респонсекоде](responsecode.md).
  
### <a name="example-of-addentityfeedback-in-conjunction-with-findpeople"></a>Пример Аддентитифидбакк в сочетании с FindPeople

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

#### <a name="addentityfeedback-request"></a>Запрос Аддентитифидбакк

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
> Использование идентификатора транзакции ответа FindPeople в качестве идентификатора транзакции запроса Аддентитифидбакк. 
  
#### <a name="addentityfeedback-response"></a>Ответ Аддентитифидбакк

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


