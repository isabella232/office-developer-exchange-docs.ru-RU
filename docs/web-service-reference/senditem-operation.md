---
title: Операция SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: 337b89ef-e1b7-45ed-92f3-8abe4200e4c7
description: Операция SendItem используется для отправки сообщений электронной почты, размещенных в хранилище Exchange.
ms.openlocfilehash: 9136379e50723211fe5a483c7f113da4fa125fc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530340"
---
# <a name="senditem-operation"></a><span data-ttu-id="2286e-103">Операция SendItem</span><span class="sxs-lookup"><span data-stu-id="2286e-103">SendItem operation</span></span>

<span data-ttu-id="2286e-104">Операция SendItem используется для отправки сообщений электронной почты, размещенных в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2286e-104">The SendItem operation is used to send e-mail messages that are located in the Exchange store.</span></span>
  
## <a name="senditem-e-mail-message-request-example"></a><span data-ttu-id="2286e-105">Пример запроса SendItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="2286e-105">SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="2286e-106">Description</span><span class="sxs-lookup"><span data-stu-id="2286e-106">Description</span></span>

<span data-ttu-id="2286e-107">В приведенном ниже примере показано, как отправить сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="2286e-107">The following example shows how to send an e-mail message.</span></span>
  
### <a name="code"></a><span data-ttu-id="2286e-108">Код</span><span class="sxs-lookup"><span data-stu-id="2286e-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2286e-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="2286e-109">Comments</span></span>

<span data-ttu-id="2286e-110">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="2286e-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="2286e-111">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="2286e-111">Request elements</span></span>

<span data-ttu-id="2286e-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2286e-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="2286e-113">SendItem</span><span class="sxs-lookup"><span data-stu-id="2286e-113">SendItem</span></span>](senditem.md)
    
- [<span data-ttu-id="2286e-114">итемидс</span><span class="sxs-lookup"><span data-stu-id="2286e-114">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="2286e-115">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="2286e-115">ItemId</span></span>](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a><span data-ttu-id="2286e-116">Успешный ответ SendItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="2286e-116">Successful SendItem (E-mail Message) Response</span></span>

### <a name="description"></a><span data-ttu-id="2286e-117">Description</span><span class="sxs-lookup"><span data-stu-id="2286e-117">Description</span></span>

<span data-ttu-id="2286e-118">В следующем примере показан успешный ответ SendItem.</span><span class="sxs-lookup"><span data-stu-id="2286e-118">The following example shows a successful SendItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="2286e-119">Код</span><span class="sxs-lookup"><span data-stu-id="2286e-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="2286e-120">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="2286e-120">Successful response elements</span></span>

<span data-ttu-id="2286e-121">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2286e-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="2286e-122">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="2286e-122">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2286e-123">сендитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="2286e-123">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="2286e-124">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="2286e-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2286e-125">сендитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="2286e-125">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="2286e-126">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="2286e-126">ResponseCode</span></span>](responsecode.md)
    
### <a name="comments"></a><span data-ttu-id="2286e-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="2286e-127">Comments</span></span>

<span data-ttu-id="2286e-128">Представитель, пытающийся отправить сообщение электронной почты, размещенное в папке "Черновики" основного приложения с параметром SendAndSaveCopy, чтобы сохранить копию в папке "Отправленные", не будет автоматически перемещать копию отправленного элемента в папку "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="2286e-128">A delegate who tries to send an e-mail message that is located in the principal's Drafts folder with the SendAndSaveCopy option set to save a copy in the Sent Items distinguished folder will silently fail to move a copy of the sent item to the Sent Items distinguished folder.</span></span> <span data-ttu-id="2286e-129">Элемент останется в папке "Черновики" основного приложения.</span><span class="sxs-lookup"><span data-stu-id="2286e-129">The item will remain in the principal's Drafts folder.</span></span> <span data-ttu-id="2286e-130">Чтобы устранить эту ошибку, необходимо указать почтовый ящик участника в элементе [дистингуишедфолдерид](distinguishedfolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="2286e-130">The workaround for this issue is to specify the principal's mailbox in the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="2286e-131">Если делегат создает сообщение электронной почты и сохраняет его в папке "Черновики" почтового ящика представителя, необходимо учитывать дополнительный сценарий.</span><span class="sxs-lookup"><span data-stu-id="2286e-131">An additional scenario to consider is when a delegate creates an e-mail message and saves it to the Drafts folder of the delegate's mailbox.</span></span> <span data-ttu-id="2286e-132">Если делегат пытается отправить элемент и сохранить копию в различающейся папке "Отправленные" участника, сообщение отправляется правильно, черновик остается в папке "Черновики" делегата, а отправленное сообщение не будет отображаться в папке "Отправленные" представителя или субъекта "Отправленные", а ответ является успешным.</span><span class="sxs-lookup"><span data-stu-id="2286e-132">If the delegate tries to send the item and save a copy to the principal's Sent Items distinguished folder, the message is sent correctly, the draft message remains in the delegate's Drafts folder, the sent message does not appear in either the delegate's or principal's Sent Items folder, and the response is a success.</span></span>
  
## <a name="invalid-senditem-e-mail-message-request-example"></a><span data-ttu-id="2286e-133">Недопустимый пример запроса SendItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="2286e-133">Invalid SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="2286e-134">Description</span><span class="sxs-lookup"><span data-stu-id="2286e-134">Description</span></span>

<span data-ttu-id="2286e-135">В приведенном ниже примере кода показан пример запроса с недопустимым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="2286e-135">The following code sample shows an example of a request with an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="2286e-136">Код</span><span class="sxs-lookup"><span data-stu-id="2286e-136">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a><span data-ttu-id="2286e-137">Сообщение об ошибке SendItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="2286e-137">SendItem (E-mail Message) error response</span></span>

### <a name="description"></a><span data-ttu-id="2286e-138">Description</span><span class="sxs-lookup"><span data-stu-id="2286e-138">Description</span></span>

<span data-ttu-id="2286e-139">В следующем примере показан ответ об ошибке для запроса SendItem, который содержит недопустимый идентификатор.</span><span class="sxs-lookup"><span data-stu-id="2286e-139">The following example shows an error response to a SendItem request that contains an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="2286e-140">Код</span><span class="sxs-lookup"><span data-stu-id="2286e-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="2286e-141">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="2286e-141">Error response elements</span></span>

<span data-ttu-id="2286e-142">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="2286e-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="2286e-143">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="2286e-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="2286e-144">сендитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="2286e-144">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="2286e-145">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="2286e-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="2286e-146">сендитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="2286e-146">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="2286e-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="2286e-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2286e-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="2286e-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2286e-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="2286e-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="2286e-150">См. также</span><span class="sxs-lookup"><span data-stu-id="2286e-150">See also</span></span>



[<span data-ttu-id="2286e-151">Операция SendItem</span><span class="sxs-lookup"><span data-stu-id="2286e-151">SendItem operation</span></span>](senditem-operation.md)
  
 <span data-ttu-id="2286e-152">**сендитемтипе**</span><span class="sxs-lookup"><span data-stu-id="2286e-152">**SendItemType**</span></span>


- [<span data-ttu-id="2286e-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2286e-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

