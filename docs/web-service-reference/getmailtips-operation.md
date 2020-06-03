---
title: Операция GetMailTips
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetMailTips
api_type:
- schema
ms.assetid: 025483ec-a9f3-4735-8a95-d26e30ea7974
description: Операция с подсказками получает сведения о почтовых подсказках для указанного почтового ящика.
ms.openlocfilehash: 41a4bb99ee7ae4e416ec8a106968bb7869e60345
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458658"
---
# <a name="getmailtips-operation"></a><span data-ttu-id="36fac-103">Операция GetMailTips</span><span class="sxs-lookup"><span data-stu-id="36fac-103">GetMailTips operation</span></span>

<span data-ttu-id="36fac-104">Операция с подсказками получает сведения о **почтовых** подсказках для указанного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="36fac-104">The **GetMailTips** operation gets the mail tips information for the specified mailbox.</span></span> 
  
## <a name="getmailtips-request-example"></a><span data-ttu-id="36fac-105">Пример запроса на получение почтовых подсказок</span><span class="sxs-lookup"><span data-stu-id="36fac-105">GetMailTips request example</span></span>

### <a name="description"></a><span data-ttu-id="36fac-106">Description</span><span class="sxs-lookup"><span data-stu-id="36fac-106">Description</span></span>

<span data-ttu-id="36fac-107">Клиент создает XML-код запроса и отправляет его на сервер.</span><span class="sxs-lookup"><span data-stu-id="36fac-107">The client constructs the request XML and sends it to the server.</span></span> <span data-ttu-id="36fac-108">Запрос определяет клиента, который отправляется как, почтовый ящик для получения советов и советов по использованию электронной почты.</span><span class="sxs-lookup"><span data-stu-id="36fac-108">The request identifies who the client is sending as, the mailbox to retrieve the mail tips for, and what mail tips are requested.</span></span> <span data-ttu-id="36fac-109">В этом примере клиент запрашивает возвращение всех почтовых подсказок для выбранного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="36fac-109">In this example, the client requests that all mail tips be returned for the selected mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="36fac-110">Код</span><span class="sxs-lookup"><span data-stu-id="36fac-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
  <soap:Header> 
    <t:RequestServerVersion Version="Exchange2010" /> 
  </soap:Header> 
  <soap:Body> 
    <GetMailTips xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"> 
      <SendingAs> 
        <t:EmailAddress> user1@contoso.com </t:EmailAddress> 
        <t:RoutingType>SMTP</t:RoutingType> 
      </SendingAs> 
      <Recipients> 
        <t:Mailbox> 
          <t:EmailAddress> user2@contoso.com </t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
        </t:Mailbox> 
      </Recipients> 
      <MailTipsRequested>All</MailTipsRequested> 
    </GetMailTips> 
  </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="36fac-111">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="36fac-111">Request elements</span></span>

<span data-ttu-id="36fac-112">В запрос включены следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36fac-112">The following elements are included in the request:</span></span>
  
- [<span data-ttu-id="36fac-113">GetMailTips</span><span class="sxs-lookup"><span data-stu-id="36fac-113">GetMailTips</span></span>](getmailtips.md)
    
- [<span data-ttu-id="36fac-114">сендингас</span><span class="sxs-lookup"><span data-stu-id="36fac-114">SendingAs</span></span>](sendingas.md)
    
- [<span data-ttu-id="36fac-115">Получатели (АррайофреЦипиентстипе)</span><span class="sxs-lookup"><span data-stu-id="36fac-115">Recipients (ArrayOfRecipientsType)</span></span>](recipients-arrayofrecipientstype.md)
    
- [<span data-ttu-id="36fac-116">маилтипсрекуестед</span><span class="sxs-lookup"><span data-stu-id="36fac-116">MailTipsRequested</span></span>](mailtipsrequested.md)
    
## <a name="successful-getmailtips-response-example"></a><span data-ttu-id="36fac-117">Пример отклика успешных почтовых подсказок</span><span class="sxs-lookup"><span data-stu-id="36fac-117">Successful GetMailTips response example</span></span>

### <a name="description"></a><span data-ttu-id="36fac-118">Description</span><span class="sxs-lookup"><span data-stu-id="36fac-118">Description</span></span>

<span data-ttu-id="36fac-119">В приведенном ниже примере кода SOAP показан успешный ответ **на запрос по** подсказке.</span><span class="sxs-lookup"><span data-stu-id="36fac-119">The following Simple Object Access Protocol (SOAP) body example shows a successful response to the **GetMailTips** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="36fac-120">Код</span><span class="sxs-lookup"><span data-stu-id="36fac-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"> 
  <s:Header> 
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="0" MajorBuildNumber="536" MinorBuildNumber="0" Version="Exchange2010" 
xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
xmlns:xsd="http://www.w3.org/2001/XMLSchema"/> 
  </s:Header> 
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <GetMailTipsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"> 
      <ResponseCode>NoError</ResponseCode> 
      <ResponseMessages> 
        <MailTipsResponseMessageType ResponseClass="Success"> 
        <ResponseCode>NoError</ResponseCode> 
        <m:MailTips xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"> 20 / 29 [MS-OXWMT] — v20100517 Mail Tips Web Service Extensions Copyright © 2010 Microsoft Corporation. Release: Monday, May 17, 2010 
          <t:RecipientAddress xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
          <t:Name/> 
          <t:EmailAddress>user2@contoso.com</t:EmailAddress> 
          <t:RoutingType>SMTP</t:RoutingType> 
          </t:RecipientAddress> 
          <t:PendingMailTips xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/> 
          <t:OutOfOffice xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"> 
            <t:ReplyBody> 
              <t:Message/> 
            </t:ReplyBody> 
          </t:OutOfOffice> 
          <t:MailboxFull xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:MailboxFull> 
          <t:CustomMailTip xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">Hello World Mailtips</t:CustomMailTip> 
          <t:TotalMemberCount xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">1</t:TotalMemberCount> 
          <t:ExternalMemberCount xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">0</t:ExternalMemberCount> 
          <t:MaxMessageSize xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">10485760</t:MaxMessageSize> 
          <t:DeliveryRestricted xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:DeliveryRestricted> 
          <t:IsModerated xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:IsModerated> 
          <t:InvalidRecipient xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">false</t:InvalidRecipient> 
        </m:MailTips> 
        </MailTipsResponseMessageType> 
      </ResponseMessages> 
    </GetMailTipsResponse> 
  </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="36fac-121">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="36fac-121">Response elements</span></span>

<span data-ttu-id="36fac-122">В ответ включаются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="36fac-122">The following elements are included in the response:</span></span>
  
- [<span data-ttu-id="36fac-123">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="36fac-123">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="36fac-124">Подсказки</span><span class="sxs-lookup"><span data-stu-id="36fac-124">MailTips</span></span>](mailtips.md)
    
## <a name="see-also"></a><span data-ttu-id="36fac-125">См. также</span><span class="sxs-lookup"><span data-stu-id="36fac-125">See also</span></span>



[<span data-ttu-id="36fac-126">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="36fac-126">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="36fac-127">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="36fac-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

