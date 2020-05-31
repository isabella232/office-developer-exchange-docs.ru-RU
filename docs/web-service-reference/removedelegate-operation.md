---
title: Операция RemoveDelegate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RemoveDelegate
api_type:
- schema
ms.assetid: 1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a
description: Операция RemoveDelegate удаляет одного или нескольких делегатов из почтового ящика пользователя.
ms.openlocfilehash: 6f3371d19bd8a7fd967d4959d85037ae6b51f6aa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835088"
---
# <a name="removedelegate-operation"></a><span data-ttu-id="2fe7c-103">Операция RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="2fe7c-103">RemoveDelegate operation</span></span>

<span data-ttu-id="2fe7c-104">Операция **RemoveDelegate** удаляет одного или нескольких делегатов из почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-104">The **RemoveDelegate** operation removes one or more delegates from a user's mailbox.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="2fe7c-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="2fe7c-105">SOAP Headers</span></span>

<span data-ttu-id="2fe7c-106">Операция **RemoveDelegate** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-106">The **RemoveDelegate** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="2fe7c-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="2fe7c-107">**Header**</span></span>|<span data-ttu-id="2fe7c-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2fe7c-108">**Element**</span></span>|<span data-ttu-id="2fe7c-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2fe7c-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2fe7c-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="2fe7c-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="2fe7c-111">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="2fe7c-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2fe7c-112">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="2fe7c-113">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="2fe7c-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="2fe7c-114">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="2fe7c-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="2fe7c-115">Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="2fe7c-116">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="2fe7c-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="2fe7c-117">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="2fe7c-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2fe7c-118">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="2fe7c-119">серверверсион</span><span class="sxs-lookup"><span data-stu-id="2fe7c-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="2fe7c-120">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="2fe7c-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2fe7c-121">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="removedelegate-request-example"></a><span data-ttu-id="2fe7c-122">Пример запроса RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="2fe7c-122">RemoveDelegate request example</span></span>

### <a name="description"></a><span data-ttu-id="2fe7c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="2fe7c-123">Description</span></span>

<span data-ttu-id="2fe7c-124">В приведенном ниже примере кода показано, как удалить двух делегатов из почтового ящика user1's.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-124">The following code example shows how to remove two delegates from user1's mailbox.</span></span> <span data-ttu-id="2fe7c-125">В этом примере один делегат удаляется с помощью основного SMTP-адреса делегата, а другой удаляется с помощью идентификатора безопасности делегата (SID).</span><span class="sxs-lookup"><span data-stu-id="2fe7c-125">In this example, one delegate is removed by using the delegate's primary SMTP address, and the other one is removed by using the delegate's security identifier (SID).</span></span>
  
### <a name="code"></a><span data-ttu-id="2fe7c-126">Код</span><span class="sxs-lookup"><span data-stu-id="2fe7c-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1"/>
  </soap:Header>
  <soap:Body>
    <RemoveDelegate xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>user1@example.com</t:EmailAddress>
      </Mailbox>
      <UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>user2@example.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:SID>S-1-5-21-1333220396-2200287332-232816053-1118</t:SID>
        </t:UserId>
      </UserIds>
    </RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="2fe7c-127">Comments</span><span class="sxs-lookup"><span data-stu-id="2fe7c-127">Comments</span></span>

<span data-ttu-id="2fe7c-128">Операция **RemoveDelegate** не требует наличия почтового ящика или наличия почтового ящика в службе каталогов Active Directory для указанного пользователя делегата.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-128">The **RemoveDelegate** operation does not require the specified delegate user to have a mailbox or to exist in the Active Directory directory service.</span></span> <span data-ttu-id="2fe7c-129">Если запись делегата потеряна, операция **RemoveDelegate** будет выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-129">The **RemoveDelegate** operation will succeed if the delegate entry is orphaned.</span></span> 
  
## <a name="removedelegate-response-example"></a><span data-ttu-id="2fe7c-130">Пример отклика RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="2fe7c-130">RemoveDelegate response example</span></span>

### <a name="description"></a><span data-ttu-id="2fe7c-131">Описание</span><span class="sxs-lookup"><span data-stu-id="2fe7c-131">Description</span></span>

<span data-ttu-id="2fe7c-132">В приведенном ниже примере ответа **RemoveDelegate** показан успешный ответ на запрос **RemoveDelegate** .</span><span class="sxs-lookup"><span data-stu-id="2fe7c-132">The following example of a **RemoveDelegate** response shows a successful response to a **RemoveDelegate** request.</span></span> <span data-ttu-id="2fe7c-133">Ответ содержит элемент **делегатеусерреспонсемессажетипе** для каждого делегата, который удаляется из почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-133">The response contains a **DelegateUserResponseMessageType** element for each delegate that is removed from the mailbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2fe7c-134">Код</span><span class="sxs-lookup"><span data-stu-id="2fe7c-134">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" 
                         MinorVersion="1" 
                         MajorBuildNumber="206" 
                         MinorBuildNumber="0" 
                         Version="Exchange2007_SP1" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              ResponseClass="Success" 
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
      </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="removedelegate-error-response-example"></a><span data-ttu-id="2fe7c-135">Пример ответа на сообщение об ошибке RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="2fe7c-135">RemoveDelegate Error response example</span></span>

### <a name="description"></a><span data-ttu-id="2fe7c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="2fe7c-136">Description</span></span>

<span data-ttu-id="2fe7c-137">В приведенном ниже примере ответа на ошибку **RemoveDelegate** показаны результаты запроса на удаление делегата, который не существует.</span><span class="sxs-lookup"><span data-stu-id="2fe7c-137">The following example of a **RemoveDelegate** error response shows the results of a request to remove a delegate that does not exist.</span></span> 
  
### <a name="code"></a><span data-ttu-id="2fe7c-138">Код</span><span class="sxs-lookup"><span data-stu-id="2fe7c-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8"
                         MinorVersion="1"
                         MajorBuildNumber="206"
                         MinorBuildNumber="0"
                         Version="Exchange2007_SP1"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <m:RemoveDelegateResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                              ResponseClass="Success"
                              xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Error">
          <m:MessageText>The user is not a delegate for the mailbox.</m:MessageText>
          <m:ResponseCode>ErrorNotDelegate</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:RemoveDelegateResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="2fe7c-139">См. также</span><span class="sxs-lookup"><span data-stu-id="2fe7c-139">See also</span></span>



- [<span data-ttu-id="2fe7c-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2fe7c-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

