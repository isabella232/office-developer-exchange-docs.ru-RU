---
title: Операция ArchiveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: Поиск сведений о ArchiveItemной операции EWS.
ms.openlocfilehash: d1e18122e67c36babbc8bf01d305309e2b17b568
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463435"
---
# <a name="archiveitem-operation"></a>Операция ArchiveItem

Поиск сведений о **ArchiveItemной** операции EWS. 
  
Операция **ArchiveItem** перемещает элемент в архивный почтовый ящик пользователя почтового ящика. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-archiveitem-operation"></a>Использование операции ArchiveItem

Операция **ArchiveItem** использует в запросе два аргумента, которые определяют элементы для перемещения в архивный почтовый ящик и конечную папку для этих элементов. Чтобы эта операция работала, необходимо включить архивный почтовый ящик. Сведения о том, как включить архивный почтовый ящик, можно найти [в разделе Управление архивами на месте](https://technet.microsoft.com/library/jj651146.aspx).
  
### <a name="archiveitem-operation-soap-headers"></a>Заголовки SOAP операции ArchiveItem

Операция **ArchiveItem** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, как определено в RFC 3066 **теги для идентификации языков**, которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a>Пример запроса операции ArchiveItem: перемещение элемента в архивную папку "Входящие"

В следующем примере запроса операции **ArchiveItem** показано, как переместить элемент в архивную папку "Входящие". 
  
> [!NOTE]
> Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:ArchiveItem>
         <m:ArchiveSourceFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ArchiveSourceFolderId>
         <m:ItemIds>
            <t:ItemId Id="AQMkG5BBwrQAAAxoAAAA=" ChangeKey="CQAAAHCtAAAAAAB7"/>
         </m:ItemIds>
      </m:ArchiveItem>
   </soap:Body>
</soap:Envelope>
```

Текст SOAP Request содержит следующие элементы:
  
- [ArchiveItem](archiveitem.md)    
- [арчивесаурцефолдерид](archivesourcefolderid.md)    
- [дистингуишедфолдерид](distinguishedfolderid.md)    
- [итемидс](itemids.md)   
- [Идентификатор](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a>Успешный отклик операции ArchiveItem

В следующем примере показан успешный ответ на запрос операции **ArchiveItem** для перемещения элемента в архивный почтовый ящик. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [арчивеитемреспонсе](archiveitemresponse.md)    
- [респонсемессажес](responsemessages.md)   
- [арчивеитемреспонсемессаже](archiveitemresponsemessage.md)    
- [респонсекоде](responsecode.md)    
- [Items](items.md)
    
## <a name="archiveitem-operation-error-response"></a>Ответ об ошибке операции ArchiveItem

В следующем примере показан ответ об ошибке для запроса операции **ArchiveItem** . Это ответ на действительный запрос на архивацию элемента, когда архивный почтовый ящик не включен для пользователя. 
  
```xml
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
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Error">
               <m:MessageText>Archive mailbox is not enabled for this user.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [арчивеитемреспонсе](archiveitemresponse.md)    
- [респонсемессажес](responsemessages.md)    
- [арчивеитемреспонсемессаже](archiveitemresponsemessage.md)    
- [мессажетекст](messagetext.md)    
- [респонсекоде](responsecode.md)    
- [дескриптивелинккэй](descriptivelinkkey.md)    
- [Items](items.md)
    
Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).
  
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md) 
- [Архивация в веб-служб Exchange в Exchange](https://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    

