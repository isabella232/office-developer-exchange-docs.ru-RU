---
title: Операция MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Поиск сведений о MarkAsJunkной операции EWS.
ms.openlocfilehash: 25d6b01dfff64c4e45f3382223311219d349c165
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468574"
---
# <a name="markasjunk-operation"></a>Операция MarkAsJunk

Поиск сведений о **MarkAsJunkной** операции EWS. 
  
Операция **MarkAsJunk** добавляет и удаляет пользователей из списка заблокированных сообщений электронной почты и перемещает сообщения электронной почты в папку "Нежелательная почта". 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-markasjunk-operation"></a>Использование операции MarkAsJunk

Операция **MarkAsJunk** содержит два логических параметра, указывающие, следует ли добавить отправителя электронной почты в список заблокированных отправителей и следует ли переместить целевое сообщение электронной почты в папку нежелательной почты по умолчанию или папку "Входящие". Действия определяются значениями атрибутов **MoveItem** и **нежелательной почты** . Ниже приведены возможные действия, основанные на комбинациях значений для атрибутов **MoveItem** и **нежелательной почты** : 
  
- Если атрибуту InAttribute присвоено значение **true**, **а атрибуту** **MoveItem** присвоено значение **true**, отправитель целевого сообщения электронной почты добавляется в список заблокированных отправителей и сообщение электронной почты перемещается в папку "Нежелательная дмаил".
    
- Если атрибуту InAttribute присвоено значение **true**, **а атрибуту** **MoveItem** присвоено значение **false**, отправитель целевого сообщения электронной почты добавляется в список заблокированных отправителей, а сообщение электронной почты не перемещается из нее.
    
- Если атрибуту InAttribute присвоено значение **false**, **а атрибуту** **MoveItem** присвоено значение **true**, то отправитель целевого сообщения электронной почты удален из списка заблокированных отправителей, а сообщение электронной почты перемещается в папку "Входящие".
    
- Если атрибуту InAttribute присвоено значение **false**, **а атрибуту** **MoveItem** присвоено значение **false**, то отправитель целевого сообщения электронной почты удаляется из списка заблокированных отправителей, а сообщение электронной почты не перемещается из папки.
    
> [!IMPORTANT]
> Содержимое списка заблокированных отправителей не обнаруживается в EWS. Если отправитель добавляется в список заблокированных отправителей, необходимо сохранить копию сообщения электронной почты, отправленного заблокированным отправителем, чтобы разблокировать отправителя в будущем. 
  
### <a name="markasjunk-operation-soap-headers"></a>Заголовки SOAP операции MarkAsJunk

Операция **MarkAsJunk** может использовать заголовки SOAP, указанные в приведенной ниже таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ексчанжеимперсонатион](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, который олицетворяет клиентское приложение. Этот заголовок является применимым для запроса.  <br/> |
|**маилбокскултуре** <br/> |[маилбокскултуре](mailboxculture.md) <br/> |Определяет язык и региональные параметры, определенные в документе RFC 3066 "Теги для идентификации языков", которые будут использоваться для доступа к почтовому ящику. Этот заголовок является применимым для запроса.  <br/> |
|**рекуестверсион** <br/> |[рекуестсерверверсион](requestserverversion.md) <br/> |Определяет версию схемы для запроса операции. Этот заголовок является применимым для запроса.  <br/> |
|**серверверсион** <br/> |[серверверсионинфо](serverversioninfo.md) <br/> |Определяет версию сервера, который ответил на запрос. Этот заголовок является применимым для отклика.  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>Пример запроса операции MarkAsJunk: Добавление отправителя в список заблокированных отправителей

В следующем примере запроса операции **MarkAsJunk** показано, как добавить отправителя электронного письма в список заблокированных отправителей и переместить сообщение в папку нежелательной почты. Операция **MarkAsJunk** принимает уникальный идентификатор электронного сообщения, чтобы определить адрес электронной почты, который используется для ссылки на отправителя, добавляемого в список заблокированных отправителей. 
  
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
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

Текст SOAP Request содержит следующие элементы:
  
- [MarkAsJunk](markasjunk.md)
    
- [итемидс](itemids.md)
    
- [Идентификатор](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>Успешный отклик операции MarkAsJunk

В следующем примере показан успешный ответ на запрос операции **MarkAsJunk** для добавления отправителя в список заблокированных отправителей и перемещения сообщения электронной почты в папку нежелательной почты. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
           <m:ResponseMessages>
               <m:MarkAsJunkResponseMessage ResponseClass="Success">
                  <m:ResponseCode>NoError</m:ResponseCode>
                 <m:MovedItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
               </m:MarkAsJunkResponseMessage>
           </m:ResponseMessages>
        </m:MarkAsJunkResponse>
    </s:Body>
</s:Envelope>
```

Тело SOAP отклика содержит следующие элементы:
  
- [маркасжункреспонсе](markasjunkresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [маркасжункреспонсемессаже](markasjunkresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [моведитемид](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>Пример запроса операции MarkAsJunk: Удаление отправителя из списка заблокированных отправителей

В приведенном ниже примере запроса операции **MarkAsJunk** показано, как удалить отправителя сообщения электронной почты из списка заблокированных отправителей и переместить сообщение в папку "Входящие". Чтобы удалить отправителя из списка заблокированных отправителей, необходимо оставить сообщение электронной почты, отправленное заблокированным отправителем. Адрес электронной почты отправителя связан с сообщениями электронной почты, отправленными отправителями. Удаление отправителя из списка заблокированных отправителей не будет успешным, если справочное сообщение электронной почты больше не существует в почтовом ящике пользователя. Идентификатор элемента, используемый для связи с сообщением электронной почты с отправителями, должен быть связан с элементом, который существует в почтовом ящике Exchange. Рекомендуется создать скрытую папку для хранения элементов, отправленных ранее заблокированными отправителями, чтобы отправители можно было разблокировать из клиентского приложения. В случае, если элемент удален из почтового ящика Exchange, администратору необходимо использовать консоль управления Exchange для доступа к списку заблокированных отправителей, чтобы удалить отправителя из списка. Сведения о том, как разблокировать пользователя с помощью консоли управления Exchange, можно узнать в статье [Настройка параметров надежных отправителей и заблокированных отправителей в Office 365](https://support.microsoft.com/kb/2545137).
  
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
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

Успешный ответ на удаление отправителя из списка заблокированных отправителей совпадает с ответом на Добавление отправителя в список заблокированных отправителей.
  
Текст SOAP Request содержит следующие элементы:
  
- [MarkAsJunk](markasjunk.md)
    
- [итемидс](itemids.md)
    
- [Идентификатор](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>Ответ об ошибке операции MarkAsJunk

В следующем примере показан ответ об ошибке для запроса операции **MarkAsJunk** . Это ответ на запрос на добавление или удаление отправителя из списка заблокированных отправителей, если сообщение электронной почты, заданное идентификатором элемента, больше не существует в почтовом ящике. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

Основной текст сообщения об ошибке SOAP содержит следующие элементы:
  
- [маркасжункреспонсе](markasjunkresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [маркасжункреспонсемессаже](markasjunkresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetItem](getitem-operation.md) Операция GetItem 
    
- [Операция FindItem](finditem-operation.md)
    

