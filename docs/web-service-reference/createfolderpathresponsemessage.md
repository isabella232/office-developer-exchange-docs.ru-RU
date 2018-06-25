---
title: CreateFolderPathResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7b3507-713d-4ccf-8518-75fa6f967d6d
description: Элемент CreateFolderPathResponseMessage указывает сообщение ответа на запрос CreateFolderPath.
ms.openlocfilehash: f8f85cc246bb5d5ecd5cb745267d9d373286cf7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761878"
---
# <a name="createfolderpathresponsemessage"></a><span data-ttu-id="db245-103">CreateFolderPathResponseMessage</span><span class="sxs-lookup"><span data-stu-id="db245-103">CreateFolderPathResponseMessage</span></span>

<span data-ttu-id="db245-104">Элемент **CreateFolderPathResponseMessage** указывает сообщение ответа на запрос **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="db245-104">The **CreateFolderPathResponseMessage** element specifies the response message for a **CreateFolderPath** request.</span></span> 
  
```XML
<CreateFolderPathResponseMessage ResponseClass="">
    <Folders></Folders>
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</CreateFolderPathResponseMessage>
```

 <span data-ttu-id="db245-105">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="db245-105">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db245-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="db245-106">Attributes and elements</span></span>

<span data-ttu-id="db245-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="db245-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db245-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="db245-108">Attributes</span></span>

|<span data-ttu-id="db245-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="db245-109">**Attribute**</span></span>|<span data-ttu-id="db245-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db245-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="db245-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="db245-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="db245-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="db245-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="db245-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="db245-113">ResponseClass</span></span>

|<span data-ttu-id="db245-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="db245-114">**Value**</span></span>|<span data-ttu-id="db245-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db245-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="db245-116">Успешное выполнение</span><span class="sxs-lookup"><span data-stu-id="db245-116">Success</span></span>  <br/> |<span data-ttu-id="db245-117">Означает успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="db245-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="db245-118">Предупреждающая</span><span class="sxs-lookup"><span data-stu-id="db245-118">Warning</span></span>  <br/> |<span data-ttu-id="db245-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="db245-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="db245-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="db245-120">Error</span></span>  <br/> |<span data-ttu-id="db245-121">Отображается сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="db245-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="db245-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="db245-122">Child elements</span></span>

|<span data-ttu-id="db245-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db245-123">**Element**</span></span>|<span data-ttu-id="db245-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db245-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db245-125">Папки</span><span class="sxs-lookup"><span data-stu-id="db245-125">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="db245-126">Содержит набор папок, используемых в операциях папки.</span><span class="sxs-lookup"><span data-stu-id="db245-126">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
|[<span data-ttu-id="db245-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="db245-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="db245-128">В настоящее время используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="db245-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="db245-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="db245-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="db245-130">Предоставляет текстовое описание состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="db245-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="db245-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="db245-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="db245-132">Предоставляет дополнительные сведения об ошибке ответа.</span><span class="sxs-lookup"><span data-stu-id="db245-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="db245-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="db245-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="db245-134">Предоставляет сведения о состоянии о запросе.</span><span class="sxs-lookup"><span data-stu-id="db245-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db245-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="db245-135">Parent elements</span></span>

|<span data-ttu-id="db245-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db245-136">**Element**</span></span>|<span data-ttu-id="db245-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db245-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db245-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="db245-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="db245-139">Содержит сообщения ответа на запрос веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="db245-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="db245-140">Замечания</span><span class="sxs-lookup"><span data-stu-id="db245-140">Remarks</span></span>

<span data-ttu-id="db245-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="db245-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="db245-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="db245-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db245-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="db245-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db245-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="db245-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="db245-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="db245-145">Schema Name</span></span>  <br/> |<span data-ttu-id="db245-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="db245-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="db245-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="db245-147">Validation File</span></span>  <br/> |<span data-ttu-id="db245-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="db245-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db245-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="db245-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="db245-150">См. также</span><span class="sxs-lookup"><span data-stu-id="db245-150">See also</span></span>

- [<span data-ttu-id="db245-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="db245-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

