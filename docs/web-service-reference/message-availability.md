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
description: Элемент Message содержит ответ "нет на месте" (отсутствие на работе).
ms.openlocfilehash: 13d118422ccb5a2897c21b6d124f170bf461dbf6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467006"
---
# <a name="message-availability"></a><span data-ttu-id="9d9bb-103">Сообщение (доступность)</span><span class="sxs-lookup"><span data-stu-id="9d9bb-103">Message (Availability)</span></span>

<span data-ttu-id="9d9bb-104">Элемент **Message** содержит ответ "нет на месте" (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="9d9bb-104">The **Message** element contains the out of Office (OOF) response.</span></span> 
  
```xml
<Message/> 
```

 <span data-ttu-id="9d9bb-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="9d9bb-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d9bb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9d9bb-106">Attributes and elements</span></span>

<span data-ttu-id="9d9bb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d9bb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9d9bb-108">Attributes</span></span>

<span data-ttu-id="9d9bb-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d9bb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9d9bb-110">Child elements</span></span>

<span data-ttu-id="9d9bb-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d9bb-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9d9bb-112">Parent elements</span></span>

|<span data-ttu-id="9d9bb-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9d9bb-113">**Element**</span></span>|<span data-ttu-id="9d9bb-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9d9bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d9bb-115">интерналрепли</span><span class="sxs-lookup"><span data-stu-id="9d9bb-115">InternalReply</span></span>](internalreply.md) <br/> | <span data-ttu-id="9d9bb-116">Содержит сообщение об отсутствии на работе, отправленное другим пользователям в домене отправителя.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-116">Contains the OOF message sent to other users in the sender's domain.</span></span> <br/> <br/>  <span data-ttu-id="9d9bb-117">Ниже приведены возможные выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-117">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/InternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/InternalReply` <br/> |
|[<span data-ttu-id="9d9bb-118">екстерналрепли</span><span class="sxs-lookup"><span data-stu-id="9d9bb-118">ExternalReply</span></span>](externalreply.md) <br/> | <span data-ttu-id="9d9bb-119">Содержит сообщение об отсутствии на работе, которое отправляется адресам, не входящим в домен отправителя.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-119">Contains the OOF message that is sent to addresses outside the sender's domain.</span></span>  <br/> <br/> <span data-ttu-id="9d9bb-120">Ниже приведены возможные выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-120">The following are the possible XPath expressions to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/ExternalReply` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/ExternalReply` <br/> |
|[<span data-ttu-id="9d9bb-121">реплибоди</span><span class="sxs-lookup"><span data-stu-id="9d9bb-121">ReplyBody</span></span>](replybody.md) <br/> |<span data-ttu-id="9d9bb-122">Содержит сообщение об отсутствии на месте и язык, используемый для сообщения.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-122">Contains an OOF message and the language used for the message.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d9bb-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9d9bb-123">Text value</span></span>

<span data-ttu-id="9d9bb-124">Для установки сообщения об отсутствии на месте требуется текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-124">A text value is required to set the OOF message.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d9bb-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="9d9bb-125">Remarks</span></span>

<span data-ttu-id="9d9bb-126">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="9d9bb-127">Пример</span><span class="sxs-lookup"><span data-stu-id="9d9bb-127">Example</span></span>

<span data-ttu-id="9d9bb-128">В следующем примере запроса [операции SetUserOofSettings](setuseroofsettings-operation.md) задается для [уфстате](oofstate.md) значение **Enabled**, устанавливается время бездействия в 10 дней, а также задаются внутренние и внешние сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="9d9bb-128">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="9d9bb-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9d9bb-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d9bb-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9d9bb-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d9bb-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9d9bb-131">Schema Name</span></span>  <br/> |<span data-ttu-id="9d9bb-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9d9bb-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d9bb-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9d9bb-133">Validation File</span></span>  <br/> |<span data-ttu-id="9d9bb-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9d9bb-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d9bb-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9d9bb-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d9bb-136">False</span><span class="sxs-lookup"><span data-stu-id="9d9bb-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d9bb-137">См. также</span><span class="sxs-lookup"><span data-stu-id="9d9bb-137">See also</span></span>

- [<span data-ttu-id="9d9bb-138">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="9d9bb-138">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="9d9bb-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="9d9bb-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

