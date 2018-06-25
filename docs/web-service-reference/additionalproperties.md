---
title: AdditionalProperties
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AdditionalProperties
api_type:
- schema
ms.assetid: 7a269aed-dcfd-4c3e-9e14-094e53828101
description: Элемент AdditionalProperties определяет дополнительные свойства для использования в GetItem, UpdateItem, CreateItem, FindItem или запрашивает FindFolder.
ms.openlocfilehash: 64e4f1ee6b24cf8015b7893dc4a904ca8b32d58e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761346"
---
# <a name="additionalproperties"></a><span data-ttu-id="ea4a2-103">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="ea4a2-103">AdditionalProperties</span></span>

<span data-ttu-id="ea4a2-104">Элемент **AdditionalProperties** определяет дополнительные свойства для использования в [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)или запрашивает [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="ea4a2-104">The **AdditionalProperties** element identifies additional properties for use in [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 <span data-ttu-id="ea4a2-105">**NonEmptyArrayOfPathsToElementType**</span><span class="sxs-lookup"><span data-stu-id="ea4a2-105">**NonEmptyArrayOfPathsToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea4a2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ea4a2-106">Attributes and elements</span></span>

<span data-ttu-id="ea4a2-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea4a2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ea4a2-108">Attributes</span></span>

<span data-ttu-id="ea4a2-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea4a2-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ea4a2-110">Child elements</span></span>

|<span data-ttu-id="ea4a2-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea4a2-111">**Element**</span></span>|<span data-ttu-id="ea4a2-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea4a2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea4a2-113">ExtendedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ea4a2-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="ea4a2-114">Задает расширенные свойства MAPI для получения, установки или создать.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-114">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="ea4a2-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ea4a2-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="ea4a2-116">Идентифицирует часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="ea4a2-117">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="ea4a2-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="ea4a2-118">Идентифицирует часто упоминаемые свойства словаря по URI.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-118">Identifies frequently referenced dictionary properties by URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea4a2-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ea4a2-119">Parent elements</span></span>

|<span data-ttu-id="ea4a2-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea4a2-120">**Element**</span></span>|<span data-ttu-id="ea4a2-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea4a2-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea4a2-122">FolderShape</span><span class="sxs-lookup"><span data-stu-id="ea4a2-122">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="ea4a2-123">Задает свойства папки для включения в [GetFolder](getfolder.md), [FindFolder](findfolder.md)или [SyncFolderHierarchy](syncfolderhierarchy.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-123">Identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span><br/><br/>  <span data-ttu-id="ea4a2-124">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-124">The following are the XPath expressions to this element:</span></span><br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="ea4a2-125">ItemShape</span><span class="sxs-lookup"><span data-stu-id="ea4a2-125">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="ea4a2-126">Определяет свойства элемента и содержимого для включения в [GetItem](getitem.md), [FindItem](finditem.md)или [SyncFolderItems](syncfolderitems.md) ответа.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-126">Identifies the item properties and content to include in a [GetItem](getitem.md), [FindItem](finditem.md), or [SyncFolderItems](syncfolderitems.md) response.</span></span><br/><br/>  <span data-ttu-id="ea4a2-127">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-127">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="ea4a2-128">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="ea4a2-128">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="ea4a2-129">Определяет дополнительные расширенные свойства элемента для возврата в ответ на запрос [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="ea4a2-129">Identifies additional extended item properties to return in a response to a [GetItem](getitem.md) request.</span></span><br/><br/> <span data-ttu-id="ea4a2-130">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-130">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea4a2-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="ea4a2-131">Remarks</span></span>

<span data-ttu-id="ea4a2-132">Не все дочерние элементы можно использовать с [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)или [FindFolder](findfolder.md) запросов.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-132">Not all the child elements can be used with [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> <span data-ttu-id="ea4a2-133">Свойство должно быть применимы к папке или элемента, к которому осуществляется.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-133">The property must be applicable to the folder or item that is accessed.</span></span> <span data-ttu-id="ea4a2-134">Используйте расширенные свойства для доступа к другим свойствам.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-134">Use extended properties to access other properties.</span></span> <span data-ttu-id="ea4a2-135">Если свойство не существует для данного элемента, соответствующий элемент не будет передан в результирующем XML-документе.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-135">If the property does not exist for a given item, no corresponding element will be emitted into the resulting XML.</span></span> 
  
<span data-ttu-id="ea4a2-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="ea4a2-137">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="ea4a2-137">This element is optional.</span></span>
  
## <a name="example"></a><span data-ttu-id="ea4a2-138">Пример</span><span class="sxs-lookup"><span data-stu-id="ea4a2-138">Example</span></span>

<span data-ttu-id="ea4a2-139">В следующем примере запрос показано, как получить Тема элемента с помощью элемента **AdditionalProperties** .</span><span class="sxs-lookup"><span data-stu-id="ea4a2-139">The following request example shows how to get an item subject by using the **AdditionalProperties** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="ASkAS="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="ea4a2-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ea4a2-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea4a2-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ea4a2-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea4a2-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ea4a2-142">Schema Name</span></span>  <br/> |<span data-ttu-id="ea4a2-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ea4a2-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="ea4a2-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ea4a2-144">Validation File</span></span>  <br/> |<span data-ttu-id="ea4a2-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea4a2-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea4a2-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ea4a2-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea4a2-147">False</span><span class="sxs-lookup"><span data-stu-id="ea4a2-147">False</span></span>  <br/> |
   

