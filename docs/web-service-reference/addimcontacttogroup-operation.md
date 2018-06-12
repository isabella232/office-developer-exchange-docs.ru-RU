---
title: Операция AddImContactToGroup
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 376acc42-2684-4596-aca1-82a4a10865c9
description: Найдите сведения о веб-служб Exchange AddImContactToGroup операции.
ms.openlocfilehash: 669d798b6cabc1cab1fc057a3e18c565467440f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761336"
---
# <a name="addimcontacttogroup-operation"></a>Операция AddImContactToGroup

Найдите сведения о **AddImContactToGroup** операции веб-служб Exchange. 
  
Операции веб-служб Exchange (EWS) **AddImContactToGroup** Добавляет существующий контакт, обмен мгновенными сообщениями (IM) в группу. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-addimcontacttogroup-operation"></a>С помощью операции AddImContactToGroup

Операция **AddImContactToGroup** может принимать только служб обмена мгновенными сообщениями. Если вы хотите добавить новый контакт обмена мгновенными Сообщениями единого хранилища контактов, с помощью операции [AddNewImContactToGroup](addnewimcontacttogroup-operation.md) . 
  
Операция **AddImContactToGroup** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
**В таблице 1. Заголовки SOAP AddImContactToGroup операции**

|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении. Этот заголовок можно применять к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику. Этот заголовок можно применять к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="addimcontacttogroup-operation-request-example-add-an-existing-im-contact-to-an-im-group"></a>Пример запроса AddImContactToGroup операции: Добавление существующего обмена мгновенными Сообщениями обратитесь к группе обмена мгновенными Сообщениями

Приведенный ниже запрос операции **AddImContactToGroup** показано, как добавить существующий контакт обмена мгновенными Сообщениями с группой обмена мгновенными Сообщениями. 
  
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
      <m:AddImContactToGroup>
         <m:ContactId Id="AAMkAGQ1MjJjMTBkLTc4Y2AA="
                      ChangeKey="EQAAABYAAABtF8oI7i"/>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkzzAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

Запрос SOAP body содержит следующие элементы:
  
- [AddImContactToGroup](addimcontacttogroup.md)
    
- [ContactId](contactid.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-addimcontacttogroup-operation-response"></a>Успешные операции ответа AddImContactToGroup

В следующем примере показано успешного ответа на запрос операции **AddImContactToGroup** . 
  
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
      <AddImContactToGroupResponse ResponseClass="Success" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </AddImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

Ответ SOAP body содержит следующие элементы:
  
- [AddImContactToGroupResponse](addimcontacttogroupresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="addimcontacttogroup-operation-errorinvalidimcontactid-error-response"></a>Операция AddImContactToGroup ErrorInvalidImContactId ошибка ответа

В следующем примере показано ошибочный ответ на запрос операции **AddImContactToGroup** . Приведенный ниже ответ ошибка возникает при попытке добавить контакт, который не является для обмена мгновенными Сообщениями контакта. 
  
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
      <AddImContactToGroupResponse ResponseClass="Error" 
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Contact Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImContactId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         </AddImContactToGroupResponse>
      </s:Body>
</s:Envelope>
```

Ошибка ответ SOAP body содержит следующие элементы:
  
- [AddImContactToGroupResponse](addimcontacttogroupresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операция AddImGroup](addimgroup-operation.md)
    
- [Операция AddNewImContactToGroup](addnewimcontacttogroup-operation.md)
    
- [Операция SetImGroup](setimgroup-operation.md)
    
- [Операция RemoveImGroup](removeimgroup-operation.md)
    
- [Операция GetImItemList](getimitemlist-operation.md)
    
- [Пользователи и контакты в EWS для Exchange](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

