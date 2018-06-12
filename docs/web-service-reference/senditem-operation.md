---
title: SendItem Operation
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
description: Операция SendItem используется для отправки сообщений электронной почты, расположенные в хранилище Exchange.
ms.openlocfilehash: 780778b1599d0d5e5f4b6e5b58b67773bbe18cda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835336"
---
# <a name="senditem-operation"></a><span data-ttu-id="bfdb9-103">SendItem Operation</span><span class="sxs-lookup"><span data-stu-id="bfdb9-103">SendItem operation</span></span>

<span data-ttu-id="bfdb9-104">Операция SendItem используется для отправки сообщений электронной почты, расположенные в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-104">The SendItem operation is used to send e-mail messages that are located in the Exchange store.</span></span>
  
## <a name="senditem-e-mail-message-request-example"></a><span data-ttu-id="bfdb9-105">Пример запроса SendItem (сообщения электронной почты)</span><span class="sxs-lookup"><span data-stu-id="bfdb9-105">SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="bfdb9-106">Описание</span><span class="sxs-lookup"><span data-stu-id="bfdb9-106">Description</span></span>

<span data-ttu-id="bfdb9-107">Следующем примере показано, как отправить сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-107">The following example shows how to send an e-mail message.</span></span>
  
### <a name="code"></a><span data-ttu-id="bfdb9-108">Программа</span><span class="sxs-lookup"><span data-stu-id="bfdb9-108">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="bfdb9-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="bfdb9-109">Comments</span></span>

<span data-ttu-id="bfdb9-110">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="bfdb9-111">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="bfdb9-111">Request elements</span></span>

<span data-ttu-id="bfdb9-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bfdb9-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="bfdb9-113">SendItem</span><span class="sxs-lookup"><span data-stu-id="bfdb9-113">SendItem</span></span>](senditem.md)
    
- [<span data-ttu-id="bfdb9-114">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="bfdb9-114">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="bfdb9-115">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="bfdb9-115">ItemId</span></span>](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a><span data-ttu-id="bfdb9-116">Ответ успешные SendItem (сообщения электронной почты)</span><span class="sxs-lookup"><span data-stu-id="bfdb9-116">Successful SendItem (E-mail Message) Response</span></span>

### <a name="description"></a><span data-ttu-id="bfdb9-117">Описание</span><span class="sxs-lookup"><span data-stu-id="bfdb9-117">Description</span></span>

<span data-ttu-id="bfdb9-118">В следующем примере показано успешного ответа SendItem.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-118">The following example shows a successful SendItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="bfdb9-119">Программа</span><span class="sxs-lookup"><span data-stu-id="bfdb9-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="bfdb9-120">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="bfdb9-120">Successful response elements</span></span>

<span data-ttu-id="bfdb9-121">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bfdb9-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="bfdb9-122">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bfdb9-122">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="bfdb9-123">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="bfdb9-123">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="bfdb9-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bfdb9-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bfdb9-125">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bfdb9-125">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="bfdb9-126">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bfdb9-126">ResponseCode</span></span>](responsecode.md)
    
### <a name="comments"></a><span data-ttu-id="bfdb9-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="bfdb9-127">Comments</span></span>

<span data-ttu-id="bfdb9-128">Делегат, который пытается отправить сообщение электронной почты, которая находится в папке «Черновики» участника с SendAndSaveCopy для параметра сохранять копию в отправленные именованной папки выполняться не будут для перемещения копию отправленного элемента отправленные различающееся папка.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-128">A delegate who tries to send an e-mail message that is located in the principal's Drafts folder with the SendAndSaveCopy option set to save a copy in the Sent Items distinguished folder will silently fail to move a copy of the sent item to the Sent Items distinguished folder.</span></span> <span data-ttu-id="bfdb9-129">Элемент будет оставаться в папке «Черновики» участника.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-129">The item will remain in the principal's Drafts folder.</span></span> <span data-ttu-id="bfdb9-130">Для указания основного сервера почтовых ящиков в элементе [DistinguishedFolderId](distinguishedfolderid.md) является способа решения этой проблемы.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-130">The workaround for this issue is to specify the principal's mailbox in the [DistinguishedFolderId](distinguishedfolderid.md) element.</span></span> 
  
<span data-ttu-id="bfdb9-131">Дополнительные сценарии, которые следует учитывать при делегат создает сообщение электронной почты и сохраняет его в папке «Черновики» почтового ящика делегата.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-131">An additional scenario to consider is when a delegate creates an e-mail message and saves it to the Drafts folder of the delegate's mailbox.</span></span> <span data-ttu-id="bfdb9-132">Если делегат пытается отправить элемент и сохранить копию в папку различающееся отправленные участника, сообщение отправляется правильно, остается черновик сообщения в папке «Черновики», делегата, отправленное сообщение не отображается в делегата или участника Папка "Отправленные", а ответ выполнен успешно.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-132">If the delegate tries to send the item and save a copy to the principal's Sent Items distinguished folder, the message is sent correctly, the draft message remains in the delegate's Drafts folder, the sent message does not appear in either the delegate's or principal's Sent Items folder, and the response is a success.</span></span>
  
## <a name="invalid-senditem-e-mail-message-request-example"></a><span data-ttu-id="bfdb9-133">Пример запроса недопустимый SendItem (сообщения электронной почты)</span><span class="sxs-lookup"><span data-stu-id="bfdb9-133">Invalid SendItem (E-mail Message) request example</span></span>

### <a name="description"></a><span data-ttu-id="bfdb9-134">Описание</span><span class="sxs-lookup"><span data-stu-id="bfdb9-134">Description</span></span>

<span data-ttu-id="bfdb9-135">В следующем примере кода показан пример запроса с недопустимым идентификатором.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-135">The following code sample shows an example of a request with an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="bfdb9-136">Программа</span><span class="sxs-lookup"><span data-stu-id="bfdb9-136">Code</span></span>

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a><span data-ttu-id="bfdb9-137">Отклик SendItem (сообщения электронной почты)</span><span class="sxs-lookup"><span data-stu-id="bfdb9-137">SendItem (E-mail Message) error response</span></span>

### <a name="description"></a><span data-ttu-id="bfdb9-138">Описание</span><span class="sxs-lookup"><span data-stu-id="bfdb9-138">Description</span></span>

<span data-ttu-id="bfdb9-139">В следующем примере показано возврату ошибки SendItem-запрос, который содержит недопустимый идентификатор.</span><span class="sxs-lookup"><span data-stu-id="bfdb9-139">The following example shows an error response to a SendItem request that contains an invalid identifier.</span></span>
  
### <a name="code"></a><span data-ttu-id="bfdb9-140">Программа</span><span class="sxs-lookup"><span data-stu-id="bfdb9-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="bfdb9-141">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="bfdb9-141">Error response elements</span></span>

<span data-ttu-id="bfdb9-142">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bfdb9-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="bfdb9-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="bfdb9-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="bfdb9-144">SendItemResponse</span><span class="sxs-lookup"><span data-stu-id="bfdb9-144">SendItemResponse</span></span>](senditemresponse.md)
    
- [<span data-ttu-id="bfdb9-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bfdb9-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bfdb9-146">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bfdb9-146">SendItemResponseMessage</span></span>](senditemresponsemessage.md)
    
- [<span data-ttu-id="bfdb9-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="bfdb9-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="bfdb9-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bfdb9-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bfdb9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bfdb9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="bfdb9-150">См. также</span><span class="sxs-lookup"><span data-stu-id="bfdb9-150">See also</span></span>



[<span data-ttu-id="bfdb9-151">SendItem Operation</span><span class="sxs-lookup"><span data-stu-id="bfdb9-151">SendItem operation</span></span>](senditem-operation.md)
  
 <span data-ttu-id="bfdb9-152">**SendItemType**</span><span class="sxs-lookup"><span data-stu-id="bfdb9-152">**SendItemType**</span></span>


- [<span data-ttu-id="bfdb9-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bfdb9-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

