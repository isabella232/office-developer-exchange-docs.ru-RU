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
ms.openlocfilehash: 45a3e12756f3cbf29b76b442f7103abc5fb9a833
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461928"
---
# <a name="freebusyresponse"></a><span data-ttu-id="89b46-103">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="89b46-103">FreeBusyResponse</span></span>

<span data-ttu-id="89b46-104">Элемент **фрибусиреспонсе** содержит сведения о доступности для одного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="89b46-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="89b46-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="89b46-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="89b46-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="89b46-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="89b46-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="89b46-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="89b46-108">**фрибусиреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="89b46-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89b46-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="89b46-109">Attributes and elements</span></span>

<span data-ttu-id="89b46-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="89b46-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89b46-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="89b46-111">Attributes</span></span>

<span data-ttu-id="89b46-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="89b46-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89b46-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="89b46-113">Child elements</span></span>

|<span data-ttu-id="89b46-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89b46-114">**Element**</span></span>|<span data-ttu-id="89b46-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89b46-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89b46-116">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="89b46-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="89b46-117">Предоставляет описательные сведения о состоянии отклика.</span><span class="sxs-lookup"><span data-stu-id="89b46-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="89b46-118">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="89b46-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="89b46-119">Содержит сведения о доступности для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="89b46-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="89b46-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="89b46-120">Parent elements</span></span>

|<span data-ttu-id="89b46-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89b46-121">**Element**</span></span>|<span data-ttu-id="89b46-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89b46-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89b46-123">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="89b46-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="89b46-124">Содержит сведения о доступности запрошенных пользователей и состояние отклика.</span><span class="sxs-lookup"><span data-stu-id="89b46-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="89b46-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="89b46-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="89b46-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="89b46-126">Remarks</span></span>

<span data-ttu-id="89b46-127">Этот элемент не включается в ответ GetUserAvailability, если не запрашиваются сведения о занятости.</span><span class="sxs-lookup"><span data-stu-id="89b46-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="89b46-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="89b46-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89b46-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="89b46-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89b46-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="89b46-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="89b46-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="89b46-131">Schema Name</span></span>  <br/> |<span data-ttu-id="89b46-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="89b46-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="89b46-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="89b46-133">Validation File</span></span>  <br/> |<span data-ttu-id="89b46-134">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="89b46-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="89b46-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="89b46-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="89b46-136">False</span><span class="sxs-lookup"><span data-stu-id="89b46-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89b46-137">См. также</span><span class="sxs-lookup"><span data-stu-id="89b46-137">See also</span></span>



[<span data-ttu-id="89b46-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="89b46-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="89b46-139">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="89b46-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="89b46-140">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="89b46-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

