---
title: InternalReply
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- InternalReply
api_type:
- schema
ms.assetid: 1d784ded-b874-4eb1-8f6d-2e0e03330e1e
description: Элемент InternalReply содержит ожидания ответа сообщения об отсутствии для других пользователей в домене или доверенных доменов пользователя.
ms.openlocfilehash: ac5e9eadac7f45c233007ffb05f4d2430875ec52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833955"
---
# <a name="internalreply"></a><span data-ttu-id="55100-103">InternalReply</span><span class="sxs-lookup"><span data-stu-id="55100-103">InternalReply</span></span>

<span data-ttu-id="55100-104">Элемент **InternalReply** содержит ожидания ответа сообщения об отсутствии для других пользователей в домене или доверенных доменов пользователя.</span><span class="sxs-lookup"><span data-stu-id="55100-104">The **InternalReply** element contains the out of office (OOF) response sent to other users in the user's domain or trusted domains.</span></span> 
  
```XML
<InternalReply>
   <Message/> 
</InternalReply>
```

 <span data-ttu-id="55100-105">**ReplyBody**</span><span class="sxs-lookup"><span data-stu-id="55100-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55100-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="55100-106">Attributes and elements</span></span>

<span data-ttu-id="55100-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="55100-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55100-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="55100-108">Attributes</span></span>

|<span data-ttu-id="55100-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="55100-109">**Attribute**</span></span>|<span data-ttu-id="55100-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55100-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="55100-111">XML: lang</span><span class="sxs-lookup"><span data-stu-id="55100-111">xml:lang</span></span>  <br/> |<span data-ttu-id="55100-112">Указывает язык, используемый в сообщении **InternalReply** .</span><span class="sxs-lookup"><span data-stu-id="55100-112">Specifies the language used in the **InternalReply** message.</span></span> <span data-ttu-id="55100-113">Возможные значения этого атрибута определены в IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="55100-113">The possible values of this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="55100-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="55100-114">Child elements</span></span>

|<span data-ttu-id="55100-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55100-115">**Element**</span></span>|<span data-ttu-id="55100-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55100-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55100-117">Сообщение (доступность)</span><span class="sxs-lookup"><span data-stu-id="55100-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="55100-118">Содержит ответа об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="55100-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55100-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="55100-119">Parent elements</span></span>

|<span data-ttu-id="55100-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55100-120">**Element**</span></span>|<span data-ttu-id="55100-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55100-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55100-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="55100-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="55100-123">Задает параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="55100-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="55100-124">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="55100-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="55100-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="55100-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="55100-126">Содержит параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="55100-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="55100-127">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="55100-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55100-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="55100-128">Remarks</span></span>

<span data-ttu-id="55100-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="55100-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="55100-130">Пример</span><span class="sxs-lookup"><span data-stu-id="55100-130">Example</span></span>

<span data-ttu-id="55100-131">В следующем примере запроса SetUserOofSettings задает [OofState](oofstate.md) **включена**, задает длительность об отсутствии на работе для 10 дней и задает внешних и внутренних сообщений об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="55100-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF for 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="55100-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="55100-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55100-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="55100-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55100-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="55100-134">Schema Name</span></span>  <br/> |<span data-ttu-id="55100-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="55100-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="55100-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="55100-136">Validation File</span></span>  <br/> |<span data-ttu-id="55100-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55100-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55100-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="55100-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="55100-139">False</span><span class="sxs-lookup"><span data-stu-id="55100-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55100-140">См. также</span><span class="sxs-lookup"><span data-stu-id="55100-140">See also</span></span>



[<span data-ttu-id="55100-141">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="55100-141">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
  
[<span data-ttu-id="55100-142">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="55100-142">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

