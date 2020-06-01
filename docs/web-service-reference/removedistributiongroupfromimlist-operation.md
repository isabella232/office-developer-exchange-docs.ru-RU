---
title: Операция RemoveDistributionGroupFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: Поиск сведений о RemoveDistributionGroupFromImListной операции EWS.
ms.openlocfilehash: 66220f0cab99f404e17136bbb7836ca13d569b53
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459604"
---
# <a name="removedistributiongroupfromimlist-operation"></a>Операция RemoveDistributionGroupFromImList

Поиск сведений о **RemoveDistributionGroupFromImListной** операции EWS. 
  
Операция **RemoveDistributionGroupFromImList** удаляет группу рассылки из списка мгновенных сообщений LYNC (IM), когда Lync использует Exchange для хранилища контактов. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a>Использование операции RemoveDistributionGroupFromImList

Операция **RemoveDistributionGroupFromImList** принимает один аргумент, определяющий группу рассылки, которую необходимо удалить из списка обмена мгновенными сообщениями Lync, хранящегося на сервере Exchange. 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a>Заголовки SOAP операции RemoveDistributionGroupFromImList

Операция **RemoveDistributionGroupFromImList** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a>Пример запроса операции RemoveDistributionGroupFromImList: Удаление группы рассылки из списка обмена мгновенными сообщениями

В следующем примере запроса операции **RemoveDistributionGroupFromImList** показано, как удалить группу рассылки из группы обмена мгновенными сообщениями. Операция **RemoveDistributionGroupFromImList** принимает уникальный идентификатор группы, чтобы определить группу рассылки, которую требуется удалить из списка обмена мгновенными сообщениями. Элемент [ексчанжестореид](exchangestoreid.md) , который возвращается в ответе для [операции GetImItemList](getimitemlist-operation.md) , и [Операция AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md) идентифицирует группы рассылки, которые можно удалить из списка мгновенных сообщений. 
  
> [!NOTE]
> Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость. 
  
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

В теле SOAP запроса используются следующие элементы:
  
- [RemoveDistributionGroupFromImList](removedistributiongroupfromimlist.md)
    
- [GroupId](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a>Успешный отклик операции RemoveDistributionGroupFromImList

В следующем примере показан успешный ответ на запрос операции **RemoveDistributionGroupFromImList** для удаления группы рассылки из группы обмена мгновенными сообщениями. 
  
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

В теле SOAP отклика используются следующие элементы:
  
- [ремоведистрибутионграупфромимлистреспонсе](removedistributiongroupfromimlistresponse.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a>Пример ответа на сообщение об ошибке операции RemoveDistributionGroupFromImList

В следующем примере показан ответ об ошибке для запроса операции **RemoveDistributionGroupFromImList** . Это ответ на запрос на удаление группы рассылки, которая уже удалена из почтового ящика. 
  
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

В теле SOAP отклика об ошибке используются следующие элементы:
  
- [ремоведистрибутионграупфромимлистреспонсе](removedistributiongroupfromimlistresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetImItemList](getimitemlist-operation.md)
    
- [Операция AddDistributionGroupToImList](adddistributiongrouptoimlist-operation.md)
    
- [Пользователи и контакты в EWS для Exchange](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

