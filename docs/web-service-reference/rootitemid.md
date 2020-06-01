---
title: рутитемид
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
description: Элемент Рутитемид определяет корневой элемент удаленного вложения.
ms.openlocfilehash: d8badd465fd5a93e1a6354d55ac5c4b080897152
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457097"
---
# <a name="rootitemid"></a><span data-ttu-id="074b8-103">рутитемид</span><span class="sxs-lookup"><span data-stu-id="074b8-103">RootItemId</span></span>

<span data-ttu-id="074b8-104">Элемент **рутитемид** определяет корневой элемент удаленного вложения.</span><span class="sxs-lookup"><span data-stu-id="074b8-104">The **RootItemId** element identifies the root item of a deleted attachment.</span></span> 
  
[<span data-ttu-id="074b8-105">делетеаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="074b8-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
  
[<span data-ttu-id="074b8-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="074b8-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="074b8-107">делетеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="074b8-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
[<span data-ttu-id="074b8-108">рутитемид</span><span class="sxs-lookup"><span data-stu-id="074b8-108">RootItemId</span></span>](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 <span data-ttu-id="074b8-109">**рутитемидтипе**</span><span class="sxs-lookup"><span data-stu-id="074b8-109">**RootItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="074b8-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="074b8-110">Attributes and elements</span></span>

<span data-ttu-id="074b8-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="074b8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="074b8-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="074b8-112">Attributes</span></span>

|<span data-ttu-id="074b8-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="074b8-113">**Attribute**</span></span>|<span data-ttu-id="074b8-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="074b8-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="074b8-115">**рутитемид**</span><span class="sxs-lookup"><span data-stu-id="074b8-115">**RootItemId**</span></span> <br/> |<span data-ttu-id="074b8-116">Определяет корневой элемент удаленного вложения.</span><span class="sxs-lookup"><span data-stu-id="074b8-116">Identifies the root item of a deleted attachment.</span></span>  <br/> |
|<span data-ttu-id="074b8-117">**рутитемчанжекэй**</span><span class="sxs-lookup"><span data-stu-id="074b8-117">**RootItemChangeKey**</span></span> <br/> |<span data-ttu-id="074b8-118">Определяет новый ключ изменения корневого элемента удаленного вложения.</span><span class="sxs-lookup"><span data-stu-id="074b8-118">Identifies the new change key of the root item of a deleted attachment.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="074b8-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="074b8-119">Child elements</span></span>

<span data-ttu-id="074b8-120">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="074b8-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="074b8-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="074b8-121">Parent elements</span></span>

|<span data-ttu-id="074b8-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="074b8-122">**Element**</span></span>|<span data-ttu-id="074b8-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="074b8-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="074b8-124">делетеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="074b8-124">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md) <br/> |<span data-ttu-id="074b8-125">Содержит состояние и результат запроса DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="074b8-125">Contains the status and result of a DeleteAttachment request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="074b8-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="074b8-126">Remarks</span></span>

<span data-ttu-id="074b8-127">Элемент **рутитемид** используется только в ответах DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="074b8-127">The **RootItemId** element is only used in DeleteAttachment responses.</span></span> <span data-ttu-id="074b8-128">Это определяет идентификатор корневого элемента и, что более важно, новый ключ изменения для родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="074b8-128">This identifies the root item identifier, and more importantly, the new change key to the parent item.</span></span> 
  
<span data-ttu-id="074b8-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="074b8-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="074b8-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="074b8-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="074b8-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="074b8-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="074b8-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="074b8-132">Schema name</span></span>  <br/> |<span data-ttu-id="074b8-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="074b8-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="074b8-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="074b8-134">Validation file</span></span>  <br/> |<span data-ttu-id="074b8-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="074b8-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="074b8-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="074b8-136">Can be empty</span></span>  <br/> |<span data-ttu-id="074b8-137">False</span><span class="sxs-lookup"><span data-stu-id="074b8-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="074b8-138">См. также</span><span class="sxs-lookup"><span data-stu-id="074b8-138">See also</span></span>



[<span data-ttu-id="074b8-139">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="074b8-139">DeleteAttachment</span></span>](deleteattachment.md)
  
[<span data-ttu-id="074b8-140">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="074b8-140">DeleteAttachment operation</span></span>](deleteattachment-operation.md)


- [<span data-ttu-id="074b8-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="074b8-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

