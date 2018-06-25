---
title: RootItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: Элемент RootItemId определяет корневой элемент удаленного вложения.
ms.openlocfilehash: 484b185db63c9692eaca7e43c49d6e95375a1a98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835251"
---
# <a name="rootitemid"></a><span data-ttu-id="da720-103">RootItemId</span><span class="sxs-lookup"><span data-stu-id="da720-103">RootItemId</span></span>

<span data-ttu-id="da720-104">Элемент **RootItemId** определяет корневой элемент удаленного вложения.</span><span class="sxs-lookup"><span data-stu-id="da720-104">The **RootItemId** element identifies the root item of a deleted attachment.</span></span> 
  
[<span data-ttu-id="da720-105">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="da720-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
  
[<span data-ttu-id="da720-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="da720-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="da720-107">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="da720-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
[<span data-ttu-id="da720-108">RootItemId</span><span class="sxs-lookup"><span data-stu-id="da720-108">RootItemId</span></span>](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="da720-109">**RootItemIdType**</span><span class="sxs-lookup"><span data-stu-id="da720-109">**RootItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da720-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da720-110">Attributes and elements</span></span>

<span data-ttu-id="da720-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="da720-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da720-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da720-112">Attributes</span></span>

|<span data-ttu-id="da720-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="da720-113">**Attribute**</span></span>|<span data-ttu-id="da720-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da720-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="da720-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="da720-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="da720-116">Определяет корневой элемент удаленного вложения.</span><span class="sxs-lookup"><span data-stu-id="da720-116">Identifies the root item of a deleted attachment.</span></span>  <br/> |
|<span data-ttu-id="da720-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="da720-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="da720-118">Определяет новый ключ изменения корневого элемента удаленного вложения.</span><span class="sxs-lookup"><span data-stu-id="da720-118">Identifies the new change key of the root item of a deleted attachment.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="da720-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da720-119">Child elements</span></span>

<span data-ttu-id="da720-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="da720-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da720-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da720-121">Parent elements</span></span>

|<span data-ttu-id="da720-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da720-122">**Element**</span></span>|<span data-ttu-id="da720-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da720-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da720-124">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="da720-124">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md) <br/> |<span data-ttu-id="da720-125">Содержит состояние и результат запроса DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="da720-125">Contains the status and result of a DeleteAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="da720-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="da720-126">Remarks</span></span>

<span data-ttu-id="da720-127">Элемент **RootItemId** используется только в ответы DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="da720-127">The **RootItemId** element is only used in DeleteAttachment responses.</span></span> <span data-ttu-id="da720-128">Определяет идентификатор корневого элемента и важнее, новый ключ изменения для родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="da720-128">This identifies the root item identifier, and more importantly, the new change key to the parent item.</span></span> 
  
<span data-ttu-id="da720-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="da720-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da720-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da720-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da720-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da720-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da720-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da720-132">Schema name</span></span>  <br/> |<span data-ttu-id="da720-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="da720-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="da720-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da720-134">Validation file</span></span>  <br/> |<span data-ttu-id="da720-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="da720-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da720-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da720-136">Can be empty</span></span>  <br/> |<span data-ttu-id="da720-137">False</span><span class="sxs-lookup"><span data-stu-id="da720-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da720-138">См. также</span><span class="sxs-lookup"><span data-stu-id="da720-138">See also</span></span>



[<span data-ttu-id="da720-139">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="da720-139">DeleteAttachment</span></span>](deleteattachment.md)
  
[<span data-ttu-id="da720-140">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="da720-140">DeleteAttachment operation</span></span>](deleteattachment-operation.md)


- [<span data-ttu-id="da720-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="da720-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

