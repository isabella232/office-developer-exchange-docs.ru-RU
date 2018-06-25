---
title: AttachmentIds
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentIds
api_type:
- schema
ms.assetid: 46ce3ad7-4b20-43ae-8c63-39f1e3c2666b
description: Элемент AttachmentIds содержит массив идентификаторов вложения.
ms.openlocfilehash: f205aefe6a7dc4ec208e8a96b8a6b47094aa741b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761512"
---
# <a name="attachmentids"></a><span data-ttu-id="1b6cc-103">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="1b6cc-103">AttachmentIds</span></span>

<span data-ttu-id="1b6cc-104">Элемент **AttachmentIds** содержит массив идентификаторов вложения.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-104">The **AttachmentIds** element contains an array of attachment identifiers.</span></span> 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 <span data-ttu-id="1b6cc-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span><span class="sxs-lookup"><span data-stu-id="1b6cc-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b6cc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1b6cc-106">Attributes and elements</span></span>

<span data-ttu-id="1b6cc-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b6cc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1b6cc-108">Attributes</span></span>

<span data-ttu-id="1b6cc-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b6cc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1b6cc-110">Child elements</span></span>

|<span data-ttu-id="1b6cc-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b6cc-111">**Element**</span></span>|<span data-ttu-id="1b6cc-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b6cc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b6cc-113">Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="1b6cc-113">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md) <br/> |<span data-ttu-id="1b6cc-114">Элемент, который определяет одного вложения.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-114">The element that identifies a single attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b6cc-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1b6cc-115">Parent elements</span></span>

|<span data-ttu-id="1b6cc-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b6cc-116">**Element**</span></span>|<span data-ttu-id="1b6cc-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b6cc-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b6cc-118">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="1b6cc-118">DeleteAttachment</span></span>](deleteattachment.md) <br/> |<span data-ttu-id="1b6cc-119">Элемент, который определяет запрос для удаления вложения из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-119">The element that defines a request to delete an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="1b6cc-120">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-120">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteAttachment` <br/> |
|[<span data-ttu-id="1b6cc-121">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="1b6cc-121">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="1b6cc-122">Элемент, который определяет запрос для получения вложения из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-122">The element that defines a request to get an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="1b6cc-123">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1b6cc-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="1b6cc-124">Remarks</span></span>

<span data-ttu-id="1b6cc-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1b6cc-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b6cc-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1b6cc-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b6cc-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1b6cc-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b6cc-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1b6cc-128">Schema Name</span></span>  <br/> |<span data-ttu-id="1b6cc-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1b6cc-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b6cc-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1b6cc-130">Validation File</span></span>  <br/> |<span data-ttu-id="1b6cc-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b6cc-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b6cc-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1b6cc-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b6cc-133">False</span><span class="sxs-lookup"><span data-stu-id="1b6cc-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b6cc-134">См. также</span><span class="sxs-lookup"><span data-stu-id="1b6cc-134">See also</span></span>

- [<span data-ttu-id="1b6cc-135">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="1b6cc-135">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="1b6cc-136">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="1b6cc-136">GetAttachment operation</span></span>](getattachment-operation.md)

