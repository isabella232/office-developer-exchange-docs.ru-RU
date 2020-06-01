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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460857"
---
# <a name="attachmentid-getattachment-and-deleteattachment"></a><span data-ttu-id="61e66-103">AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="61e66-103">AttachmentId (GetAttachment and DeleteAttachment)</span></span>

<span data-ttu-id="61e66-104">Элемент **AttachmentId** определяет одно вложение.</span><span class="sxs-lookup"><span data-stu-id="61e66-104">The **AttachmentId** element identifies a single attachment.</span></span> 
  
```xml
<AttachmentId Id="" />
```

 <span data-ttu-id="61e66-105">**рекуестаттачментидтипе**</span><span class="sxs-lookup"><span data-stu-id="61e66-105">**RequestAttachmentIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="61e66-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="61e66-106">Attributes and elements</span></span>

<span data-ttu-id="61e66-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="61e66-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="61e66-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="61e66-108">Attributes</span></span>

|<span data-ttu-id="61e66-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="61e66-109">**Attribute**</span></span>|<span data-ttu-id="61e66-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="61e66-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="61e66-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="61e66-111">**Id**</span></span> <br/> |<span data-ttu-id="61e66-112">Указывает идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="61e66-112">Specifies the attachment identifier.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="61e66-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="61e66-113">Child elements</span></span>

<span data-ttu-id="61e66-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="61e66-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="61e66-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="61e66-115">Parent elements</span></span>

|<span data-ttu-id="61e66-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="61e66-116">**Element**</span></span>|<span data-ttu-id="61e66-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="61e66-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="61e66-118">аттачментидс</span><span class="sxs-lookup"><span data-stu-id="61e66-118">AttachmentIds</span></span>](attachmentids.md) <br/> | <span data-ttu-id="61e66-119">Содержит массив идентификаторов вложений.</span><span class="sxs-lookup"><span data-stu-id="61e66-119">Contains an array of attachment identifiers.</span></span><br/><br/>  <span data-ttu-id="61e66-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="61e66-120">The following are the XPath expressions to this element:</span></span><br/><br/>`/DeleteAttachment/AttachmentIds`<br/><br/>`/GetAttachment/AttachmentIds` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="61e66-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="61e66-121">Remarks</span></span>

<span data-ttu-id="61e66-122">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="61e66-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="61e66-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="61e66-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="61e66-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="61e66-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="61e66-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="61e66-125">Schema Name</span></span>  <br/> |<span data-ttu-id="61e66-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="61e66-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="61e66-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="61e66-127">Validation File</span></span>  <br/> |<span data-ttu-id="61e66-128">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="61e66-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="61e66-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="61e66-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="61e66-130">False</span><span class="sxs-lookup"><span data-stu-id="61e66-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="61e66-131">См. также</span><span class="sxs-lookup"><span data-stu-id="61e66-131">See also</span></span>

- [<span data-ttu-id="61e66-132">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="61e66-132">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="61e66-133">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="61e66-133">GetAttachment operation</span></span>](getattachment-operation.md)

