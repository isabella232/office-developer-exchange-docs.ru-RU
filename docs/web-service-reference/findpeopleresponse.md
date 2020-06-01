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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466404"
---
# <a name="findpeopleresponse"></a><span data-ttu-id="b4a4d-103">финдпеоплереспонсе</span><span class="sxs-lookup"><span data-stu-id="b4a4d-103">FindPeopleResponse</span></span>

<span data-ttu-id="b4a4d-104">Элемент **финдпеоплереспонсе** указывает ответ на запрос **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="b4a4d-104">The **FindPeopleResponse** element specifies the response to a **FindPeople** request.</span></span> 
  
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

 <span data-ttu-id="b4a4d-105">**финдпеоплереспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-105">**FindPeopleResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4a4d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b4a4d-106">Attributes and elements</span></span>

<span data-ttu-id="b4a4d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4a4d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4a4d-108">Attributes</span></span>

|<span data-ttu-id="b4a4d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-109">**Attribute**</span></span>|<span data-ttu-id="b4a4d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b4a4d-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="b4a4d-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="b4a4d-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-112">Specifies the response class.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="b4a4d-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="b4a4d-113">ResponseClass</span></span>

|<span data-ttu-id="b4a4d-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-114">**Value**</span></span>|<span data-ttu-id="b4a4d-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b4a4d-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="b4a4d-116">Success</span></span>  <br/> |<span data-ttu-id="b4a4d-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="b4a4d-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="b4a4d-118">Warning</span></span>  <br/> |<span data-ttu-id="b4a4d-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="b4a4d-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="b4a4d-120">Error</span></span>  <br/> |<span data-ttu-id="b4a4d-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b4a4d-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b4a4d-122">Child elements</span></span>

|<span data-ttu-id="b4a4d-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-123">**Element**</span></span>|<span data-ttu-id="b4a4d-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4a4d-125">Люди</span><span class="sxs-lookup"><span data-stu-id="b4a4d-125">People</span></span>](people.md) <br/> |<span data-ttu-id="b4a4d-126">Указывает массив данных о пользователях, возвращаемых в результате запроса **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="b4a4d-126">Specifies an array of persona data returned as the result of a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="b4a4d-127">тоталнумберофпеоплеинвиев</span><span class="sxs-lookup"><span data-stu-id="b4a4d-127">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md) <br/> |<span data-ttu-id="b4a4d-128">Указывает общее количество пользователей, хранящихся на сервере, которые возвращаются запросом **FindPeople** .</span><span class="sxs-lookup"><span data-stu-id="b4a4d-128">Specifies the total number of personas stored on a server that are returned by a **FindPeople** request.</span></span>  <br/> |
|[<span data-ttu-id="b4a4d-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="b4a4d-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b4a4d-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b4a4d-131">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="b4a4d-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b4a4d-132">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-132">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="b4a4d-133">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="b4a4d-133">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b4a4d-134">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-134">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="b4a4d-135">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="b4a4d-135">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b4a4d-136">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-136">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4a4d-137">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b4a4d-137">Parent elements</span></span>

|<span data-ttu-id="b4a4d-138">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-138">**Element**</span></span>|<span data-ttu-id="b4a4d-139">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b4a4d-139">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4a4d-140">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="b4a4d-140">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b4a4d-141">Указывает массив ответных сообщений.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-141">Specifies an array of response messages.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b4a4d-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="b4a4d-142">Remarks</span></span>

<span data-ttu-id="b4a4d-143">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-143">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b4a4d-144">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b4a4d-144">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b4a4d-145">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b4a4d-145">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4a4d-146">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b4a4d-146">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b4a4d-147">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b4a4d-147">Schema Name</span></span>  <br/> |<span data-ttu-id="b4a4d-148">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="b4a4d-148">Message schema</span></span>  <br/> |
|<span data-ttu-id="b4a4d-149">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b4a4d-149">Validation File</span></span>  <br/> |<span data-ttu-id="b4a4d-150">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b4a4d-150">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b4a4d-151">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b4a4d-151">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b4a4d-152">См. также</span><span class="sxs-lookup"><span data-stu-id="b4a4d-152">See also</span></span>



- [<span data-ttu-id="b4a4d-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b4a4d-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

