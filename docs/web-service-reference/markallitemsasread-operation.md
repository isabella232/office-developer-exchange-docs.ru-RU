---
title: Операция MarkAllItemsAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: Поиск сведений о MarkAllItemsAsReadной операции EWS.
ms.openlocfilehash: 995a6219f0a3b41bddb0d65c875d981322e1ce78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834354"
---
# <a name="markallitemsasread-operation"></a>Операция MarkAllItemsAsRead

Поиск сведений о **MarkAllItemsAsReadной** операции EWS. 
  
Операция **MarkAllItemsAsRead** устанавливает свойство- [Read](isread.md) для всех элементов в одной или нескольких папках, чтобы показать, что все элементы прочитаны или не прочитаны. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-markallitemsasread-operation"></a>Использование операции MarkAllItemsAsRead

С помощью операции **MarkAllItemsAsRead** можно задать свойство- [Read](isread.md) для всех элементов в папках, определенных с помощью идентификатора папки веб-служб Exchange (EWS) или имени папки Exchange по умолчанию. Операция **MarkAllItemsAsRead** также может подавлять отправку уведомлений о прочтении для элементов, помеченных как прочитанные. 
  
### <a name="markallitemsasread-operation-soap-headers"></a>Заголовки SOAP операции MarkAllItemsAsRead

Операция **MarkAllItemsAsRead** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a>Пример запроса операции MarkAllItemsAsRead: Пометка всех элементов в папке как прочитанных

В следующем примере запроса операции **MarkAllItemsAsRead** показано, как задать свойство- [Read](isread.md) , которое также называется флагом чтения, равное **true** всем элементам в папке. В этом примере также показано, что уведомления о прочтении не отправляются в ответ на запросы уведомления о прочтении. 
  
> [!NOTE]
> Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость. Для этой операции не требуются ключи изменения. 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>true</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

Текст SOAP Request содержит следующие элементы:
  
- [MarkAllItemsAsRead](markallitemsasread.md)
    
- [реадфлаг](readflag.md)
    
- [суппрессреадрецеиптс](suppressreadreceipts.md)
    
- [фолдеридс](folderids.md)
    
- [FolderId](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a>Успешный отклик операции MarkAllItemsAsRead

В следующем примере показан успешный ответ на запрос операции **MarkAllItemsAsRead** , чтобы пометить все элементы в папке как прочтенные. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [маркаллитемсасреадреспонсе](markallitemsasreadresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [маркаллитемсасреадреспонсемессаже](markallitemsasreadresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a>Пример запроса операции MarkAllItemsAsRead: Пометка всех элементов в папке как непрочтенных

В приведенном ниже примере запроса операции **MarkAllItemsAsRead** показано, как задать для свойства [читал](isread.md) значение **false** для всех элементов в папке. В этом примере также показано, что уведомления о прочтении не отправляются в ответ на запросы уведомления о прочтении. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>false</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

Успешный ответ на запрос на пометку всех элементов как прочитанных совпадает с ответом на запрос, помечающий все элементы как непрочтенные.
  
Текст SOAP Request содержит следующие элементы:
  
- [MarkAllItemsAsRead](markallitemsasread.md)
    
- [реадфлаг](readflag.md)
    
- [суппрессреадрецеиптс](suppressreadreceipts.md)
    
- [фолдеридс](folderids.md)
    
- [FolderId](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a>Ответ об ошибке операции MarkAllItemsAsRead

В следующем примере показан ответ об ошибке запроса операции **MarkAllItemsAsRead** , чтобы пометить все элементы в папке как прочтенные или непрочтенные, если папка не существует в почтовом ящике. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:MarkAllItemsAsReadResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Error">
               <m:MessageText>The specified object was not found in the store.</m:MessageText>
               <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>

```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [маркаллитемсасреадреспонсе](markallitemsasreadresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [маркаллитемсасреадреспонсемессаже](markallitemsasreadresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция FindFolder](findfolder-operation.md)
    

