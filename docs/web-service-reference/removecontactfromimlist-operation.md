---
title: Операция RemoveContactFromImList
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: Поиск сведений о RemoveContactFromImListной операции EWS.
ms.openlocfilehash: 8b3d83a0b53bad169d9f3478540e5087901f3a12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458469"
---
# <a name="removecontactfromimlist-operation"></a>Операция RemoveContactFromImList

Поиск сведений о **RemoveContactFromImListной** операции EWS. 
  
Операция **RemoveContactFromImList** удаляет контакты из списка мгновенных сообщений LYNC (IM), когда Lync использует Exchange для хранилища контактов. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-removecontactfromimlist-operation"></a>Использование операции RemoveContactFromImList

Операция **RemoveContactFromImList** принимает один аргумент, который определяет контакт, который необходимо удалить из списка контактов Lync, хранящегося на сервере Exchange. Список контактов, для которых предназначена эта операция, называется **Контакты Lync** в Outlook 2013. 
  
> [!CAUTION]
> Не используйте [операцию DeleteItem](deleteitem-operation.md) для удаления контактов из списка контактов. Для поддержки удаления контакта из списка **контактов Lync** может потребоваться дополнительная обработка на стороне сервера. Обратите внимание, что список **контактов Lync** является концептуальным эквивалентом стандартной папки почтовых ящиков **контактов Lync** . 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a>Заголовки SOAP операции RemoveContactFromImList

Операция **RemoveContactFromImList** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a>Пример запроса операции RemoveContactFromImList: Удаление контакта из списка контактов Lync

В следующем примере запроса операции **RemoveContactFromImList** показано, как удалить контакт из списка **контактов Lync** . Операция **RemoveContactFromImList** принимает один уникальный идентификатор контакта для идентификации контакта, который удален из списка **контактов Lync** . 
  
> [!NOTE]
> Все идентификаторы элементов и изменения ключей в этой статье были сокращены, чтобы сохранить удобочитаемость. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

В теле SOAP запроса используются следующие элементы:
  
- [RemoveContactFromImList](removecontactfromimlist.md)
    
- [ContactId](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a>Успешный отклик операции RemoveContactFromImList

В следующем примере показан успешный ответ на запрос операции **RemoveContactFromImList** для удаления контакта из списка **контактов Lync** . 
  
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
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

В теле SOAP отклика используются следующие элементы:
  
- [ремовеконтактфромимлистреспонсе](removecontactfromimlistresponse.md)
    
- [респонсекоде](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a>Ответ об ошибке операции RemoveContactFromImList

В следующем примере показан ответ об ошибке для запроса операции **RemoveContactFromImList** . Это ответ на запрос на удаление контакта из списка **контактов Lync** , когда контакт больше не существует в списке. 
  
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
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

В теле SOAP отклика об ошибке используются следующие элементы:
  
- [ремовеконтактфромимлистреспонсе](removecontactfromimlistresponse.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetImItemList](getimitemlist-operation.md)
    

