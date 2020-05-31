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
ms.openlocfilehash: 52731ea66420c21cf3fb8d19082aef65551c2af2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762744"
---
# <a name="getdelegateresponse"></a><span data-ttu-id="08ddd-103">жетделегатереспонсе</span><span class="sxs-lookup"><span data-stu-id="08ddd-103">GetDelegateResponse</span></span>

<span data-ttu-id="08ddd-104">Элемент **жетделегатереспонсе** содержит состояние и результат запроса [операции Delegate](getdelegate-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="08ddd-104">The **GetDelegateResponse** element contains the status and result of a [GetDelegate operation](getdelegate-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="08ddd-105">**жетделегатереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="08ddd-105">**GetDelegateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08ddd-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="08ddd-106">Attributes and elements</span></span>

<span data-ttu-id="08ddd-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="08ddd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08ddd-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="08ddd-108">Attributes</span></span>

<span data-ttu-id="08ddd-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="08ddd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08ddd-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="08ddd-110">Child elements</span></span>

|<span data-ttu-id="08ddd-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08ddd-111">**Element**</span></span>|<span data-ttu-id="08ddd-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08ddd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08ddd-113">деливермитингрекуестс</span><span class="sxs-lookup"><span data-stu-id="08ddd-113">DeliverMeetingRequests</span></span>](delivermeetingrequests.md) <br/> |<span data-ttu-id="08ddd-114">Определяет способ обработки приглашений на собрание между представителем и участником.</span><span class="sxs-lookup"><span data-stu-id="08ddd-114">Defines how meeting requests are handled between the delegate and the principal.</span></span>  <br/> |
|[<span data-ttu-id="08ddd-115">Респонсемессажес (Аррайофделегатеусерреспонсемессажетипе)</span><span class="sxs-lookup"><span data-stu-id="08ddd-115">ResponseMessages (ArrayOfDelegateUserResponseMessageType)</span></span>](responsemessages-arrayofdelegateuserresponsemessagetype.md) <br/> |<span data-ttu-id="08ddd-116">Содержит ответные сообщения для запроса управления делегированием веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="08ddd-116">Contains the response messages for an Exchange Web Services delegate management request.</span></span>  <br/> |
|[<span data-ttu-id="08ddd-117">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="08ddd-117">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="08ddd-118">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="08ddd-118">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="08ddd-119">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="08ddd-119">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="08ddd-120">Предоставляет код ошибки, определяющий конкретную ошибку, обнаруженную в запросе.</span><span class="sxs-lookup"><span data-stu-id="08ddd-120">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="08ddd-121">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="08ddd-121">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="08ddd-122">В настоящее время не используется и зарезервировано для последующего использования.</span><span class="sxs-lookup"><span data-stu-id="08ddd-122">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="08ddd-123">Он содержит значение 0.</span><span class="sxs-lookup"><span data-stu-id="08ddd-123">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="08ddd-124">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="08ddd-124">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="08ddd-125">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="08ddd-125">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08ddd-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="08ddd-126">Parent elements</span></span>

<span data-ttu-id="08ddd-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="08ddd-127">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08ddd-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="08ddd-128">Remarks</span></span>

<span data-ttu-id="08ddd-129">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="08ddd-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08ddd-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="08ddd-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08ddd-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="08ddd-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="08ddd-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="08ddd-132">Schema Name</span></span>  <br/> |<span data-ttu-id="08ddd-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="08ddd-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="08ddd-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="08ddd-134">Validation File</span></span>  <br/> |<span data-ttu-id="08ddd-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="08ddd-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="08ddd-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="08ddd-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="08ddd-137">False</span><span class="sxs-lookup"><span data-stu-id="08ddd-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08ddd-138">См. также</span><span class="sxs-lookup"><span data-stu-id="08ddd-138">See also</span></span>



[<span data-ttu-id="08ddd-139">Операция GetDelegate</span><span class="sxs-lookup"><span data-stu-id="08ddd-139">GetDelegate operation</span></span>](getdelegate-operation.md)


- [<span data-ttu-id="08ddd-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="08ddd-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

