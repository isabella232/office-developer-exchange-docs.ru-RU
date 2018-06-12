---
title: Добавление и удаление адреса электронной почты в списке заблокированных отправителей с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b88288ee-6af7-45b5-a55c-5929cd0c16f1
description: Узнайте, как использовать управляемый API EWS или веб-служб Exchange для адресов электронной почты, чтобы добавлять и удалять их в списке заблокированных отправителей.
ms.openlocfilehash: c03ed585ebd62802000179d8c837786ba5f9aab4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760957"
---
# <a name="add-and-remove-email-addresses-from-the-blocked-senders-list-by-using-ews-in-exchange"></a>Добавление и удаление адреса электронной почты в списке заблокированных отправителей с помощью веб-служб Exchange в Exchange

Узнайте, как использовать управляемый API EWS или веб-служб Exchange для адресов электронной почты, чтобы добавлять и удалять их в списке заблокированных отправителей.
  
Список заблокированных отправителей в окне Параметры нежелательной почты пользователя предоставляет способ для перемещения всех сообщений электронной почты из указанного отправителей в папку нежелательной почты. Можно включить управляемый API EWS или приложение веб-служб Exchange, адреса электронной почты, чтобы добавить или удалить их из списка заблокированных отправителей.
  
Обратите внимание, что сообщение от адреса электронной почты должен существовать в почтовом ящике пользователя вы можете добавить адрес электронной почты или удалить его из списка заблокированных отправителей. Управляемый API EWS [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) метод и операции EWS [MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) используйте коллекцию идентификаторов элементов. Элемент идентификаторы в коллекции указывают сообщений в почтовый ящик, для которого следует изменить состояние нежелательной почты. 
  
Прямой доступ к списку заблокированных отправителей можно использовать командлеты [Get-mailboxjunkemailconfiguration служит](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx) и [Set-mailboxjunkemailconfiguration служит](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) командной консоли Exchange. 
  
## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-the-ews-managed-api"></a>Адрес электронной почты, чтобы добавить или удалить его из списка заблокированных отправителей с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_AddRemoveEWSMA"> </a>

Чтобы добавить отправителя сообщения электронной почты в список заблокированных отправителей, используйте метод **MarkAsJunk** и установите для параметра **isJunk** значение **true**. Чтобы удалить отправителя сообщения электронной почты в списке заблокированных отправителей, установите для параметра **isJunk** значение **false**.
  
Следующем примере показано, как использовать метод **MarkAsJunk** для изменения нежелательной состояние сообщения. 
  
```cs
private static void MarkMessageAsJunk(ExchangeService service, ItemId messageId, bool isJunk, bool moveItem)
{
    List<ItemId> junkItemIds = new List<ItemId>();
    junkItemIds.Add(messageId);
    ServiceResponseCollection<MarkAsJunkResponse> responseCollection = null;
    try
    {
        // If isJunk is true, the sender of the email message is added to 
        // the Blocked Senders List. If isJunk is false, the sender is removed
        // from the list (if present).
        responseCollection = service.MarkAsJunk(junkItemIds, isJunk, moveItem);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error marking item as junk: {0}", ex.ErrorCode);
        return;
    }
    foreach (MarkAsJunkResponse response in responseCollection)
    {
        if (response.Result == ServiceResult.Success)
        {
            Console.WriteLine("Successfully marked message as {0}junk.", isJunk ? "": "NOT ");
            if (moveItem)
            {
                Console.WriteLine("New item ID: {0}", response.MovedItemId.ToString());
            }
        }
        else
        {
            Console.WriteLine("[{0}]: {1}", response.Result.ToString(),
                response.ErrorCode.ToString());
        }
    }
}
```

## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-ews"></a>Адрес электронной почты, чтобы добавить или удалить его из списка заблокированных отправителей с помощью веб-служб Exchange
<a name="bk_AddRemoveEWS"> </a>

Следующий запрос SOAP веб-служб Exchange помечает элемент как нежелательная почта, задав атрибут **IsJunk** на элемент [MarkAsJunk](http://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) значение **true**. Он также перемещает сообщение в папку нежелательной почты, задав атрибут **MoveItem** на элемент **MarkAsJunk** значение **true**.
  
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
        <t:ItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAENAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEuAAA=" 
            ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAADi" />
      </m:ItemIds>
    </m:MarkAsJunk>
  </soap:Body>
</soap:Envelope>
```

Приведенный ниже ответ SOAP веб-служб Exchange показывает успешного ответа. Элемент [MovedItemId](http://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) в ответе содержит идентификатор элемента для элемента, после был перемещен. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:MovedItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEbAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59DIAAA="
              ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59E+" />
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>См. также

- [Управление папкой "Входящие" и веб-службы Exchange](inbox-management-and-ews-in-exchange.md)   
- [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)   
- [MarkAsJunk Operation](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)   
- [Get-mailboxjunkemailconfiguration служит](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx)   
- [SET-mailboxjunkemailconfiguration служит](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) 
- [Командная консоль Exchange](../management/exchange-management-shell.md)
    

