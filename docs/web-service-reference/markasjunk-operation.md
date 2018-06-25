---
title: MarkAsJunk Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: Найдите сведения о веб-служб Exchange MarkAsJunk операции.
ms.openlocfilehash: b9d79e6fbec87ce41030b4981f3c16f2f9ce9507
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834353"
---
# <a name="markasjunk-operation"></a>MarkAsJunk Operation

Найдите сведения о **MarkAsJunk** операции веб-служб Exchange. 
  
Операция **MarkAsJunk** добавляет и удаление пользователей из списка заблокированных электронной почты и перемещает сообщения электронной почты в папку нежелательной почты. 
  
Эта операция появилась в Exchange Server 2013.
  
## <a name="using-the-markasjunk-operation"></a>С помощью операции MarkAsJunk

Операция **MarkAsJunk** содержит два типа Boolean вариантов, чтобы указать ли будет добавлен в список заблокированных отправителей электронной почты отправителя и является ли целевой для сообщения электронной почты необходимо переместить папку нежелательной почты по умолчанию или к папке "Входящие". Действия определяются по значениям **IsJunk** и **MoveItem** атрибуты. Ниже приведены возможные действия в зависимости от комбинации значений атрибутов **IsJunk** и **MoveItem** . 
  
- Если атрибут **IsJunk** имеет значение **true**, а атрибут **MoveItem** имеет значение **true**, отправителя сообщения электронной почты конечного добавляется в список заблокированных отправителей, и сообщение электронной почты перемещается в папку нежелательной Dmail.
    
- Если атрибут **IsJunk** имеет значение **true**, а атрибут **MoveItem** присвоено **значение false**, отправителя сообщения электронной почты конечного добавляется в список заблокированных отправителей, и сообщение электронной почты не перемещается из папки.
    
- Если атрибут **IsJunk** имеет значение **false**, а **MoveItem** атрибут имеет значение **true**, отправителя конечного messageis электронной почты, удаляется из списка заблокированных отправителей, и сообщение электронной почты перемещается в папку "Входящие".
    
- Если атрибут **IsJunk** имеет значение **false**, а атрибут **MoveItem** присвоено **значение false**, отправителя сообщения электронной почты конечного удаляется из списка заблокированных отправителей, и сообщение электронной почты не перемещается из папки.
    
> [!IMPORTANT]
> Содержимое списка заблокированных отправителей не доступные из веб-служб Exchange. Если отправитель добавляется в список заблокированных отправителей, необходимо сохранить копию сообщения электронной почты, отправленные с заблокированных отправителей разблокирование отправителя в будущем. 
  
### <a name="markasjunk-operation-soap-headers"></a>Заголовки SOAP MarkAsJunk операции

Операция **MarkAsJunk** можно использовать заголовки SOAP, которые перечислены в следующей таблице. 
  
|**Имя заголовка**|**Элемент**|**Описание**|
|:-----|:-----|:-----|
|**Олицетворение** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |Идентифицирует пользователя, которого олицетворения в клиентском приложении. Этот заголовок можно применять к запросу.  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |Определяет язык и региональные параметры, как определено в RFC 3066, «Теги для идентификации языков», который будет использоваться для доступа к почтовому ящику. Этот заголовок можно применять к запросу.  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |Определяет версию схемы для операции запроса. Этот заголовок можно применять к запросу.  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |Определяет версию сервера, ответившего на запрос. Этот заголовок можно применять, чтобы получить ответ.  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>Пример запроса MarkAsJunk операции: Добавление отправителя в список заблокированных отправителей

В следующем примере запрос операции **MarkAsJunk** показано, как добавить отправителя сообщения электронной почты в список заблокированных отправителей и перемещать сообщения электронной почты в папку нежелательной почты. Операция **MarkAsJunk** принимает идентификатор сообщения уникальные электронной почты для идентификации электронной почты, который используется для ссылки отправителя, который добавляется в список заблокированных отправителей. 
  
> [!NOTE]
> Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость. 
  
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
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

Запрос SOAP body содержит следующие элементы:
  
- [MarkAsJunk](markasjunk.md)
    
- [Что ItemID](itemids.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>Успешные операции ответа MarkAsJunk

В следующем примере показано успешного ответа на запрос операции **MarkAsJunk** добавить отправителя в список заблокированных отправителей и перемещение сообщений электронной почты в папку нежелательной почты. 
  
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
        <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Ответ SOAP body содержит следующие элементы:
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [MovedItemId](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>Пример запроса MarkAsJunk операции: удаление отправителя в список заблокированных отправителей

В следующем примере запрос операции **MarkAsJunk** показано, как удалить отправителя сообщения электронной почты из списка заблокированных отправителей и перемещение сообщений электронной почты в папке "Входящие". Необходимо хранить сообщения электронной почты, отправленные с заблокированных отправителей, чтобы удалить отправителя из списка заблокированных отправителей. Адрес электронной почты отправителя связан с сообщениями электронной почты, отправленные отправителем. Удаление отправителя в список заблокированных отправителей не выполняется, если сообщение электронной почты ссылку больше не существует в почтовом ящике пользователя. Идентификатор элемента, который используется для связи с его отправителю сообщения электронной почты должен быть связан с элементом, который существует в почтовом ящике Exchange. Рекомендуется создать скрытые папки для хранения элементов, отправленных ранее заблокированных отправителей, чтобы отправители может быть заблокирован из клиентского приложения. В случае, если элемент был удален из почтового ящика Exchange, администратор должен использовать консоль управления Exchange для доступа к списку заблокированных отправителей для удаления отправителя из списка. Сведения о том, как разблокировать пользователя с помощью консоли управления Exchange, в [Настройка надежных отправителей и заблокированных отправителей параметры в Office 365](http://support.microsoft.com/kb/2545137).
  
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
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

Успешного ответа для удаления отправителя в список заблокированных отправителей — это то же, что ответ на добавление отправителя в список заблокированных отправителей.
  
Запрос SOAP body содержит следующие элементы:
  
- [MarkAsJunk](markasjunk.md)
    
- [Что ItemID](itemids.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>Ошибка операции MarkAsJunk ответа

В следующем примере показано ошибочный ответ на запрос операции **MarkAsJunk** . Это ответ на запрос для добавления или удаления отправителя в списке заблокированных отправителей, когда сообщение электронной почты, указанного идентификатором идентификатор элемента больше не существует в почтовом ящике. 
  
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
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Ошибка ответ SOAP body содержит следующие элементы:
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также

- [Операции EWS в Exchange](ews-operations-in-exchange.md)
    
- [Операции GetItem](getitem-operation.md) Операции GetItem 
    
- [FindItem Operation](finditem-operation.md)
    

