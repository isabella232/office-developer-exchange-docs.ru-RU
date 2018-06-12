---
title: FindPeopleResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: Элемент FindPeopleResponse указывает ответ на запрос FindPeople.
ms.openlocfilehash: 4f2c2f6069a515d5153ea488b35182d8b35f029f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762591"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="7c4b7-103">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="7c4b7-103">FindPeopleResponse</span></span>

<span data-ttu-id="7c4b7-104">Элемент **FindPeopleResponse** указывает ответ на запрос **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="7c4b7-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
```XML
<FindPeopleResponse ResponseClass=" Success | Warning | Error ">
    <People/>
    <TotalNumberOfPeopleInView/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</FindPeopleResponse>
```

 <span data-ttu-id="7c4b7-105">**FindPeopleResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c4b7-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7c4b7-106">Attributes and elements</span></span>

<span data-ttu-id="7c4b7-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c4b7-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7c4b7-108">Attributes</span></span>

|<span data-ttu-id="7c4b7-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-109">**Attribute**</span></span>|<span data-ttu-id="7c4b7-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c4b7-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7c4b7-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="7c4b7-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="7c4b7-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="7c4b7-113">ResponseClass</span></span>

|<span data-ttu-id="7c4b7-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-114">**Value**</span></span>|<span data-ttu-id="7c4b7-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c4b7-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="7c4b7-116">Success</span></span>  <br/> |<span data-ttu-id="7c4b7-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="7c4b7-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="7c4b7-118">Warning</span></span>  <br/> |<span data-ttu-id="7c4b7-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="7c4b7-120">Error</span><span class="sxs-lookup"><span data-stu-id="7c4b7-120">Error</span></span>  <br/> |<span data-ttu-id="7c4b7-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7c4b7-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7c4b7-122">Child elements</span></span>

|<span data-ttu-id="7c4b7-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-123">**Element**</span></span>|<span data-ttu-id="7c4b7-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c4b7-125">Людей</span><span class="sxs-lookup"><span data-stu-id="7c4b7-125">People</span></span>](people.md) <br/> |<span data-ttu-id="7c4b7-126">Указывает массив данных пользователя, возвращаемых в результате запроса **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="7c4b7-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="7c4b7-127">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="7c4b7-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="7c4b7-128">Задает общее количество пользователей, хранящихся на сервере, возвращенных по запросу **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="7c4b7-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="7c4b7-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="7c4b7-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7c4b7-130">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7c4b7-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7c4b7-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7c4b7-132">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="7c4b7-133">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7c4b7-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7c4b7-134">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="7c4b7-135">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7c4b7-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7c4b7-136">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c4b7-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7c4b7-137">Parent elements</span></span>

|<span data-ttu-id="7c4b7-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-138">**Element**</span></span>|<span data-ttu-id="7c4b7-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c4b7-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c4b7-140">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7c4b7-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7c4b7-141">Указывает массив сообщения ответа.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c4b7-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="7c4b7-142">Remarks</span></span>

<span data-ttu-id="7c4b7-143">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7c4b7-144">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c4b7-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c4b7-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7c4b7-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c4b7-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7c4b7-146">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7c4b7-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7c4b7-147">Schema Name</span></span>  <br/> |<span data-ttu-id="7c4b7-148">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="7c4b7-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="7c4b7-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7c4b7-149">Validation File</span></span>  <br/> |<span data-ttu-id="7c4b7-150">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7c4b7-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7c4b7-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7c4b7-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7c4b7-152">См. также</span><span class="sxs-lookup"><span data-stu-id="7c4b7-152">See also</span></span>



- [<span data-ttu-id="7c4b7-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7c4b7-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

