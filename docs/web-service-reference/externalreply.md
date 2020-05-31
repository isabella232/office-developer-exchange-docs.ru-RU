---
title: екстерналрепли
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExternalReply
api_type:
- schema
ms.assetid: cbcfa469-242c-4f98-8f4f-2c9bcbe69f5a
description: Элемент Екстерналрепли содержит ответ "нет на месте" (отсутствие на месте), который отправляется на адреса вне домена получателя или доверенных доменов.
ms.openlocfilehash: f318b34c98dd42487b8ca3791ba915fb91d629a5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762513"
---
# <a name="externalreply"></a><span data-ttu-id="d9728-103">екстерналрепли</span><span class="sxs-lookup"><span data-stu-id="d9728-103">ExternalReply</span></span>

<span data-ttu-id="d9728-104">Элемент **екстерналрепли** содержит ответ "нет на месте" (отсутствие на месте), который отправляется на адреса вне домена получателя или доверенных доменов.</span><span class="sxs-lookup"><span data-stu-id="d9728-104">The **ExternalReply** element contains the out of office (OOF) response that is sent to addresses outside the recipient's domain or trusted domains.</span></span> 
  
```XML
<ExternalReply>
   <Message/>
</ExternalReply>
```

 <span data-ttu-id="d9728-105">**реплибоди**</span><span class="sxs-lookup"><span data-stu-id="d9728-105">**ReplyBody**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d9728-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d9728-106">Attributes and elements</span></span>

<span data-ttu-id="d9728-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d9728-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d9728-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d9728-108">Attributes</span></span>

|<span data-ttu-id="d9728-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d9728-109">**Attribute**</span></span>|<span data-ttu-id="d9728-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d9728-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d9728-111">XML: lang</span><span class="sxs-lookup"><span data-stu-id="d9728-111">xml:lang</span></span>  <br/> |<span data-ttu-id="d9728-112">Указывает язык, используемый в сообщении **екстерналрепли** .</span><span class="sxs-lookup"><span data-stu-id="d9728-112">Specifies the language used in the **ExternalReply** message.</span></span> <span data-ttu-id="d9728-113">Возможные значения для этого атрибута определены в документе IETF RFC 3066.</span><span class="sxs-lookup"><span data-stu-id="d9728-113">The possible values for this attribute are defined by IETF RFC 3066.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d9728-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d9728-114">Child elements</span></span>

|<span data-ttu-id="d9728-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d9728-115">**Element**</span></span>|<span data-ttu-id="d9728-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d9728-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9728-117">Сообщение (доступность)</span><span class="sxs-lookup"><span data-stu-id="d9728-117">Message (Availability)</span></span>](message-availability.md) <br/> |<span data-ttu-id="d9728-118">Содержит отклик на отсутствие на работе.</span><span class="sxs-lookup"><span data-stu-id="d9728-118">Contains the OOF response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d9728-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d9728-119">Parent elements</span></span>

|<span data-ttu-id="d9728-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d9728-120">**Element**</span></span>|<span data-ttu-id="d9728-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d9728-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d9728-122">усеруфсеттингс</span><span class="sxs-lookup"><span data-stu-id="d9728-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="d9728-123">Задает параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="d9728-123">Specifies the OOF settings.</span></span>  <br/> <span data-ttu-id="d9728-124">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d9728-124">The following is the XPath expression to this element:</span></span>  <br/>  `/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="d9728-125">уфсеттингс</span><span class="sxs-lookup"><span data-stu-id="d9728-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="d9728-126">Содержит параметры отсутствия на работе.</span><span class="sxs-lookup"><span data-stu-id="d9728-126">Contains the OOF settings.</span></span>  <br/> <span data-ttu-id="d9728-127">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d9728-127">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserOofSettingsResponse/OofSettings` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d9728-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="d9728-128">Remarks</span></span>

<span data-ttu-id="d9728-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="d9728-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="d9728-130">Пример</span><span class="sxs-lookup"><span data-stu-id="d9728-130">Example</span></span>

<span data-ttu-id="d9728-131">В следующем примере запроса SetUserOofSettings задается для [уфстате](oofstate.md) значение **Enabled**, устанавливается время бездействия в 10 дней, а также задаются внутренние и внешние сообщения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="d9728-131">The following example of a SetUserOofSettings request sets the [OofState](oofstate.md) to **Enabled**, sets the duration of OOF to 10 days, and sets the internal and external OOF messages.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="d9728-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d9728-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d9728-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d9728-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d9728-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d9728-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d9728-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d9728-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="d9728-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d9728-136">Validation File</span></span>  <br/> |<span data-ttu-id="d9728-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d9728-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d9728-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d9728-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d9728-139">False</span><span class="sxs-lookup"><span data-stu-id="d9728-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d9728-140">См. также</span><span class="sxs-lookup"><span data-stu-id="d9728-140">See also</span></span>



[<span data-ttu-id="d9728-141">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="d9728-141">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

