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
description: Элемент GetAttachment является корневым элементом запроса для получения вложения из хранилища Exchange.
ms.openlocfilehash: d03d086ff443db87b0104a2ec83599eb9eaea6b9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463981"
---
# <a name="getattachment"></a><span data-ttu-id="4729e-103">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="4729e-103">GetAttachment</span></span>

<span data-ttu-id="4729e-104">Элемент **GetAttachment** является корневым элементом запроса для получения вложения из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="4729e-104">The **GetAttachment** element is the root element in a request to get an attachment from the Exchange store.</span></span> 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 <span data-ttu-id="4729e-105">**жетаттачменттипе**</span><span class="sxs-lookup"><span data-stu-id="4729e-105">**GetAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4729e-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4729e-106">Attributes and elements</span></span>

<span data-ttu-id="4729e-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4729e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4729e-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4729e-108">Attributes</span></span>

<span data-ttu-id="4729e-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4729e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4729e-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4729e-110">Child elements</span></span>

|<span data-ttu-id="4729e-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4729e-111">**Element**</span></span>|<span data-ttu-id="4729e-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4729e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4729e-113">аттачментшапе</span><span class="sxs-lookup"><span data-stu-id="4729e-113">AttachmentShape</span></span>](attachmentshape.md) <br/> |<span data-ttu-id="4729e-114">Определяет дополнительные свойства расширенного элемента, которые возвращаются в ответ на запрос [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="4729e-114">Identifies additional extended item properties to return in a response to a [GetAttachment](getattachment.md) request.</span></span> <span data-ttu-id="4729e-115">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="4729e-115">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="4729e-116">аттачментидс</span><span class="sxs-lookup"><span data-stu-id="4729e-116">AttachmentIds</span></span>](attachmentids.md) <br/> |<span data-ttu-id="4729e-117">Содержит массив идентификаторов вложений.</span><span class="sxs-lookup"><span data-stu-id="4729e-117">Contains an array of attachment identifiers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4729e-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4729e-118">Parent elements</span></span>

<span data-ttu-id="4729e-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="4729e-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4729e-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="4729e-120">Remarks</span></span>

<span data-ttu-id="4729e-121">Элемент [аттачментшапе](attachmentshape.md) не требуется для определения свойств, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="4729e-121">The [AttachmentShape](attachmentshape.md) element is not required to identify the properties returned in the response.</span></span> <span data-ttu-id="4729e-122">[Операция GetAttachment](getattachment-operation.md) возвращает имя, ContentType, ContentId, ContentLocation и свойства содержимого для вложенных файлов.</span><span class="sxs-lookup"><span data-stu-id="4729e-122">The [GetAttachment operation](getattachment-operation.md) returns the Name, ContentType, ContentId, ContentLocation, and the Content properties for file attachments.</span></span> <span data-ttu-id="4729e-123">Для вложений элемента возвращаемыми свойствами являются имя, ContentType, идентификатор ContentId, ContentLocation и все свойства вложенного элемента.</span><span class="sxs-lookup"><span data-stu-id="4729e-123">For item attachments, the returned properties are the Name, ContentType, ContentId, ContentLocation, and all the attached item's properties.</span></span> <span data-ttu-id="4729e-124">Это эквивалентно использованию базовой фигуры Аллпропертиес в запросе [GetItem](getitem.md) .</span><span class="sxs-lookup"><span data-stu-id="4729e-124">This is equivalent to using the AllProperties base shape in a [GetItem](getitem.md) request.</span></span> 
  
<span data-ttu-id="4729e-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4729e-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4729e-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4729e-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4729e-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4729e-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4729e-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4729e-128">Schema Name</span></span>  <br/> |<span data-ttu-id="4729e-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4729e-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4729e-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4729e-130">Validation File</span></span>  <br/> |<span data-ttu-id="4729e-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4729e-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4729e-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4729e-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="4729e-133">False</span><span class="sxs-lookup"><span data-stu-id="4729e-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4729e-134">См. также</span><span class="sxs-lookup"><span data-stu-id="4729e-134">See also</span></span>



[<span data-ttu-id="4729e-135">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="4729e-135">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="4729e-136">жетаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="4729e-136">GetAttachmentResponse</span></span>](getattachmentresponse.md)

