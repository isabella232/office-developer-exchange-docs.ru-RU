---
title: жетделегатереспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetDelegateResponse
api_type:
- schema
ms.assetid: 71a418a5-5652-40e1-8f84-fe4f7c9f86af
description: Элемент Жетделегатереспонсе содержит состояние и результат запроса операции Delegate.
ms.openlocfilehash: 81c5033cd67b79baa131d71ea0b866c788ae5e82
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462026"
---
# <a name="getdelegateresponse"></a><span data-ttu-id="4f06a-103">жетделегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="4f06a-103">GetDelegateResponse</span></span>

<span data-ttu-id="4f06a-104">Элемент **жетделегатереспонсе** содержит состояние и результат запроса [операции Delegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="4f06a-104">The **GetDelegateResponse** element contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span> 
  
```xml
<GetDelegateResponse>
   <DeliverMeetingRequests/>
   <ResponseMessages/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</GetDelegateResponse>
```

 <span data-ttu-id="4f06a-105">**жетделегатереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="4f06a-105">**GetDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4f06a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4f06a-106">Attributes and elements</span></span>

<span data-ttu-id="4f06a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4f06a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4f06a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4f06a-108">Attributes</span></span>

<span data-ttu-id="4f06a-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4f06a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4f06a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4f06a-110">Child elements</span></span>

|<span data-ttu-id="4f06a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4f06a-111">**Element**</span></span>|<span data-ttu-id="4f06a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4f06a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4f06a-113">деливермитингрекуестс</span><span class="sxs-lookup"><span data-stu-id="4f06a-113">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="4f06a-114">Определяет способ обработки приглашений на собрание между представителем и участником.</span><span class="sxs-lookup"><span data-stu-id="4f06a-114">Defines how meeting requests are handled between the delegate and the principal.</span></span>  <br/> |
|[<span data-ttu-id="4f06a-115">Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="4f06a-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="4f06a-116">Содержит ответные сообщения для запроса управления делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4f06a-116">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="4f06a-117">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="4f06a-117">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4f06a-118">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="4f06a-118">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4f06a-119">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="4f06a-119">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4f06a-120">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="4f06a-120">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4f06a-121">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="4f06a-121">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4f06a-122">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="4f06a-122">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4f06a-123">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="4f06a-123">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4f06a-124">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="4f06a-124">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4f06a-125">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="4f06a-125">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4f06a-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4f06a-126">Parent elements</span></span>

<span data-ttu-id="4f06a-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="4f06a-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4f06a-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="4f06a-128">Remarks</span></span>

<span data-ttu-id="4f06a-129">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4f06a-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4f06a-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4f06a-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4f06a-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4f06a-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4f06a-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4f06a-132">Schema Name</span></span>  <br/> |<span data-ttu-id="4f06a-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4f06a-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4f06a-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4f06a-134">Validation File</span></span>  <br/> |<span data-ttu-id="4f06a-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4f06a-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4f06a-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4f06a-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="4f06a-137">False</span><span class="sxs-lookup"><span data-stu-id="4f06a-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4f06a-138">См. также</span><span class="sxs-lookup"><span data-stu-id="4f06a-138">See also</span></span>



[<span data-ttu-id="4f06a-139">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="4f06a-139">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="4f06a-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4f06a-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

