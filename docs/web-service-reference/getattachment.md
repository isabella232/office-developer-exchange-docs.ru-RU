---
title: GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: Элемент GetAttachment является корневым элементом в запросе для получения вложения из хранилища Exchange.
ms.openlocfilehash: fb639c86a0654e8f9e9601310f7c2f5b0fc7d729
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762698"
---
# <a name="getattachment"></a><span data-ttu-id="81d32-103">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="81d32-103">GetAttachment</span></span>

<span data-ttu-id="81d32-104">Элемент **GetAttachment** является корневым элементом в запросе для получения вложения из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="81d32-104">The **GetAttachment** element is the root element in a request to get an attachment from the Exchange store.</span></span> 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 <span data-ttu-id="81d32-105">**GetAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="81d32-105">**GetAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81d32-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="81d32-106">Attributes and elements</span></span>

<span data-ttu-id="81d32-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="81d32-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81d32-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="81d32-108">Attributes</span></span>

<span data-ttu-id="81d32-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="81d32-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81d32-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="81d32-110">Child elements</span></span>

|<span data-ttu-id="81d32-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81d32-111">**Element**</span></span>|<span data-ttu-id="81d32-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81d32-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81d32-113">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="81d32-113">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="81d32-114">Определяет дополнительные расширенные свойства элемента для возврата в ответ на запрос [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="81d32-114">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> <span data-ttu-id="81d32-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="81d32-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="81d32-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="81d32-116">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="81d32-117">Содержит массив идентификаторов вложения.</span><span class="sxs-lookup"><span data-stu-id="81d32-117">Contains an array of attachment identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81d32-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="81d32-118">Parent elements</span></span>

<span data-ttu-id="81d32-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="81d32-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="81d32-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="81d32-120">Remarks</span></span>

<span data-ttu-id="81d32-121">Элемент [AttachmentShape](attachmentshape.md) не требуется для идентификации свойства, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="81d32-121">The [AttachmentShape](attachmentshape.md) element is not required to identify the properties returned in the response.</span></span> <span data-ttu-id="81d32-122">[Операция GetAttachment](getattachment-operation.md) возвращает имя, ContentType, ContentId, ContentLocation и свойства содержимого для вложенных файлов.</span><span class="sxs-lookup"><span data-stu-id="81d32-122">The [GetAttachment operation](getattachment-operation.md) returns the Name, ContentType, ContentId, ContentLocation, and the Content properties for file attachments.</span></span> <span data-ttu-id="81d32-123">Для вложений элемента возвращаемого свойства — это имя, ContentType, ContentId, ContentLocation и все вложенные свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="81d32-123">For item attachments, the returned properties are the Name, ContentType, ContentId, ContentLocation, and all the attached item's properties.</span></span> <span data-ttu-id="81d32-124">Это эквивалентно использованию фигуры базовый AllProperties в запросе [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="81d32-124">This is equivalent to using the AllProperties base shape in a [GetItem](getitem.md) request.</span></span> 
  
<span data-ttu-id="81d32-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="81d32-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81d32-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="81d32-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81d32-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="81d32-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="81d32-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="81d32-128">Schema Name</span></span>  <br/> |<span data-ttu-id="81d32-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="81d32-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="81d32-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="81d32-130">Validation File</span></span>  <br/> |<span data-ttu-id="81d32-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="81d32-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="81d32-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="81d32-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="81d32-133">False</span><span class="sxs-lookup"><span data-stu-id="81d32-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81d32-134">См. также</span><span class="sxs-lookup"><span data-stu-id="81d32-134">See also</span></span>



[<span data-ttu-id="81d32-135">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="81d32-135">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="81d32-136">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="81d32-136">GetAttachmentResponse</span></span>](getattachmentresponse.md)

