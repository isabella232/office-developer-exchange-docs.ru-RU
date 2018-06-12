---
title: Идентификатора вложения AttachmentId
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
description: Элемент идентификатора вложения AttachmentId определяет вложение элемента или файла. Данный элемент используется в CreateAttachment ответы.
ms.openlocfilehash: 2910503d1661ca3aaeeb4e319deb39f6b57c5c0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761509"
---
# <a name="attachmentid"></a><span data-ttu-id="d36b5-104">Идентификатора вложения AttachmentId</span><span class="sxs-lookup"><span data-stu-id="d36b5-104">AttachmentId</span></span>

<span data-ttu-id="d36b5-105">Элемент **идентификатора вложения AttachmentId** определяет вложение элемента или файла.</span><span class="sxs-lookup"><span data-stu-id="d36b5-105">The **AttachmentId** element identifies an item or file attachment.</span></span> <span data-ttu-id="d36b5-106">Данный элемент используется в CreateAttachment ответы.</span><span class="sxs-lookup"><span data-stu-id="d36b5-106">This element is used in CreateAttachment responses.</span></span> 
  
```xml
<AttachmentId Id="" RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="d36b5-107">**AttachmentIdType**</span><span class="sxs-lookup"><span data-stu-id="d36b5-107">**AttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d36b5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d36b5-108">Attributes and elements</span></span>

<span data-ttu-id="d36b5-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d36b5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d36b5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d36b5-110">Attributes</span></span>

|<span data-ttu-id="d36b5-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="d36b5-111">**Attribute**</span></span>|<span data-ttu-id="d36b5-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d36b5-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d36b5-113">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="d36b5-113">**Id**</span></span> <br/> |<span data-ttu-id="d36b5-114">Указывает уникальный идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="d36b5-114">Identifies the unique identifier of the attachment.</span></span>  <br/> |
|<span data-ttu-id="d36b5-115">**RootItemId**</span><span class="sxs-lookup"><span data-stu-id="d36b5-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="d36b5-116">Указывает уникальный идентификатор корневого элемента хранилища, к которому подключен вложение.</span><span class="sxs-lookup"><span data-stu-id="d36b5-116">Identifies the unique identifier of the root store item to which the attachment is attached.</span></span>  <br/> |
|<span data-ttu-id="d36b5-117">**RootItemChangeKey**</span><span class="sxs-lookup"><span data-stu-id="d36b5-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="d36b5-118">Идентифицирует ключ изменения корневого элемента хранилища, к которому подключен вложение.</span><span class="sxs-lookup"><span data-stu-id="d36b5-118">Identifies the change key of the root store item to which the attachment is attached.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d36b5-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d36b5-119">Child elements</span></span>

<span data-ttu-id="d36b5-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="d36b5-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d36b5-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d36b5-121">Parent elements</span></span>

|<span data-ttu-id="d36b5-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d36b5-122">**Element**</span></span>|<span data-ttu-id="d36b5-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d36b5-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d36b5-124">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="d36b5-124">ItemAttachment</span></span>](itemattachment.md) <br/> |<span data-ttu-id="d36b5-125">Представляет собой элемент Exchange, подключенный к другой элемент Exchange.</span><span class="sxs-lookup"><span data-stu-id="d36b5-125">Represents an Exchange item that is attached to another Exchange item.</span></span>  <br/> |
|[<span data-ttu-id="d36b5-126">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="d36b5-126">FileAttachment</span></span>](fileattachment.md) <br/> |<span data-ttu-id="d36b5-127">Представляет файл, подключенный к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="d36b5-127">Represents a file that is attached to an item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d36b5-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="d36b5-128">Remarks</span></span>

<span data-ttu-id="d36b5-129">Обратите внимание на то, что при создании вложения, изменить ключ корневого элемента изменяется важно.</span><span class="sxs-lookup"><span data-stu-id="d36b5-129">It is important to note that when an attachment is created, the change key of the root item is altered.</span></span>
  
<span data-ttu-id="d36b5-130">Элемент [идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) используется в DeleteAttachment и GetAttachment запросов.</span><span class="sxs-lookup"><span data-stu-id="d36b5-130">The [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md) element is used in DeleteAttachment and GetAttachment requests.</span></span> 
  
<span data-ttu-id="d36b5-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d36b5-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d36b5-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d36b5-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d36b5-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d36b5-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d36b5-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d36b5-134">Schema name</span></span>  <br/> |<span data-ttu-id="d36b5-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d36b5-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="d36b5-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d36b5-136">Validation file</span></span>  <br/> |<span data-ttu-id="d36b5-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d36b5-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d36b5-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d36b5-138">Can be empty</span></span>  <br/> |<span data-ttu-id="d36b5-139">False</span><span class="sxs-lookup"><span data-stu-id="d36b5-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d36b5-140">См. также</span><span class="sxs-lookup"><span data-stu-id="d36b5-140">See also</span></span>

- [<span data-ttu-id="d36b5-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d36b5-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

