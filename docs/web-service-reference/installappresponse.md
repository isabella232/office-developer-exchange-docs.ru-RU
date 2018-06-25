---
title: InstallAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5e0582d-c1e1-453b-93ed-c31165c82697
description: Элемент InstallAppResponse указывает ответ на запрос InstallApp.
ms.openlocfilehash: 8e8da720b3a38e979b3d83810bb798350822146c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833942"
---
# <a name="installappresponse"></a><span data-ttu-id="406c0-103">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="406c0-103">InstallAppResponse</span></span>

<span data-ttu-id="406c0-104">Элемент **InstallAppResponse** указывает ответ на запрос **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="406c0-104">The **InstallAppResponse** element specifies the response to an **InstallApp** request.</span></span> 
  
```xml
<InstallAppResponse ResponseClass="">
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</InstallAppResponse>
```

 <span data-ttu-id="406c0-105">**InstallAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="406c0-105">**InstallAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="406c0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="406c0-106">Attributes and elements</span></span>

<span data-ttu-id="406c0-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="406c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="406c0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="406c0-108">Attributes</span></span>

|<span data-ttu-id="406c0-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="406c0-109">**Attribute**</span></span>|<span data-ttu-id="406c0-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="406c0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="406c0-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="406c0-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="406c0-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="406c0-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="406c0-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="406c0-113">ResponseClass</span></span>

|<span data-ttu-id="406c0-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="406c0-114">**Value**</span></span>|<span data-ttu-id="406c0-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="406c0-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="406c0-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="406c0-116">Success</span></span>  <br/> |<span data-ttu-id="406c0-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="406c0-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="406c0-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="406c0-118">Warning</span></span>  <br/> |<span data-ttu-id="406c0-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="406c0-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="406c0-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="406c0-120">Error</span></span>  <br/> |<span data-ttu-id="406c0-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="406c0-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="406c0-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="406c0-122">Child elements</span></span>

|<span data-ttu-id="406c0-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="406c0-123">**Element**</span></span>|<span data-ttu-id="406c0-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="406c0-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="406c0-125">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="406c0-125">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="406c0-126">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="406c0-126">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="406c0-127">MessageText</span><span class="sxs-lookup"><span data-stu-id="406c0-127">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="406c0-128">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="406c0-128">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="406c0-129">MessageXml</span><span class="sxs-lookup"><span data-stu-id="406c0-129">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="406c0-130">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="406c0-130">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="406c0-131">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="406c0-131">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="406c0-132">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="406c0-132">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="406c0-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="406c0-133">Parent elements</span></span>

|<span data-ttu-id="406c0-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="406c0-134">**Element**</span></span>|<span data-ttu-id="406c0-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="406c0-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="406c0-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="406c0-136">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="406c0-137">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="406c0-137">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="406c0-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="406c0-138">Text value</span></span>

<span data-ttu-id="406c0-139">Нет.</span><span class="sxs-lookup"><span data-stu-id="406c0-139">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="406c0-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="406c0-140">Remarks</span></span>

<span data-ttu-id="406c0-141">Элемент **GetAppManifestsResponseMessage** используется для клиентов, относящихся к Exchange Online и версий Microsoft Exchange Server, начиная с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="406c0-141">The **GetAppManifestsResponseMessage** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="406c0-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="406c0-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="406c0-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="406c0-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="406c0-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="406c0-144">Schema Name</span></span>  <br/> |<span data-ttu-id="406c0-145">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="406c0-145">Message schema</span></span>  <br/> |
|<span data-ttu-id="406c0-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="406c0-146">Validation File</span></span>  <br/> |<span data-ttu-id="406c0-147">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="406c0-147">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="406c0-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="406c0-148">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="406c0-149">См. также</span><span class="sxs-lookup"><span data-stu-id="406c0-149">See also</span></span>



- [<span data-ttu-id="406c0-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="406c0-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

