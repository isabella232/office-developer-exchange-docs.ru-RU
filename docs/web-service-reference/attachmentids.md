---
title: аттачментидс
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
description: Элемент Аттачментидс содержит массив идентификаторов вложений.
ms.openlocfilehash: cff1cb5658690fd6dd2c6a7812e1f600a4c80e29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464254"
---
# <a name="attachmentids"></a><span data-ttu-id="152a3-103">аттачментидс</span><span class="sxs-lookup"><span data-stu-id="152a3-103">AttachmentIds</span></span>

<span data-ttu-id="152a3-104">Элемент **аттачментидс** содержит массив идентификаторов вложений.</span><span class="sxs-lookup"><span data-stu-id="152a3-104">The **AttachmentIds** element contains an array of attachment identifiers.</span></span> 
  
```xml
<AttachmentIds>
   <AttachmentId Id=""/>
</AttachmentIds>
```

 <span data-ttu-id="152a3-105">**нонемптяррайофрекуестаттачментидстипе**</span><span class="sxs-lookup"><span data-stu-id="152a3-105">**NonEmptyArrayOfRequestAttachmentIdsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="152a3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="152a3-106">Attributes and elements</span></span>

<span data-ttu-id="152a3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="152a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="152a3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="152a3-108">Attributes</span></span>

<span data-ttu-id="152a3-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="152a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="152a3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="152a3-110">Child elements</span></span>

|<span data-ttu-id="152a3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="152a3-111">**Element**</span></span>|<span data-ttu-id="152a3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="152a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="152a3-113">AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="152a3-113">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md) <br/> |<span data-ttu-id="152a3-114">Элемент, определяющий отдельное вложение.</span><span class="sxs-lookup"><span data-stu-id="152a3-114">The element that identifies a single attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="152a3-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="152a3-115">Parent elements</span></span>

|<span data-ttu-id="152a3-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="152a3-116">**Element**</span></span>|<span data-ttu-id="152a3-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="152a3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="152a3-118">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="152a3-118">DeleteAttachment</span></span>](deleteattachment.md) <br/> |<span data-ttu-id="152a3-119">Элемент, определяющий запрос на удаление вложения из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="152a3-119">The element that defines a request to delete an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="152a3-120">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="152a3-120">The following is the XPath expression to this element:</span></span>  <br/>  `/DeleteAttachment` <br/> |
|[<span data-ttu-id="152a3-121">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="152a3-121">GetAttachment</span></span>](getattachment.md) <br/> |<span data-ttu-id="152a3-122">Элемент, определяющий запрос на получение вложения из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="152a3-122">The element that defines a request to get an attachment from the Exchange store.</span></span>  <br/> <span data-ttu-id="152a3-123">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="152a3-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetAttachment` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="152a3-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="152a3-124">Remarks</span></span>

<span data-ttu-id="152a3-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="152a3-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="152a3-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="152a3-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="152a3-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="152a3-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="152a3-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="152a3-128">Schema Name</span></span>  <br/> |<span data-ttu-id="152a3-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="152a3-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="152a3-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="152a3-130">Validation File</span></span>  <br/> |<span data-ttu-id="152a3-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="152a3-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="152a3-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="152a3-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="152a3-133">False</span><span class="sxs-lookup"><span data-stu-id="152a3-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="152a3-134">См. также</span><span class="sxs-lookup"><span data-stu-id="152a3-134">See also</span></span>

- [<span data-ttu-id="152a3-135">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="152a3-135">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="152a3-136">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="152a3-136">GetAttachment operation</span></span>](getattachment-operation.md)

