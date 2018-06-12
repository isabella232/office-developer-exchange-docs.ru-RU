---
title: Сообщение (доступность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Message
api_type:
- schema
ms.assetid: 1eec24dd-c981-41f4-a2f0-c51d43f1d7c0
description: Элемент сообщение содержит ожидания ответа Office (OOF).
ms.openlocfilehash: 9facd04767fdcc0fd9dfd84fc6badb1a7633d2b5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834452"
---
# <a name="message-availability"></a><span data-ttu-id="bc8ec-103">Сообщение (доступность)</span><span class="sxs-lookup"><span data-stu-id="bc8ec-103">Message (Availability)</span></span>

<span data-ttu-id="bc8ec-104">Элемент **сообщение** содержит ожидания ответа Office (OOF).</span><span class="sxs-lookup"><span data-stu-id="bc8ec-104">The **Message** element contains the out of Office (OOF) response.</span></span> 
  
```xml
<Message/> 
```

 <span data-ttu-id="bc8ec-105">**string**</span><span class="sxs-lookup"><span data-stu-id="bc8ec-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc8ec-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc8ec-106">Attributes and elements</span></span>

<span data-ttu-id="bc8ec-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc8ec-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc8ec-108">Attributes</span></span>

<span data-ttu-id="bc8ec-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc8ec-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc8ec-110">Child elements</span></span>

<span data-ttu-id="bc8ec-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc8ec-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc8ec-112">Parent elements</span></span>

|<span data-ttu-id="bc8ec-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc8ec-113">**Element**</span></span>|<span data-ttu-id="bc8ec-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc8ec-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc8ec-115">InternalReply</span><span class="sxs-lookup"><span data-stu-id="bc8ec-115">InternalReply</span></span>](internalreply.md) <br/> | <span data-ttu-id="bc8ec-116">Содержит сообщения об отсутствии на работе, для других пользователей в домен отправителя.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-116">Contains the OOF message sent to other users in the sender's domain.</span></span> <br/> <br/>  <span data-ttu-id="bc8ec-117">Ниже приведены возможные выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-117">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/InternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/InternalReply` <br/> |
|[<span data-ttu-id="bc8ec-118">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="bc8ec-118">ExternalReply</span></span>](externalreply.md) <br/> | <span data-ttu-id="bc8ec-119">Содержит сообщение об отсутствии на работе, которое отправляется адресам за пределами домена отправителя.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-119">Contains the OOF message that is sent to addresses outside the sender's domain.</span></span>  <br/> <br/> <span data-ttu-id="bc8ec-120">Ниже приведены возможные выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-120">The following are the possible XPath expressions to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/ExternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/ExternalReply` <br/> |
|[<span data-ttu-id="bc8ec-121">ReplyBody</span><span class="sxs-lookup"><span data-stu-id="bc8ec-121">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="bc8ec-122">Содержит сообщение об отсутствии на работе и язык, используемый для сообщения.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-122">Contains an OOF message and the language used for the message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bc8ec-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bc8ec-123">Text value</span></span>

<span data-ttu-id="bc8ec-124">Текстовое значение необходимо задать для сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-124">A text value is required to set the OOF message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bc8ec-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="bc8ec-125">Remarks</span></span>

<span data-ttu-id="bc8ec-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="bc8ec-127">Пример</span><span class="sxs-lookup"><span data-stu-id="bc8ec-127">Example</span></span>

<span data-ttu-id="bc8ec-128">В следующем примере [SetUserOofSettings операция](setuseroofsettings-operation.md) запроса задает [OofState](oofstate.md) **включена**, задает длительность об отсутствии на работе на 10 дней и задает внешних и внутренних сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="bc8ec-128">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="bc8ec-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc8ec-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc8ec-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc8ec-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc8ec-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc8ec-131">Schema Name</span></span>  <br/> |<span data-ttu-id="bc8ec-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bc8ec-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc8ec-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc8ec-133">Validation File</span></span>  <br/> |<span data-ttu-id="bc8ec-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bc8ec-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc8ec-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc8ec-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc8ec-136">False</span><span class="sxs-lookup"><span data-stu-id="bc8ec-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc8ec-137">См. также</span><span class="sxs-lookup"><span data-stu-id="bc8ec-137">See also</span></span>

- [<span data-ttu-id="bc8ec-138">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="bc8ec-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="bc8ec-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc8ec-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

