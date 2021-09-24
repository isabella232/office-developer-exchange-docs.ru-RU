---
title: Операция RemoveDistributionGroupFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: Сведения об операции RemoveDistributionGroupFromImList EWS.
ms.openlocfilehash: 52b653008b7b14d2c2467cc9bb1f8f1475cee8f5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513397"
---
# <a name="removedistributiongroupfromimlist-operation"></a>Операция RemoveDistributionGroupFromImList

Сведения об операции **RemoveDistributionGroupFromImList** EWS. 
  
Операция **RemoveDistributionGroupFromImList** удаляет группу рассылки из списка мгновенных сообщений Lync, когда Lync Exchange для магазина контактов. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a>Использование операции RemoveDistributionGroupFromImList

Операция **RemoveDistributionGroupFromImList** принимает один аргумент, который определяет группу рассылки для удаления из списка Lync IM, хранимого на Exchange сервере. 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a>RemoveDistributionGroupFromImList operation SOAP headers

Операция **RemoveDistributionGroupFromImList** может использовать заголовки SOAP, перечисленные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает. Этот заглавный заглавник применим к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет культуру, определяемую в RFC 3066 , "Теги для идентификации языков", которая будет использоваться для доступа к почтовому ящику. Этот заглавный заглавник применим к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a>Пример запроса на операцию RemoveDistributionGroupFromImList: Удаление группы рассылки из списка im

В следующем примере запроса на операцию **RemoveDistributionGroupFromImList** показано, как удалить группу рассылки из группы im. Операция **RemoveDistributionGroupFromImList** принимает уникальный идентификатор группы для идентификации группы рассылки для удаления из списка im. Элемент [ExchangeStoreId,](exchangestoreid.md) возвращаемый в ответ на операцию [GetImItemList](getimitemlist-operation.md) и операцию [AddDistributionGroupToImList,](adddistributiongrouptoimlist-operation.md) определяет группы рассылки, которые можно удалить из списка обмена мгновенными данными. 
  
> [!NOTE]
> Для сохранения читаемости сокращены все идентификаторы элементов и ключи изменений в этой статье. 
  
```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveDistributionGroupFromImList>
         <m:GroupId Id="AAMkADEzO4QrAABmEh5oAAA="/>
      </m:RemoveDistributionGroupFromImList>
   </soap:Body>
</soap:Envelope>
```

В корпусе SOAP запроса используются следующие элементы:
  
- [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a>Успешный ответ на операцию RemoveDistributionGroupFromImList

В следующем примере показан успешный ответ на запрос **операции RemoveDistributionGroupFromImList** для удаления группы рассылки из группы im. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveDistributionGroupFromImListResponse ResponseClass="Success" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

В корпусе SOAP ответа используются следующие элементы:
  
- [RemoveDistributionGroupFromImListResponse](removedistributiongroupfromimlistresponse.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a>RemoveDistributionGroupFromImList operation error response example

В следующем примере показан ответ на ошибку запроса на операцию **RemoveDistributionGroupFromImList.** Это ответ на запрос об удалении группы рассылки, которая уже удалена из почтового ящика. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveDistributionGroupFromImListResponse ResponseClass="Error" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

В корпусе SOAP ответа на ошибки используются следующие элементы:
  
- [RemoveDistributionGroupFromImListResponse](removedistributiongroupfromimlistresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetImItemList](getimitemlist-operation.md)
    
- [Операция AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md)
    
- [Пользователи и контакты в EWS для Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

