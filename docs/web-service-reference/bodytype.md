---
title: BodyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BodyType
api_type:
- schema
ms.assetid: d42ec77b-fb9f-404a-9bf2-1801e8744676
description: Элемент BodyType определяет способ форматирования основного текста в ответе.
ms.openlocfilehash: f8be2e96390b40faa367cf0d34c533accc3b8afb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761595"
---
# <a name="bodytype"></a><span data-ttu-id="15a6e-103">BodyType</span><span class="sxs-lookup"><span data-stu-id="15a6e-103">BodyType</span></span>

<span data-ttu-id="15a6e-104">Элемент **BodyType** определяет способ форматирования основного текста в ответе.</span><span class="sxs-lookup"><span data-stu-id="15a6e-104">The **BodyType** element identifies how the body text is formatted in the response.</span></span> 
  
```xml
<BodyType>Best or HTML or Text</BodyType>
```

<span data-ttu-id="15a6e-105">**BodyTypeResponseType**</span><span class="sxs-lookup"><span data-stu-id="15a6e-105">**BodyTypeResponseType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="15a6e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="15a6e-106">Attributes and elements</span></span>

<span data-ttu-id="15a6e-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="15a6e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15a6e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="15a6e-108">Attributes</span></span>

<span data-ttu-id="15a6e-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="15a6e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15a6e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="15a6e-110">Child elements</span></span>

<span data-ttu-id="15a6e-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="15a6e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15a6e-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="15a6e-112">Parent elements</span></span>

|<span data-ttu-id="15a6e-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="15a6e-113">**Element**</span></span>|<span data-ttu-id="15a6e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15a6e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15a6e-115">ItemShape</span><span class="sxs-lookup"><span data-stu-id="15a6e-115">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="15a6e-116">Определяет свойства элемента и содержимого для включения в GetItem, FindItem или SyncFolderItems ответа.</span><span class="sxs-lookup"><span data-stu-id="15a6e-116">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/><br/><span data-ttu-id="15a6e-117">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="15a6e-117">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape`<br/><br/>`/FindItem/ItemShape`<br/><br/>`/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="15a6e-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="15a6e-118">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="15a6e-119">Определяет дополнительные расширенные свойства элемента для возврата в ответ на запрос [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="15a6e-119">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/><span data-ttu-id="15a6e-120">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="15a6e-120">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15a6e-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="15a6e-121">Text value</span></span>

<span data-ttu-id="15a6e-122">В следующей таблице приведены возможные значения для элемента **типа текста сообщения** .</span><span class="sxs-lookup"><span data-stu-id="15a6e-122">The following table lists the possible values for the **BodyType** element.</span></span> 
  
|<span data-ttu-id="15a6e-123">**Значение**</span><span class="sxs-lookup"><span data-stu-id="15a6e-123">**Value**</span></span>|<span data-ttu-id="15a6e-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="15a6e-124">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="15a6e-125">Рекомендации</span><span class="sxs-lookup"><span data-stu-id="15a6e-125">Best</span></span>  <br/> |<span data-ttu-id="15a6e-126">В ответе будут возвращены содержательности доступное содержимое основного текста.</span><span class="sxs-lookup"><span data-stu-id="15a6e-126">The response will return the richest available content of body text.</span></span> <span data-ttu-id="15a6e-127">Это полезно, если не известно, является ли содержимое текста или HTML.</span><span class="sxs-lookup"><span data-stu-id="15a6e-127">This is useful if it is unknown whether the content is text or HTML.</span></span><br/><br/> <span data-ttu-id="15a6e-128">Возвращаемое значение body будет текст основному сохраненных обычного текста.</span><span class="sxs-lookup"><span data-stu-id="15a6e-128">The returned body will be text if the stored body is plain text.</span></span> <span data-ttu-id="15a6e-129">В противном случае ответ вернет HTML Если сохраненные текст в формате HTML или RTF.</span><span class="sxs-lookup"><span data-stu-id="15a6e-129">Otherwise, the response will return HTML if the stored body is in either HTML or RTF format.</span></span><br/><br/> <span data-ttu-id="15a6e-130">Это значение используется по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="15a6e-130">This is the default value.</span></span>  <br/> |
|<span data-ttu-id="15a6e-131">HTML</span><span class="sxs-lookup"><span data-stu-id="15a6e-131">HTML</span></span>  <br/> |<span data-ttu-id="15a6e-132">Основной текст элемента возвращает ответ как HTML.</span><span class="sxs-lookup"><span data-stu-id="15a6e-132">The response will return an item body as HTML.</span></span>  <br/> |
|<span data-ttu-id="15a6e-133">Text</span><span class="sxs-lookup"><span data-stu-id="15a6e-133">Text</span></span>  <br/> |<span data-ttu-id="15a6e-134">В ответе будут возвращены основной текст элемента, как обычный текст.</span><span class="sxs-lookup"><span data-stu-id="15a6e-134">The response will return an item body as plain text.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="15a6e-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="15a6e-135">Remarks</span></span>

<span data-ttu-id="15a6e-136">Можно определить тип возвращаемого в ответе, установив атрибут **BodyType** элемента [Body](body.md) текст.</span><span class="sxs-lookup"><span data-stu-id="15a6e-136">You can identify the type of body returned in the response by checking the **BodyType** attribute of the [Body](body.md) element.</span></span> <span data-ttu-id="15a6e-137">Атрибут **BodyType** определяет текст HTML или текст.</span><span class="sxs-lookup"><span data-stu-id="15a6e-137">The **BodyType** attribute will identify the body as either HTML or text.</span></span> 
  
<span data-ttu-id="15a6e-138">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="15a6e-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="15a6e-139">Пример</span><span class="sxs-lookup"><span data-stu-id="15a6e-139">Example</span></span>

<span data-ttu-id="15a6e-140">Следующий пример запроса показано, где используется элемент **типа текста сообщения** .</span><span class="sxs-lookup"><span data-stu-id="15a6e-140">The following example of a request shows where a **BodyType** element is used.</span></span> 
  
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
        <t:BodyType>Best</t:BodyType>
      </AttachmentShape>
      <AttachmentIds>
        <t:AttachmentId Id="ASkAS="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="15a6e-141">В атрибуте Id был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="15a6e-141">The Id attribute has been shortened to preserve readability.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15a6e-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="15a6e-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15a6e-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="15a6e-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15a6e-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="15a6e-144">Schema Name</span></span>  <br/> |<span data-ttu-id="15a6e-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="15a6e-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="15a6e-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="15a6e-146">Validation File</span></span>  <br/> |<span data-ttu-id="15a6e-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15a6e-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15a6e-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="15a6e-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="15a6e-149">False</span><span class="sxs-lookup"><span data-stu-id="15a6e-149">False</span></span>  <br/> |
   

