---
title: креатефолдерпасреспонсемессаже
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f7b3507-713d-4ccf-8518-75fa6f967d6d
description: Элемент Креатефолдерпасреспонсемессаже указывает ответное сообщение для запроса CreateFolderPath.
ms.openlocfilehash: f8f85cc246bb5d5ecd5cb745267d9d373286cf7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761878"
---
# <a name="createfolderpathresponsemessage"></a><span data-ttu-id="30b82-103">креатефолдерпасреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="30b82-103">CreateFolderPathResponseMessage</span></span>

<span data-ttu-id="30b82-104">Элемент **креатефолдерпасреспонсемессаже** указывает ответное сообщение для запроса **CreateFolderPath** .</span><span class="sxs-lookup"><span data-stu-id="30b82-104">The **CreateFolderPathResponseMessage** element specifies the response message for a **CreateFolderPath** request.</span></span> 
  
```XML
<CreateFolderPathResponseMessage ResponseClass="">
    <Folders></Folders>
    <MessageText></MessageText>
    <ResponseCode></ResponseCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</CreateFolderPathResponseMessage>
```

 <span data-ttu-id="30b82-105">**фолдеринфореспонсемессажетипе**</span><span class="sxs-lookup"><span data-stu-id="30b82-105">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30b82-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="30b82-106">Attributes and elements</span></span>

<span data-ttu-id="30b82-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="30b82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30b82-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="30b82-108">Attributes</span></span>

|<span data-ttu-id="30b82-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="30b82-109">**Attribute**</span></span>|<span data-ttu-id="30b82-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30b82-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30b82-111">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="30b82-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="30b82-112">Указывает класс ответа.</span><span class="sxs-lookup"><span data-stu-id="30b82-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="30b82-113">респонсекласс</span><span class="sxs-lookup"><span data-stu-id="30b82-113">ResponseClass</span></span>

|<span data-ttu-id="30b82-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="30b82-114">**Value**</span></span>|<span data-ttu-id="30b82-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30b82-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30b82-116">Успешно</span><span class="sxs-lookup"><span data-stu-id="30b82-116">Success</span></span>  <br/> |<span data-ttu-id="30b82-117">Указывает на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="30b82-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="30b82-118">Предупреждение</span><span class="sxs-lookup"><span data-stu-id="30b82-118">Warning</span></span>  <br/> |<span data-ttu-id="30b82-119">Указывает на предупреждение.</span><span class="sxs-lookup"><span data-stu-id="30b82-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="30b82-120">Ошибка</span><span class="sxs-lookup"><span data-stu-id="30b82-120">Error</span></span>  <br/> |<span data-ttu-id="30b82-121">Указывает на ошибку.</span><span class="sxs-lookup"><span data-stu-id="30b82-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="30b82-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="30b82-122">Child elements</span></span>

|<span data-ttu-id="30b82-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="30b82-123">**Element**</span></span>|<span data-ttu-id="30b82-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30b82-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30b82-125">Folders</span><span class="sxs-lookup"><span data-stu-id="30b82-125">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="30b82-126">Содержит массив папок, используемых в операциях с папками.</span><span class="sxs-lookup"><span data-stu-id="30b82-126">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
|[<span data-ttu-id="30b82-127">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="30b82-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="30b82-128">В настоящее время не используется и зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="30b82-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="30b82-129">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="30b82-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="30b82-130">Предоставляет текстовое описание состояния отклика.</span><span class="sxs-lookup"><span data-stu-id="30b82-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="30b82-131">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="30b82-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="30b82-132">Предоставляет дополнительные сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="30b82-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="30b82-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="30b82-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="30b82-134">Предоставляет сведения о состоянии запроса.</span><span class="sxs-lookup"><span data-stu-id="30b82-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30b82-135">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="30b82-135">Parent elements</span></span>

|<span data-ttu-id="30b82-136">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="30b82-136">**Element**</span></span>|<span data-ttu-id="30b82-137">**Описание**</span><span class="sxs-lookup"><span data-stu-id="30b82-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30b82-138">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="30b82-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="30b82-139">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="30b82-139">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="30b82-140">Примечания</span><span class="sxs-lookup"><span data-stu-id="30b82-140">Remarks</span></span>

<span data-ttu-id="30b82-141">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="30b82-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="30b82-142">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="30b82-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30b82-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="30b82-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30b82-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="30b82-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30b82-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="30b82-145">Schema Name</span></span>  <br/> |<span data-ttu-id="30b82-146">Схема сообщения</span><span class="sxs-lookup"><span data-stu-id="30b82-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="30b82-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="30b82-147">Validation File</span></span>  <br/> |<span data-ttu-id="30b82-148">messages. xsd</span><span class="sxs-lookup"><span data-stu-id="30b82-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30b82-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="30b82-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="30b82-150">См. также</span><span class="sxs-lookup"><span data-stu-id="30b82-150">See also</span></span>

- [<span data-ttu-id="30b82-151">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="30b82-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

