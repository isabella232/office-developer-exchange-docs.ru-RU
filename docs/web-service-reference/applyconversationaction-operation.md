---
title: Операция ApplyConversationAction
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: 73d7943d-d361-4f8b-9948-d85f886efa1a
description: Операция ApplyConversationAction задает одноразовый или исполнению действие для всех элементов в беседе. Операция ApplyConversationAction позволяет распределить по категориям, перемещение, копирование, удаление и устанавливать состояние чтения всех элементов в беседе. Действия можно также задать для новых сообщений в беседе.
ms.openlocfilehash: 2a485b84ee87aec2ed807e3f4f0901b83432fa0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761424"
---
# <a name="applyconversationaction-operation"></a><span data-ttu-id="6608c-105">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="6608c-105">ApplyConversationAction operation</span></span>

<span data-ttu-id="6608c-106">Операция **ApplyConversationAction** задает одноразовый или исполнению действие для всех элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="6608c-106">The **ApplyConversationAction** operation sets a one-time or follow up action on all the items in a conversation.</span></span> <span data-ttu-id="6608c-107">Операция **ApplyConversationAction** позволяет распределить по категориям, перемещение, копирование, удаление и устанавливать состояние чтения всех элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="6608c-107">The **ApplyConversationAction** operation allows you to categorize, move, copy, delete, and set the read state on all items in a conversation.</span></span> <span data-ttu-id="6608c-108">Действия можно также задать для новых сообщений в беседе.</span><span class="sxs-lookup"><span data-stu-id="6608c-108">Actions can also be set for new messages in a conversation.</span></span> 
  
## <a name="applyconversationaction-request-example"></a><span data-ttu-id="6608c-109">Пример запроса ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="6608c-109">ApplyConversationAction request example</span></span>

### <a name="description"></a><span data-ttu-id="6608c-110">Описание</span><span class="sxs-lookup"><span data-stu-id="6608c-110">Description</span></span>

<span data-ttu-id="6608c-111">В следующем примере запрос **ApplyConversationAction** показано, как перемещать элементы в указанной беседе в другую папку.</span><span class="sxs-lookup"><span data-stu-id="6608c-111">The following example of an **ApplyConversationAction** request shows how to move the items in the specified conversation to another folder.</span></span> <span data-ttu-id="6608c-112">Также элементы, добавляемые к беседе будут перемещены в указанную папку.</span><span class="sxs-lookup"><span data-stu-id="6608c-112">Items that are added to the conversation will also be moved to the specified folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6608c-113">Программа</span><span class="sxs-lookup"><span data-stu-id="6608c-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="AAQkADVkNjM1EH39AWcDUGrnrnJ32hHpdc="/>
          <t:DestinationFolderId>
            <t:FolderId Id="AAMkADVkNjM1ODI3LTEwYTAtNDUBTTT6tWal35iSoKAAAABZZWAAA="/>
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

### <a name="remarks"></a><span data-ttu-id="6608c-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="6608c-114">Remarks</span></span>

<span data-ttu-id="6608c-115">Идентификаторы беседы и папки URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="6608c-115">The conversation and folder identifiers have been shortened to preserve readability.</span></span>
  
## <a name="applyconversationaction-response-example"></a><span data-ttu-id="6608c-116">Пример ответа ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="6608c-116">ApplyConversationAction response example</span></span>

### <a name="description"></a><span data-ttu-id="6608c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="6608c-117">Description</span></span>

<span data-ttu-id="6608c-118">В следующем примере показано успешного ответа на запрос **ApplyConversationAction** .</span><span class="sxs-lookup"><span data-stu-id="6608c-118">The following example shows a successful response to an **ApplyConversationAction** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6608c-119">Программа</span><span class="sxs-lookup"><span data-stu-id="6608c-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="91" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ApplyConversationActionResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ApplyConversationActionResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:ApplyConversationActionResponseMessage>
      </m:ResponseMessages>
    </m:ApplyConversationActionResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="6608c-120">См. также</span><span class="sxs-lookup"><span data-stu-id="6608c-120">See also</span></span>

- [<span data-ttu-id="6608c-121">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="6608c-121">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="6608c-122">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="6608c-122">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="6608c-123">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6608c-123">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="6608c-124">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="6608c-124">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

