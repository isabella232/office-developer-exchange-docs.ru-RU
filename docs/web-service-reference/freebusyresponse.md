---
title: фрибусиреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponse
api_type:
- schema
ms.assetid: 3038d106-9ac9-4ac7-bb43-96c783edbef5
description: Элемент Фрибусиреспонсе содержит сведения о доступности для одного пользователя почтового ящика.
ms.openlocfilehash: 73e3972bb53d6bf59e5156098bad06bcde5f0155
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762655"
---
# <a name="freebusyresponse"></a><span data-ttu-id="63ddd-103">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="63ddd-103">FreeBusyResponse</span></span>

<span data-ttu-id="63ddd-104">Элемент **фрибусиреспонсе** содержит сведения о доступности для одного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="63ddd-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="63ddd-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="63ddd-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="63ddd-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="63ddd-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="63ddd-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="63ddd-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="63ddd-108">**фрибусиреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="63ddd-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63ddd-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="63ddd-109">Attributes and elements</span></span>

<span data-ttu-id="63ddd-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="63ddd-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63ddd-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="63ddd-111">Attributes</span></span>

<span data-ttu-id="63ddd-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="63ddd-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63ddd-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="63ddd-113">Child elements</span></span>

|<span data-ttu-id="63ddd-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="63ddd-114">**Element**</span></span>|<span data-ttu-id="63ddd-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="63ddd-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63ddd-116">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="63ddd-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="63ddd-117">Предоставляет описательные сведения о состоянии отклика.</span><span class="sxs-lookup"><span data-stu-id="63ddd-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="63ddd-118">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="63ddd-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="63ddd-119">Содержит сведения о доступности для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="63ddd-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63ddd-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="63ddd-120">Parent elements</span></span>

|<span data-ttu-id="63ddd-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="63ddd-121">**Element**</span></span>|<span data-ttu-id="63ddd-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="63ddd-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63ddd-123">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="63ddd-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="63ddd-124">Содержит сведения о доступности запрошенных пользователей и состояние отклика.</span><span class="sxs-lookup"><span data-stu-id="63ddd-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="63ddd-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="63ddd-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="63ddd-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="63ddd-126">Remarks</span></span>

<span data-ttu-id="63ddd-127">Этот элемент не включается в ответ GetUserAvailability, если не запрашиваются сведения о занятости.</span><span class="sxs-lookup"><span data-stu-id="63ddd-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="63ddd-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="63ddd-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63ddd-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="63ddd-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63ddd-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="63ddd-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="63ddd-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="63ddd-131">Schema Name</span></span>  <br/> |<span data-ttu-id="63ddd-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="63ddd-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="63ddd-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="63ddd-133">Validation File</span></span>  <br/> |<span data-ttu-id="63ddd-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="63ddd-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63ddd-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="63ddd-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="63ddd-136">False</span><span class="sxs-lookup"><span data-stu-id="63ddd-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63ddd-137">См. также</span><span class="sxs-lookup"><span data-stu-id="63ddd-137">See also</span></span>



[<span data-ttu-id="63ddd-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="63ddd-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="63ddd-139">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="63ddd-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="63ddd-140">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="63ddd-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

