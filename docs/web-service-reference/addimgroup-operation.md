---
title: Операция AddImGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: Сведения об операции AddImGroup EWS.
ms.openlocfilehash: 9aba6a22502c1006da06ce4a9bc925f13b5b5100
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544362"
---
# <a name="addimgroup-operation"></a>Операция AddImGroup

Сведения об операции **AddImGroup** EWS. 
  
Операция **AddImGroup** Exchange веб-служб (EWS) добавляет новую группу мгновенных сообщений (IM) в почтовый ящик. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-addimgroup-operation"></a>Использование операции AddImGroup

Операция **AddImGroup** принимает только один аргумент имени отображения. 
  
Эта операция возвращает имя отображения, тип группы и Exchange хранилище новой группы.
  
В **операции AddImGroup** можно использовать заглавные таблицы SOAP, перечисленные в следующей таблице. 
  
**Таблица 1. Заготчики операции AddImGroup**

|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает. Это применимо к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет культуру, определяемую в RFC 3066 , "Теги для идентификации языков", которая будет использоваться для доступа к почтовому ящику. Это применимо к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Это применимо к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Это применимо к ответу.  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a>Пример запроса на операцию AddImGroup: создание новой группы im

В следующем примере запроса на операцию **AddImGroup** показано, как создать группу im с именем MyCustomerGroup. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Тело SOAP запроса содержит следующие элементы:
  
- [AddImGroup](addimgroup.md)
    
- [DisplayName (string)](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a>Успешный ответ операции AddImGroup

В следующем примере показан успешный ответ на запрос **операции AddImGroup.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="349"
                           MinorBuildNumber="0"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP ответа содержит следующие элементы:
  
- [AddImGroupResponse](addimgroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [ImGroup](imgroup.md)
    
- [DisplayName (string)](displayname-string.md)
    
- [GroupType](grouptype.md)
    
- [ExchangeStoreId](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a>Ответ на ошибку операции AddImGroup

В следующем примере показан ответ на ошибку на запрос **операции AddImGroup.** Это ответ на запрос, содержащий символ, который не может использоваться в имени отображения. Обратите внимание, что это ошибка SOAP, а не сообщение об ошибке на основе схемы. Отображаемая в запросе фамилия — ~!@#$%^ и ошибка возникает &amp; на &amp; символе. Символ &amp; произошел на 11-й строке и 33-й в полезной нагрузке запроса. Ответ был возвращен с кодом HTTP 500. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

- [Пользователи и контакты в EWS для Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [Операция RemoveImGroup](removeimgroup-operation.md)
    
- [SetImGroup](setimgroup.md)
    

