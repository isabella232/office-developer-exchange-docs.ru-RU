---
title: Операция AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Найдите сведения о веб-служб Exchange AddImGroup операции.
ms.openlocfilehash: 91236f9ad2236b3f6bee600b9d57bcf736090ed7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761341"
---
# <a name="addimgroup-operation"></a>Операция AddImGroup

Найдите сведения о **AddImGroup** операции веб-служб Exchange. 
  
Операции веб-служб Exchange (EWS) **AddImGroup** добавляет нового мгновенного обмена мгновенными сообщениями группу в почтовый ящик. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-addimgroup-operation"></a>С помощью операции AddImGroup

Операция **AddImGroup** только принимает аргумент одного отображаемое имя. 
  
Эта операция возвращает отображаемое имя, тип группы и идентификатор хранилища Exchange новой группы.
  
Операция **AddImGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
**В таблице 1. Заголовки SOAP AddImGroup операции**

|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении. Это применимо к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику. Это применимо к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Это применимо к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Это применимо для ответа.  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a>Пример запроса AddImGroup операции: Создание новой группы обмена мгновенными Сообщениями

Приведенный ниже запрос операции **AddImGroup** показано, как создать группу обмена мгновенными Сообщениями с именем MyCustomerGroup. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

Запрос SOAP body содержит следующие элементы:
  
- [AddImGroup](addimgroup.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a>Успешные операции ответа AddImGroup

В следующем примере показано успешного ответа на запрос операции **AddImGroup** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="349"
                           MinorBuildNumber="0"
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

Ответ SOAP body содержит следующие элементы:
  
- [AddImGroupResponse](addimgroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [ImGroup](imgroup.md)
    
- [Отображаемое имя (строка)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a>Ошибка операции AddImGroup ответа

В следующем примере показано ошибочный ответ на запрос операции **AddImGroup** . Это ответ на запрос, который содержит символ, который не может использоваться в поле отображаемое имя. Обратите внимание на то, что это ошибка SOAP и не сообщение об ошибке на основе схемы. Отображаемое имя, отправленными в запросе — ~! @# $% ^&amp;, и возникает ошибка на &amp; символов. &amp; Символ произошло 11 знаков в строке и 33rd в полезных данных запроса. Ответ с кодом HTTP 500. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>См. также

- [Пользователи и контакты в EWS для Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Операция RemoveImGroup](removeimgroup-operation.md)
    
- [SetImGroup](setimgroup.md)
    

