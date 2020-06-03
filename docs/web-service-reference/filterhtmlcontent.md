---
title: филтерхтмлконтент
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: Элемент Филтерхтмлконтент указывает, фильтруется ли потенциально небезопасное HTML-содержимое из элемента или вложения.
ms.openlocfilehash: 28e3be86b550c3f330fbb6846b64732b5674304d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462677"
---
# <a name="filterhtmlcontent"></a><span data-ttu-id="0ee33-103">филтерхтмлконтент</span><span class="sxs-lookup"><span data-stu-id="0ee33-103">FilterHtmlContent</span></span>

<span data-ttu-id="0ee33-104">Элемент **филтерхтмлконтент** указывает, фильтруется ли потенциально небезопасное HTML-содержимое из элемента или вложения.</span><span class="sxs-lookup"><span data-stu-id="0ee33-104">The **FilterHtmlContent** element specifies whether potentially unsafe HTML content is filtered from an item or attachment.</span></span> 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 <span data-ttu-id="0ee33-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="0ee33-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0ee33-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0ee33-106">Attributes and elements</span></span>

<span data-ttu-id="0ee33-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0ee33-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0ee33-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0ee33-108">Attributes</span></span>

<span data-ttu-id="0ee33-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0ee33-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0ee33-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0ee33-110">Child elements</span></span>

<span data-ttu-id="0ee33-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0ee33-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0ee33-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0ee33-112">Parent elements</span></span>

|<span data-ttu-id="0ee33-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0ee33-113">**Element**</span></span>|<span data-ttu-id="0ee33-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0ee33-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0ee33-115">аттачментшапе</span><span class="sxs-lookup"><span data-stu-id="0ee33-115">AttachmentShape</span></span>](attachmentshape.md) <br/> | <span data-ttu-id="0ee33-116">Определяет дополнительные свойства, возвращаемые в ответе на запрос [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="0ee33-116">Identifies additional properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span>  <br/><br/>  <span data-ttu-id="0ee33-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="0ee33-117">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[<span data-ttu-id="0ee33-118">итемшапе</span><span class="sxs-lookup"><span data-stu-id="0ee33-118">ItemShape</span></span>](itemshape.md) <br/> | <span data-ttu-id="0ee33-119">Определяет свойства и контент элемента, включаемые в ответ GetItem, FindItem или SyncFolderItems.</span><span class="sxs-lookup"><span data-stu-id="0ee33-119">Identifies the item properties and content to include in a GetItem, FindItem, or SyncFolderItems response.</span></span>  <br/> <br/> <span data-ttu-id="0ee33-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="0ee33-120">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0ee33-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0ee33-121">Text value</span></span>

<span data-ttu-id="0ee33-122">Этот элемент может иметь **значение true** или **false**.</span><span class="sxs-lookup"><span data-stu-id="0ee33-122">This element can be either **true** or **false**.</span></span> <span data-ttu-id="0ee33-123">Значение по умолчанию — **false**.</span><span class="sxs-lookup"><span data-stu-id="0ee33-123">The default value is **false**.</span></span> <span data-ttu-id="0ee33-124">Это логический тип данных.</span><span class="sxs-lookup"><span data-stu-id="0ee33-124">This is a Boolean data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0ee33-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="0ee33-125">Remarks</span></span>

<span data-ttu-id="0ee33-126">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0ee33-126">This element is optional.</span></span>
  
<span data-ttu-id="0ee33-127">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0ee33-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0ee33-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0ee33-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0ee33-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0ee33-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0ee33-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0ee33-130">Schema Name</span></span>  <br/> |<span data-ttu-id="0ee33-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0ee33-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="0ee33-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0ee33-132">Validation File</span></span>  <br/> |<span data-ttu-id="0ee33-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0ee33-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0ee33-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0ee33-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="0ee33-135">False</span><span class="sxs-lookup"><span data-stu-id="0ee33-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0ee33-136">См. также</span><span class="sxs-lookup"><span data-stu-id="0ee33-136">See also</span></span>

- [<span data-ttu-id="0ee33-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0ee33-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

