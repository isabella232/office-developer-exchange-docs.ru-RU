---
title: ContentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContentId
api_type:
- schema
ms.assetid: bc59100d-6079-414b-a6e0-7c15feaa3184
description: Элемент ContentId представляет идентификатор для содержимого вложения. Идентификатору ContentId можно присвоить любое строковое значение. Приложения могут использовать идентификаторы ContentId для реализации собственных механизмов идентификации.
ms.openlocfilehash: dc46ae4b33d435f5d47eb7deb39e92fd0170194b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761795"
---
# <a name="contentid"></a><span data-ttu-id="fc527-105">ContentId</span><span class="sxs-lookup"><span data-stu-id="fc527-105">ContentId</span></span>

<span data-ttu-id="fc527-106">Элемент **ContentId** представляет идентификатор для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="fc527-106">The **ContentId** element represents an identifier for the contents of an attachment.</span></span> <span data-ttu-id="fc527-107">Идентификатору **ContentId** можно присвоить любое строковое значение.</span><span class="sxs-lookup"><span data-stu-id="fc527-107">**ContentId** can be set to any string value.</span></span> <span data-ttu-id="fc527-108">Приложения могут использовать идентификаторы **ContentId** для реализации собственных механизмов идентификации.</span><span class="sxs-lookup"><span data-stu-id="fc527-108">Applications can use **ContentId** to implement their own identification mechanisms.</span></span> 
  
```xml
<ContentId/>
```

 <span data-ttu-id="fc527-109">**String**</span><span class="sxs-lookup"><span data-stu-id="fc527-109">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc527-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fc527-110">Attributes and elements</span></span>

<span data-ttu-id="fc527-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fc527-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc527-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fc527-112">Attributes</span></span>

<span data-ttu-id="fc527-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc527-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc527-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fc527-114">Child elements</span></span>

<span data-ttu-id="fc527-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="fc527-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc527-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fc527-116">Parent elements</span></span>

|<span data-ttu-id="fc527-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc527-117">**Element**</span></span>|<span data-ttu-id="fc527-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc527-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc527-119">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="fc527-119">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="fc527-120">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc527-120">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="fc527-121">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="fc527-121">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="fc527-122">Представляет файл, присоединенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fc527-122">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fc527-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fc527-123">Text value</span></span>

<span data-ttu-id="fc527-124">Строковое значение представляет идентификатор для содержимого вложения.</span><span class="sxs-lookup"><span data-stu-id="fc527-124">The string value represents the identifier to the contents of an attachment.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fc527-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="fc527-125">Remarks</span></span>

<span data-ttu-id="fc527-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fc527-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc527-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fc527-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc527-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fc527-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc527-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fc527-129">Schema name</span></span>  <br/> |<span data-ttu-id="fc527-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fc527-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc527-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fc527-131">Validation file</span></span>  <br/> |<span data-ttu-id="fc527-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fc527-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc527-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fc527-133">Can be empty</span></span>  <br/> |<span data-ttu-id="fc527-134">False</span><span class="sxs-lookup"><span data-stu-id="fc527-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc527-135">См. также</span><span class="sxs-lookup"><span data-stu-id="fc527-135">See also</span></span>



- [<span data-ttu-id="fc527-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fc527-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

