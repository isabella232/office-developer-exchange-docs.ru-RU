---
title: AttachmentId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentId
api_type:
- schema
ms.assetid: 55a5fd77-60d1-40fa-8144-770600cedc6a
description: Элемент AttachmentId определяет вложенный элемент или файл. Этот элемент используется в ответах CreateAttachment.
ms.openlocfilehash: b5dc9299b615f0fc01b8afcbaabf0ec7996e53d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459113"
---
# <a name="attachmentid"></a><span data-ttu-id="c0946-104">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="c0946-104">AttachmentId</span></span>

<span data-ttu-id="c0946-105">Элемент **AttachmentId** определяет вложенный элемент или файл.</span><span class="sxs-lookup"><span data-stu-id="c0946-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="c0946-106">Этот элемент используется в ответах CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="c0946-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="c0946-107">**аттачментидтипе**</span><span class="sxs-lookup"><span data-stu-id="c0946-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0946-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c0946-108">Attributes and elements</span></span>

<span data-ttu-id="c0946-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c0946-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0946-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c0946-110">Attributes</span></span>

|<span data-ttu-id="c0946-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="c0946-111">**Attribute**</span></span>|<span data-ttu-id="c0946-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c0946-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0946-113">**Id**</span><span class="sxs-lookup"><span data-stu-id="c0946-113">**Id**</span></span> <br/> |<span data-ttu-id="c0946-114">Определяет уникальный идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="c0946-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="c0946-115">**рутитемид**</span><span class="sxs-lookup"><span data-stu-id="c0946-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="c0946-116">Определяет уникальный идентификатор элемента корневого хранилища, к которому присоединено вложение.</span><span class="sxs-lookup"><span data-stu-id="c0946-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="c0946-117">**рутитемчанжекэй**</span><span class="sxs-lookup"><span data-stu-id="c0946-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="c0946-118">Определяет ключ изменения элемента корневого хранилища, к которому присоединено вложение.</span><span class="sxs-lookup"><span data-stu-id="c0946-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c0946-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c0946-119">Child elements</span></span>

<span data-ttu-id="c0946-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c0946-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c0946-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c0946-121">Parent elements</span></span>

|<span data-ttu-id="c0946-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c0946-122">**Element**</span></span>|<span data-ttu-id="c0946-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c0946-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0946-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="c0946-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="c0946-125">Представляет элемент Exchange, присоединенный к другому элементу Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0946-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="c0946-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="c0946-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="c0946-127">Представляет файл, присоединенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="c0946-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c0946-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="c0946-128">Remarks</span></span>

<span data-ttu-id="c0946-129">Важно отметить, что при создании вложения изменяется ключ изменения корневого элемента.</span><span class="sxs-lookup"><span data-stu-id="c0946-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="c0946-130">Элемент [AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) используется в запросах DeleteAttachment и GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="c0946-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="c0946-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c0946-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0946-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c0946-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0946-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c0946-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c0946-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c0946-134">Schema name</span></span>  <br/> |<span data-ttu-id="c0946-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c0946-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="c0946-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c0946-136">Validation file</span></span>  <br/> |<span data-ttu-id="c0946-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c0946-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c0946-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c0946-138">Can be empty</span></span>  <br/> |<span data-ttu-id="c0946-139">False</span><span class="sxs-lookup"><span data-stu-id="c0946-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0946-140">См. также</span><span class="sxs-lookup"><span data-stu-id="c0946-140">See also</span></span>

- [<span data-ttu-id="c0946-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c0946-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

