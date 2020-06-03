---
title: фрибусиреспонсеаррай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponseArray
api_type:
- schema
ms.assetid: 5592a37e-cf4b-4643-8a2a-fa58c40345b9
description: Элемент Фрибусиреспонсеаррай содержит сведения о доступности запрашиваемых пользователей и состояние отклика.
ms.openlocfilehash: b45938c19b76a377fca125fb6a19f9d712718db6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457811"
---
# <a name="freebusyresponsearray"></a><span data-ttu-id="b9017-103">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="b9017-103">FreeBusyResponseArray</span></span>

<span data-ttu-id="b9017-104">Элемент **фрибусиреспонсеаррай** содержит сведения о доступности запрашиваемых пользователей и состояние отклика.</span><span class="sxs-lookup"><span data-stu-id="b9017-104">The **FreeBusyResponseArray** element contains the requested users' availability information and the response status.</span></span> 
  
[<span data-ttu-id="b9017-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="b9017-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b9017-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="b9017-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
```xml
<FreeBusyResponseArray>
   <FreeBusyResponse>...</FreeBusyResponse>
</FreeBusyResponseArray>
```

 <span data-ttu-id="b9017-107">**аррайоффрибусиреспонсе**</span><span class="sxs-lookup"><span data-stu-id="b9017-107">**ArrayOfFreeBusyResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b9017-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b9017-108">Attributes and elements</span></span>

<span data-ttu-id="b9017-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b9017-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b9017-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b9017-110">Attributes</span></span>

<span data-ttu-id="b9017-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b9017-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b9017-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b9017-112">Child elements</span></span>

|<span data-ttu-id="b9017-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b9017-113">**Element**</span></span>|<span data-ttu-id="b9017-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b9017-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9017-115">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="b9017-115">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="b9017-116">Содержит сведения о доступности для одного пользователя почтового ящика и состояние отклика.</span><span class="sxs-lookup"><span data-stu-id="b9017-116">Contains the free/busy information for a single mailbox user and the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b9017-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b9017-117">Parent elements</span></span>

|<span data-ttu-id="b9017-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b9017-118">**Element**</span></span>|<span data-ttu-id="b9017-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b9017-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b9017-120">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="b9017-120">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="b9017-121">Содержит свойства, которые определяют сведения о доступности пользователей или сведения о предложенном времени собраний.</span><span class="sxs-lookup"><span data-stu-id="b9017-121">Contains the properties that define user availability information or suggested meeting time information.</span></span>  <br/> <span data-ttu-id="b9017-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="b9017-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b9017-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="b9017-123">Remarks</span></span>

<span data-ttu-id="b9017-124">Этот элемент не включается в ответ GetUserAvailability, если не запрашиваются сведения о занятости.</span><span class="sxs-lookup"><span data-stu-id="b9017-124">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="b9017-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b9017-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b9017-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b9017-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b9017-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b9017-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b9017-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b9017-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b9017-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b9017-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b9017-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b9017-130">Validation File</span></span>  <br/> |<span data-ttu-id="b9017-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b9017-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b9017-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b9017-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b9017-133">False</span><span class="sxs-lookup"><span data-stu-id="b9017-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9017-134">См. также</span><span class="sxs-lookup"><span data-stu-id="b9017-134">See also</span></span>



[<span data-ttu-id="b9017-135">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b9017-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b9017-136">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="b9017-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b9017-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="b9017-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

