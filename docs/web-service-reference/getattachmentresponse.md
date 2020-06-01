---
title: жетаттачментреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachmentResponse
api_type:
- schema
ms.assetid: cb65f449-309b-4b6e-8d22-d1967135490c
description: Элемент Жетаттачментреспонсе определяет ответ на запрос GetAttachment.
ms.openlocfilehash: f0daf778f1248eabc5d51ee6155c460d9248549f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461256"
---
# <a name="getattachmentresponse"></a><span data-ttu-id="55840-103">жетаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="55840-103">GetAttachmentResponse</span></span>

<span data-ttu-id="55840-104">Элемент **жетаттачментреспонсе** определяет ответ на запрос GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="55840-104">The **GetAttachmentResponse** element defines a response to a GetAttachment request.</span></span> 
  
```xml
<GetAttachmentResponse>
   <ResponseMessages/>
</GetAttachmentResponse>
```

 <span data-ttu-id="55840-105">**жетаттачментреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="55840-105">**GetAttachmentResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55840-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="55840-106">Attributes and elements</span></span>

<span data-ttu-id="55840-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="55840-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55840-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="55840-108">Attributes</span></span>

<span data-ttu-id="55840-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="55840-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55840-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="55840-110">Child elements</span></span>

|<span data-ttu-id="55840-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="55840-111">**Element**</span></span>|<span data-ttu-id="55840-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="55840-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55840-113">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="55840-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="55840-114">Содержит ответные сообщения для запроса веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="55840-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55840-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="55840-115">Parent elements</span></span>

<span data-ttu-id="55840-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="55840-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55840-117">Примечания</span><span class="sxs-lookup"><span data-stu-id="55840-117">Remarks</span></span>

<span data-ttu-id="55840-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="55840-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55840-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="55840-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55840-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="55840-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="55840-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="55840-121">Schema name</span></span>  <br/> |<span data-ttu-id="55840-122">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="55840-122">Messages schema</span></span>  <br/> |
|<span data-ttu-id="55840-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="55840-123">Validation file</span></span>  <br/> |<span data-ttu-id="55840-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="55840-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="55840-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="55840-125">Can be empty</span></span>  <br/> |<span data-ttu-id="55840-126">False</span><span class="sxs-lookup"><span data-stu-id="55840-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55840-127">См. также</span><span class="sxs-lookup"><span data-stu-id="55840-127">See also</span></span>



[<span data-ttu-id="55840-128">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="55840-128">GetAttachment operation</span></span>](getattachment-operation.md)
  
[<span data-ttu-id="55840-129">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="55840-129">GetAttachment</span></span>](getattachment.md)

