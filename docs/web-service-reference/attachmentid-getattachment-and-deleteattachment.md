---
title: AttachmentId (GetAttachment и DeleteAttachment)
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
ms.assetid: 4bea1cb5-0a0f-4e14-9b09-f91af8cf9899
description: Элемент AttachmentId определяет одно вложение.
ms.openlocfilehash: 1096487490f6066f70d2da861b3015f0fbf5a68f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460857"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a><span data-ttu-id="fc527-103">AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="fc527-103">AttachmentId (GetAttachment and DeleteAttachment)</span></span>

<span data-ttu-id="fc527-104">Элемент **AttachmentId** определяет одно вложение.</span><span class="sxs-lookup"><span data-stu-id="fc527-104">The **AttachmentId** element identifies a single attachment.</span></span> 
  
```xml
<AttachmentId Id="" />
```

 <span data-ttu-id="fc527-105">**рекуестаттачментидтипе**</span><span class="sxs-lookup"><span data-stu-id="fc527-105">**RequestAttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fc527-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fc527-106">Attributes and elements</span></span>

<span data-ttu-id="fc527-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fc527-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc527-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fc527-108">Attributes</span></span>

|<span data-ttu-id="fc527-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="fc527-109">**Attribute**</span></span>|<span data-ttu-id="fc527-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc527-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fc527-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="fc527-111">**Id**</span></span> <br/> |<span data-ttu-id="fc527-112">Указывает идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="fc527-112">Specifies the attachment identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fc527-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fc527-113">Child elements</span></span>

<span data-ttu-id="fc527-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fc527-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fc527-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fc527-115">Parent elements</span></span>

|<span data-ttu-id="fc527-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc527-116">**Element**</span></span>|<span data-ttu-id="fc527-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc527-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc527-118">аттачментидс</span><span class="sxs-lookup"><span data-stu-id="fc527-118">AttachmentIds</span></span>](attachmentids.md) <br/> | <span data-ttu-id="fc527-119">Содержит массив идентификаторов вложений.</span><span class="sxs-lookup"><span data-stu-id="fc527-119">Contains an array of attachment identifiers.</span></span><br/><br/>  <span data-ttu-id="fc527-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="fc527-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fc527-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="fc527-121">Remarks</span></span>

<span data-ttu-id="fc527-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fc527-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fc527-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fc527-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fc527-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fc527-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fc527-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fc527-125">Schema Name</span></span>  <br/> |<span data-ttu-id="fc527-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fc527-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="fc527-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fc527-127">Validation File</span></span>  <br/> |<span data-ttu-id="fc527-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fc527-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fc527-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fc527-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="fc527-130">False</span><span class="sxs-lookup"><span data-stu-id="fc527-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc527-131">См. также</span><span class="sxs-lookup"><span data-stu-id="fc527-131">See also</span></span>

- [<span data-ttu-id="fc527-132">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="fc527-132">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="fc527-133">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="fc527-133">GetAttachment operation</span></span>](getattachment-operation.md)

