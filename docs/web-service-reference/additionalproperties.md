---
title: аддитионалпропертиес
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
description: Элемент Аддитионалпропертиес определяет дополнительные свойства для использования в запросах GetItem, UpdateItem, CreateItem, FindItem или FindFolder.
ms.openlocfilehash: 90a307ba4d5ece10e15d2cec56cf5042c3d38685
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455816"
---
# <a name="additionalproperties"></a><span data-ttu-id="2c43d-103">аддитионалпропертиес</span><span class="sxs-lookup"><span data-stu-id="2c43d-103">AdditionalProperties</span></span>

<span data-ttu-id="2c43d-104">Элемент **аддитионалпропертиес** определяет дополнительные свойства для использования в запросах [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)или [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="2c43d-104">The **AdditionalProperties** element identifies additional properties for use in [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> 
  
```xml
<AdditionalProperties>
   <ExtendedFieldURI/>
   <FieldURI/>
   <IndexedFieldURI/>
</AdditionalProperties>
```

 <span data-ttu-id="2c43d-105">**нонемптяррайофпасстоелементтипе**</span><span class="sxs-lookup"><span data-stu-id="2c43d-105">**NonEmptyArrayOfPathsToElementType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2c43d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2c43d-106">Attributes and elements</span></span>

<span data-ttu-id="2c43d-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2c43d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2c43d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2c43d-108">Attributes</span></span>

<span data-ttu-id="2c43d-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2c43d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2c43d-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2c43d-110">Child elements</span></span>

|<span data-ttu-id="2c43d-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2c43d-111">**Element**</span></span>|<span data-ttu-id="2c43d-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c43d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c43d-113">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="2c43d-113">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="2c43d-114">Определяет расширенные свойства MAPI, которые необходимо получить, задать или создать.</span><span class="sxs-lookup"><span data-stu-id="2c43d-114">Identifies extended MAPI properties to get, set, or create.</span></span>  <br/> |
|[<span data-ttu-id="2c43d-115">фиелдури</span><span class="sxs-lookup"><span data-stu-id="2c43d-115">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="2c43d-116">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="2c43d-116">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="2c43d-117">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="2c43d-117">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="2c43d-118">Определяет свойства часто упоминаемого словаря по универсальному коду ресурса (URI).</span><span class="sxs-lookup"><span data-stu-id="2c43d-118">Identifies frequently referenced dictionary properties by URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2c43d-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2c43d-119">Parent elements</span></span>

|<span data-ttu-id="2c43d-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2c43d-120">**Element**</span></span>|<span data-ttu-id="2c43d-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2c43d-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2c43d-122">фолдершапе</span><span class="sxs-lookup"><span data-stu-id="2c43d-122">FolderShape</span></span>](foldershape.md) <br/> | <span data-ttu-id="2c43d-123">Определяет свойства папки, включаемые в ответ [на](getfolder.md)SyncFolderHierarchy, [FindFolder](findfolder.md)или [SyncFolderHierarchy](syncfolderhierarchy.md) .</span><span class="sxs-lookup"><span data-stu-id="2c43d-123">Identifies the folder properties to include in a [GetFolder](getfolder.md), [FindFolder](findfolder.md), or [SyncFolderHierarchy](syncfolderhierarchy.md) response.</span></span><br/><br/>  <span data-ttu-id="2c43d-124">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="2c43d-124">The following are the XPath expressions to this element:</span></span><br/><br/>  `/FindFolder/FolderShape` <br/>  `/GetFolder/FolderShape` <br/>  `/SyncFolderHierarchy/FolderShape` <br/> |
|[<span data-ttu-id="2c43d-125">итемшапе</span><span class="sxs-lookup"><span data-stu-id="2c43d-125">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="2c43d-126">Определяет свойства и контент элемента, включаемые в ответ [GetItem](getitem.md), [FindItem](finditem.md)или [SyncFolderItems](syncfolderitems.md) .</span><span class="sxs-lookup"><span data-stu-id="2c43d-126">Identifies the item properties and content to include in a [GetItem](getitem.md), [FindItem](finditem.md), or [SyncFolderItems](syncfolderitems.md) response.</span></span><br/><br/>  <span data-ttu-id="2c43d-127">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="2c43d-127">The following are the XPath expressions to this element:</span></span><br/><br/>  `/GetItem/ItemShape` <br/>  `/FindItem/ItemShape` <br/>  `/SyncFolderItems/ItemShape` <br/> |
|[<span data-ttu-id="2c43d-128">аттачментшапе</span><span class="sxs-lookup"><span data-stu-id="2c43d-128">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="2c43d-129">Определяет дополнительные свойства расширенного элемента, которые возвращаются в ответ на запрос [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="2c43d-129">Identifies additional extended item properties to return in a response to a [GetItem](getitem.md) request.</span></span><br/><br/> <span data-ttu-id="2c43d-130">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="2c43d-130">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetAttachment/AttachmentShape` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2c43d-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="2c43d-131">Remarks</span></span>

<span data-ttu-id="2c43d-132">Не все дочерние элементы могут использоваться с запросами [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md)или [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="2c43d-132">Not all the child elements can be used with [GetItem](getitem.md), [UpdateItem](updateitem.md), [CreateItem](createitem.md), [FindItem](finditem.md), or [FindFolder](findfolder.md) requests.</span></span> <span data-ttu-id="2c43d-133">Свойство должно быть применимым к папке или элементу, к которому осуществляется доступ.</span><span class="sxs-lookup"><span data-stu-id="2c43d-133">The property must be applicable to the folder or item that is accessed.</span></span> <span data-ttu-id="2c43d-134">Используйте расширенные свойства для доступа к другим свойствам.</span><span class="sxs-lookup"><span data-stu-id="2c43d-134">Use extended properties to access other properties.</span></span> <span data-ttu-id="2c43d-135">Если свойство не существует для данного элемента, в результирующий XML-файл не будет выдаваться соответствующий элемент.</span><span class="sxs-lookup"><span data-stu-id="2c43d-135">If the property does not exist for a given item, no corresponding element will be emitted into the resulting XML.</span></span> 
  
<span data-ttu-id="2c43d-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2c43d-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="2c43d-137">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="2c43d-137">This element is optional.</span></span>
  
## <a name="example"></a><span data-ttu-id="2c43d-138">Пример</span><span class="sxs-lookup"><span data-stu-id="2c43d-138">Example</span></span>

<span data-ttu-id="2c43d-139">В приведенном ниже примере запроса показано, как получить тему элемента с помощью элемента **аддитионалпропертиес** .</span><span class="sxs-lookup"><span data-stu-id="2c43d-139">The following request example shows how to get an item subject by using the **AdditionalProperties** element.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="2c43d-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2c43d-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2c43d-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2c43d-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2c43d-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2c43d-142">Schema Name</span></span>  <br/> |<span data-ttu-id="2c43d-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2c43d-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="2c43d-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2c43d-144">Validation File</span></span>  <br/> |<span data-ttu-id="2c43d-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2c43d-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2c43d-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2c43d-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="2c43d-147">False</span><span class="sxs-lookup"><span data-stu-id="2c43d-147">False</span></span>  <br/> |
   

