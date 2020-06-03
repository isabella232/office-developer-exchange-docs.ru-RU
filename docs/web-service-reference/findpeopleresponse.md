---
title: финдпеоплереспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 95f016a9-002f-4be3-abd6-f5e3528afd44
description: Элемент Финдпеоплереспонсе указывает ответ на запрос FindPeople.
ms.openlocfilehash: b969ac3f7bc2bbd3fc77bf753a15696c3b6d8216
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466404"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="964e4-103">финдпеоплереспонсе</span><span class="sxs-lookup"><span data-stu-id="964e4-103">FindPeopleResponse</span></span>

<span data-ttu-id="964e4-104">Элемент **финдпеоплереспонсе** указывает ответ на запрос **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="964e4-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
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

 <span data-ttu-id="964e4-105">**финдпеоплереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="964e4-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="964e4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="964e4-106">Attributes and elements</span></span>

<span data-ttu-id="964e4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="964e4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="964e4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="964e4-108">Attributes</span></span>

|<span data-ttu-id="964e4-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="964e4-109">**Attribute**</span></span>|<span data-ttu-id="964e4-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="964e4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="964e4-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="964e4-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="964e4-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="964e4-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="964e4-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="964e4-113">ResponseClass</span></span>

|<span data-ttu-id="964e4-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="964e4-114">**Value**</span></span>|<span data-ttu-id="964e4-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="964e4-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="964e4-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="964e4-116">Success</span></span>  <br/> |<span data-ttu-id="964e4-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="964e4-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="964e4-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="964e4-118">Warning</span></span>  <br/> |<span data-ttu-id="964e4-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="964e4-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="964e4-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="964e4-120">Error</span></span>  <br/> |<span data-ttu-id="964e4-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="964e4-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="964e4-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="964e4-122">Child elements</span></span>

|<span data-ttu-id="964e4-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="964e4-123">**Element**</span></span>|<span data-ttu-id="964e4-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="964e4-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="964e4-125">Люди</span><span class="sxs-lookup"><span data-stu-id="964e4-125">People</span></span>](people.md) <br/> |<span data-ttu-id="964e4-126">Указывает массив данных о пользователях, возвращаемых в результате запроса **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="964e4-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="964e4-127">тоталнумберофпеоплеинвиев</span><span class="sxs-lookup"><span data-stu-id="964e4-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="964e4-128">Указывает общее количество пользователей, хранящихся на сервере, которые возвращаются запросом **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="964e4-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="964e4-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="964e4-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="964e4-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="964e4-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="964e4-131">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="964e4-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="964e4-132">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="964e4-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="964e4-133">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="964e4-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="964e4-134">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="964e4-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="964e4-135">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="964e4-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="964e4-136">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="964e4-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="964e4-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="964e4-137">Parent elements</span></span>

|<span data-ttu-id="964e4-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="964e4-138">**Element**</span></span>|<span data-ttu-id="964e4-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="964e4-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="964e4-140">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="964e4-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="964e4-141">Указывает массив ответных сообщений.</span><span class="sxs-lookup"><span data-stu-id="964e4-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="964e4-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="964e4-142">Remarks</span></span>

<span data-ttu-id="964e4-143">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="964e4-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="964e4-144">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="964e4-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="964e4-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="964e4-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="964e4-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="964e4-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="964e4-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="964e4-147">Schema Name</span></span>  <br/> |<span data-ttu-id="964e4-148">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="964e4-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="964e4-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="964e4-149">Validation File</span></span>  <br/> |<span data-ttu-id="964e4-150">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="964e4-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="964e4-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="964e4-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="964e4-152">См. также</span><span class="sxs-lookup"><span data-stu-id="964e4-152">See also</span></span>



- [<span data-ttu-id="964e4-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="964e4-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

