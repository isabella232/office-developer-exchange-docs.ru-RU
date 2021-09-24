---
title: Операция MarkAsJunk
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Сведения об операции MarkAsJunk EWS.
ms.openlocfilehash: b165b415ce9380846b49d15dd321bfddba72b749
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524737"
---
# <a name="markasjunk-operation"></a>Операция MarkAsJunk

Сведения об операции **MarkAsJunk** EWS. 
  
Операция **MarkAsJunk добавляет** и удаляет пользователей из заблокированного списка электронной почты и перемещает сообщения электронной почты в папку нежелательной почты. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-markasjunk-operation"></a>Использование операции MarkAsJunk

Операция **MarkAsJunk** содержит два параметра Boolean, чтобы указать, следует ли добавить отправитель электронной почты в заблокированный список отправитель и следует ли перенаправлять целевое сообщение электронной почты в папку нежелательной почты по умолчанию или папку Входящие. Действия определяются значениями атрибутов **IsJunk** и **MoveItem.** Ниже возможен вариант действий, основанный на сочетаниях значений для атрибутов **IsJunk** и **MoveItem:** 
  
- Если атрибут **IsJunk** настроен как **true,** а атрибут **MoveItem** — **true,** отправитель целевого сообщения электронной почты добавляется в заблокированный список отправитель, а сообщение электронной почты перемещается в папку нежелательной почты.
    
- Если атрибут **IsJunk** настроен на верное, а атрибут **MoveItem** — ложный, отправитель целевого сообщения электронной почты добавляется в заблокированный список отправитель и сообщение электронной почты не перемещается из папки.
    
- Если для атрибута **IsJunk** установлено ложное, а атрибут  **MoveItem** — true, отправитель целевых сообщений электронной почты удаляется из заблокированного списка отправитель и сообщение электронной почты перемещается в папку "Входящие". 
    
- Если для **атрибута IsJunk** установлено ложное, а атрибут **MoveItem** — ложный, отправитель целевого сообщения электронной почты удаляется из заблокированного списка отправитель и сообщение электронной почты не перемещается из папки.  
    
> [!IMPORTANT]
> Содержимое заблокированного списка отправитель не может быть обнаружено в EWS. Если отправитель добавлен в заблокированный список отправитель, необходимо сохранить копию сообщения электронной почты, отправленного заблокированным отправитель, чтобы разблокировать отправитель в будущем. 
  
### <a name="markasjunk-operation-soap-headers"></a>Заглавы мыла операции MarkAsJunk

В **операции MarkAsJunk** можно использовать заглавные таблицы SOAP, перечисленные в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Определяет пользователя, которого клиентская заявка выдвигает. Этот заглавный заглавник применим к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет культуру, определяемую в RFC 3066 , "Теги для идентификации языков", которая будет использоваться для доступа к почтовому ящику. Этот заглавный заглавник применим к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для запроса на операцию. Этот заглавный заглавник применим к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, отвечаемого на запрос. Этот заглавный заглавник применим к ответу.  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>Пример запроса на операцию MarkAsJunk: Добавление отправитель в список заблокированных отправитель

В следующем примере запроса на операцию **MarkAsJunk** показано, как добавить отправитель электронной почты в заблокированный список отправитель и переместить его в папку нежелательной почты. Операция **MarkAsJunk** принимает уникальный идентификатор сообщения электронной почты для идентификации электронной почты, используемой для ссылки на отправитель, добавленный в список заблокированных отправитель. 
  
> [!NOTE]
> Для сохранения читаемости сокращены все идентификаторы элементов и ключи изменений в этой статье. 
  
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

Тело SOAP запроса содержит следующие элементы:
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>Успешный ответ операции MarkAsJunk

В следующем примере показан успешный ответ на запрос операции **MarkAsJunk,** чтобы добавить отправитель в заблокированный список отправитель и переместить сообщение электронной почты в папку нежелательной почты. 
  
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

Тело SOAP ответа содержит следующие элементы:
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [MovedItemId](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>Пример запроса на операцию MarkAsJunk: Удаление отправитель из заблокированного списка отправитель

В следующем примере запроса операции **MarkAsJunk** показано, как удалить отправитель сообщения электронной почты из заблокированного списка отправитель и переместить сообщение электронной почты в папку "Входящие". Чтобы удалить отправитель из заблокированного списка отправитель, необходимо сохранить сообщение электронной почты, отправленное заблокированным отправитером. Адрес электронной почты отправщика связан с сообщениями электронной почты, отправленными отправителю. Удаление отправитель из заблокированного списка отправитель не удастся, если эталонное сообщение электронной почты больше не существует в почтовом ящике пользователя. Идентификатор элемента, используемый для связывать сообщение электронной почты с отправитером, должен быть связан с элементом, который существует в Exchange почтовом ящике. Рекомендуется создать скрытую папку для хранения элементов, отправленных ранее заблокированными отправителями, чтобы отправители могли быть разблокированы из клиентского приложения. Если элемент удален из почтового ящика Exchange, администратору необходимо использовать консоль управления Exchange для доступа к заблокированным спискам отправитель, чтобы удалить отправитель из списка. Сведения о том, как разблокировать пользователя с помощью консоль управления Exchange, см. в пункте How [to configure the safe senders and blocked senders settings in Office 365.](https://support.microsoft.com/kb/2545137)
  
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

Успешный ответ для удаления отправитель из заблокированного списка отправитель такой же, как и ответ для добавления отправитель в заблокированный список отправитель.
  
Тело SOAP запроса содержит следующие элементы:
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>Ответ на ошибку операции MarkAsJunk

В следующем примере показан ответ на ошибку на запрос **операции MarkAsJunk.** Это ответ на запрос добавить или удалить отправитель из заблокированного списка отправитель, когда сообщения электронной почты, указанные идентификатором элемента, больше не существует в почтовом ящике. 
  
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

Тело SOAP ответа на ошибку содержит следующие элементы:
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операция GetItem](getitem-operation.md) Операция GetItem 
    
- [Операция FindItem](finditem-operation.md)
    

