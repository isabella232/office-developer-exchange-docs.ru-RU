---
title: олдфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldFolderId
api_type:
- schema
ms.assetid: da554a97-ab87-4950-9fc4-26b1972381bb
description: Элемент Олдфолдерид содержит исходный идентификатор папки, которая была перемещена или скопирована.
ms.openlocfilehash: ef73cad73213a1e8b5341907cd22177d8e1ba628
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834645"
---
# <a name="oldfolderid"></a><span data-ttu-id="cd3a5-103">олдфолдерид</span><span class="sxs-lookup"><span data-stu-id="cd3a5-103">OldFolderId</span></span>

<span data-ttu-id="cd3a5-104">Элемент **олдфолдерид** содержит исходный идентификатор папки, которая была перемещена или скопирована.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-104">The **OldFolderId** element contains the original identifier of a folder that was moved or copied.</span></span> 
  
```xml
<OldFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="cd3a5-105">**фолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="cd3a5-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cd3a5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cd3a5-106">Attributes and elements</span></span>

<span data-ttu-id="cd3a5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd3a5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cd3a5-108">Attributes</span></span>

|<span data-ttu-id="cd3a5-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="cd3a5-109">**Attribute**</span></span>|<span data-ttu-id="cd3a5-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd3a5-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cd3a5-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="cd3a5-111">**Id**</span></span> <br/> |<span data-ttu-id="cd3a5-112">Содержит строку, определяющую папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="cd3a5-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="cd3a5-114">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="cd3a5-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="cd3a5-115">Содержит строку, определяющую версию папки, определяемую атрибутом ID.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="cd3a5-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-116">This attribute is optional.</span></span> <span data-ttu-id="cd3a5-117">Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cd3a5-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cd3a5-118">Child elements</span></span>

<span data-ttu-id="cd3a5-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cd3a5-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cd3a5-120">Parent elements</span></span>

|<span data-ttu-id="cd3a5-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd3a5-121">**Element**</span></span>|<span data-ttu-id="cd3a5-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd3a5-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd3a5-123">копиедевент</span><span class="sxs-lookup"><span data-stu-id="cd3a5-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="cd3a5-124">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="cd3a5-125">моведевент</span><span class="sxs-lookup"><span data-stu-id="cd3a5-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="cd3a5-126">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cd3a5-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="cd3a5-127">Remarks</span></span>

<span data-ttu-id="cd3a5-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cd3a5-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cd3a5-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cd3a5-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cd3a5-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cd3a5-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cd3a5-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cd3a5-131">Schema Name</span></span>  <br/> |<span data-ttu-id="cd3a5-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cd3a5-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="cd3a5-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cd3a5-133">Validation File</span></span>  <br/> |<span data-ttu-id="cd3a5-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cd3a5-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cd3a5-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cd3a5-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="cd3a5-136">False</span><span class="sxs-lookup"><span data-stu-id="cd3a5-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cd3a5-137">См. также</span><span class="sxs-lookup"><span data-stu-id="cd3a5-137">See also</span></span>



[<span data-ttu-id="cd3a5-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="cd3a5-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="cd3a5-139">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="cd3a5-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="cd3a5-140">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="cd3a5-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="cd3a5-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cd3a5-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

