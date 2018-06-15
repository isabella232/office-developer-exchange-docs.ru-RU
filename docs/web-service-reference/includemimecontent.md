---
title: IncludeMimeContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IncludeMimeContent
api_type:
- schema
ms.assetid: 3f3c2300-55cd-41c0-900e-b470b290d52f
description: Элемент IncludeMimeContent указывает, возвращается ли содержимое Multipurpose Internet Mail Extensions (MIME) элемента или вложения в ответе.
ms.openlocfilehash: ddd6988be93231ac7c574a2e19c9ba4b562c7d0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833903"
---
# <a name="includemimecontent"></a><span data-ttu-id="0ca3d-103">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="0ca3d-103">IncludeMimeContent</span></span>

<span data-ttu-id="0ca3d-104">Элемент **IncludeMimeContent** указывает, возвращается ли содержимое Multipurpose Internet Mail Extensions (MIME) элемента или вложения в ответе.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-104">The **IncludeMimeContent** element specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item or attachment is returned in the response.</span></span> 
  
```xml
<IncludeMimeContent>true or false</IncludeMimeContent>
```

 <span data-ttu-id="0ca3d-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0ca3d-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ca3d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0ca3d-106">Attributes and elements</span></span>

<span data-ttu-id="0ca3d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ca3d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0ca3d-108">Attributes</span></span>

<span data-ttu-id="0ca3d-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ca3d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0ca3d-110">Child elements</span></span>

<span data-ttu-id="0ca3d-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ca3d-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0ca3d-112">Parent elements</span></span>

|<span data-ttu-id="0ca3d-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0ca3d-113">**Element**</span></span>|<span data-ttu-id="0ca3d-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ca3d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ca3d-115">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="0ca3d-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="0ca3d-116">Определяет дополнительные свойства, возвращаемые в ответ на запрос [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="0ca3d-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/> <br/> <span data-ttu-id="0ca3d-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="0ca3d-118">ItemShape</span><span class="sxs-lookup"><span data-stu-id="0ca3d-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="0ca3d-119">Определяет свойства элемента и содержимого для включения в GetItem, FindItem или SyncFolderItems ответа.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="0ca3d-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-120">The following are the XPath expressions to this element:</span></span><br/>  <br/>  `/GetItem/ItemShape` <br/><br/>  `/FindItem/ItemShape` <br/><br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ca3d-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0ca3d-121">Text value</span></span>

<span data-ttu-id="0ca3d-122">Этот элемент может быть значение **true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="0ca3d-123">Значение по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-123">The default value is **false**.</span></span> <span data-ttu-id="0ca3d-124">Это тип данных Boolean.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ca3d-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="0ca3d-125">Remarks</span></span>

<span data-ttu-id="0ca3d-126">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-126">This element is optional.</span></span>
  
<span data-ttu-id="0ca3d-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="0ca3d-128">Пример</span><span class="sxs-lookup"><span data-stu-id="0ca3d-128">Example</span></span>

<span data-ttu-id="0ca3d-129">Запрос в следующем примере показано, как для задания **IncludeMimeContent** элемента.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-129">The following example of a request demonstrates a how to set the **IncludeMimeContent** element.</span></span> 
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0ca3d-130">В атрибуте Id вложения усекается, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="0ca3d-130">The attachment Id attribute is truncated to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ca3d-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0ca3d-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ca3d-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0ca3d-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ca3d-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0ca3d-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0ca3d-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0ca3d-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ca3d-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0ca3d-135">Validation File</span></span>  <br/> |<span data-ttu-id="0ca3d-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0ca3d-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ca3d-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0ca3d-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ca3d-138">False</span><span class="sxs-lookup"><span data-stu-id="0ca3d-138">False</span></span>  <br/> |
   
