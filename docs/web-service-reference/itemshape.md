---
title: итемшапе
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemShape
api_type:
- schema
ms.assetid: c5604161-bbc0-40bc-ad75-ff7e837d745f
description: Элемент Итемшапе определяет набор свойств, возвращаемых операцией GetItem, операцией FindItem или ответом операции SyncFolderItems.
ms.openlocfilehash: ffb666ee331b55a4f04cad076c705e4bec980e03
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458126"
---
# <a name="itemshape"></a><span data-ttu-id="72611-103">итемшапе</span><span class="sxs-lookup"><span data-stu-id="72611-103">ItemShape</span></span>

<span data-ttu-id="72611-104">Элемент **итемшапе** определяет набор свойств, возвращаемых [операцией GetItem](getitem-operation.md), [операцией FindItem](finditem-operation.md)или ответом [операции SyncFolderItems](syncfolderitems-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="72611-104">The **ItemShape** element identifies a set of properties to return in a [GetItem operation](getitem-operation.md), [FindItem operation](finditem-operation.md), or [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> 
  
```XML
<ItemShape>
   <BaseShape/>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <ConvertHtmlCodePageToUTF8/>
   <AdditionalProperties/>
</ItemShape>
```

 <span data-ttu-id="72611-105">**итемреспонсешапетипе**</span><span class="sxs-lookup"><span data-stu-id="72611-105">**ItemResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72611-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="72611-106">Attributes and elements</span></span>

<span data-ttu-id="72611-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="72611-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72611-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="72611-108">Attributes</span></span>

<span data-ttu-id="72611-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="72611-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72611-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="72611-110">Child elements</span></span>

|<span data-ttu-id="72611-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="72611-111">**Element**</span></span>|<span data-ttu-id="72611-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="72611-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72611-113">басешапе</span><span class="sxs-lookup"><span data-stu-id="72611-113">BaseShape</span></span>](baseshape.md) <br/> |<span data-ttu-id="72611-114">Определяет базовую конфигурацию свойств, возвращаемых в ответе элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="72611-114">Identifies the basic configuration of properties to return in an item or folder response.</span></span>  <br/> |
|[<span data-ttu-id="72611-115">инклудемимеконтент</span><span class="sxs-lookup"><span data-stu-id="72611-115">IncludeMimeContent</span></span>](includemimecontent.md) <br/> |<span data-ttu-id="72611-116">Указывает, будет ли в ответе возвращено содержимое MIME для элемента с многоцелевыми почтовыми расширениями.</span><span class="sxs-lookup"><span data-stu-id="72611-116">Specifies whether the Multipurpose Internet Mail Extensions (MIME) content of an item is returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="72611-117">BodyType</span><span class="sxs-lookup"><span data-stu-id="72611-117">BodyType</span></span>](bodytype.md) <br/> |<span data-ttu-id="72611-118">Определяет способ форматирования основного текста в отклике.</span><span class="sxs-lookup"><span data-stu-id="72611-118">Identifies how the body text is formatted in the response.</span></span>  <br/> |
|[<span data-ttu-id="72611-119">ConvertHtmlCodePageToUTF8</span><span class="sxs-lookup"><span data-stu-id="72611-119">ConvertHtmlCodePageToUTF8</span></span>](converthtmlcodepagetoutf8.md) <br/> |<span data-ttu-id="72611-120">Указывает, преобразуется ли текст HTML элемента в формат UTF8.</span><span class="sxs-lookup"><span data-stu-id="72611-120">Indicates whether the item HTML body is converted to UTF8.</span></span>  <br/> |
|[<span data-ttu-id="72611-121">филтерхтмлконтент</span><span class="sxs-lookup"><span data-stu-id="72611-121">FilterHtmlContent</span></span>](filterhtmlcontent.md) <br/> |<span data-ttu-id="72611-122">Указывает, включена ли фильтрация HTML-содержимого.</span><span class="sxs-lookup"><span data-stu-id="72611-122">Specifies whether HTML content filtering is enabled.</span></span>  <br/> |
|[<span data-ttu-id="72611-123">аддитионалпропертиес</span><span class="sxs-lookup"><span data-stu-id="72611-123">AdditionalProperties</span></span>](additionalproperties.md) <br/> |<span data-ttu-id="72611-124">Определяет дополнительные свойства, возвращаемые в ответе.</span><span class="sxs-lookup"><span data-stu-id="72611-124">Identifies additional properties to return in a response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="72611-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="72611-125">Parent elements</span></span>

|<span data-ttu-id="72611-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="72611-126">**Element**</span></span>|<span data-ttu-id="72611-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="72611-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="72611-128">GetItem</span><span class="sxs-lookup"><span data-stu-id="72611-128">GetItem</span></span>](getitem.md) <br/> |<span data-ttu-id="72611-129">Определяет запрос на извлечение элементов из почтового ящика в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="72611-129">Defines a request to retrieve items from a mailbox in the Exchange store.</span></span>  <br/> <span data-ttu-id="72611-130">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="72611-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetItem` <br/> |
|[<span data-ttu-id="72611-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="72611-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="72611-132">Определяет запрос на поиск всех элементов, которые содержатся в папке.</span><span class="sxs-lookup"><span data-stu-id="72611-132">Defines a request to find all items that are contained in a folder.</span></span>  <br/> <span data-ttu-id="72611-133">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="72611-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
|[<span data-ttu-id="72611-134">SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="72611-134">SyncFolderItems</span></span>](syncfolderitems.md) <br/> |<span data-ttu-id="72611-135">Определяет запрос на синхронизацию элементов в папке хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="72611-135">Defines a request to synchronize items in an Exchange store folder.</span></span>  <br/> <span data-ttu-id="72611-136">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="72611-136">The following is the XPath expression to this element:</span></span>  <br/>  `/SyncFolderItems` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="72611-137">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="72611-137">Text value</span></span>

<span data-ttu-id="72611-138">Нет.</span><span class="sxs-lookup"><span data-stu-id="72611-138">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="72611-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="72611-139">Remarks</span></span>

<span data-ttu-id="72611-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="72611-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72611-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="72611-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72611-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="72611-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="72611-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="72611-143">Schema Name</span></span>  <br/> |<span data-ttu-id="72611-144">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="72611-144">Messages schema</span></span>  <br/> |
|<span data-ttu-id="72611-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="72611-145">Validation File</span></span>  <br/> |<span data-ttu-id="72611-146">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="72611-146">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="72611-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="72611-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="72611-148">False</span><span class="sxs-lookup"><span data-stu-id="72611-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="72611-149">См. также</span><span class="sxs-lookup"><span data-stu-id="72611-149">See also</span></span>



[<span data-ttu-id="72611-150">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="72611-150">GetItem operation</span></span>](getitem-operation.md)
  
[<span data-ttu-id="72611-151">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="72611-151">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="72611-152">Операция SyncFolderItems</span><span class="sxs-lookup"><span data-stu-id="72611-152">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)


- [<span data-ttu-id="72611-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="72611-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

