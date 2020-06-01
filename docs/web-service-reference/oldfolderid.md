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
ms.openlocfilehash: a6713b9e0c47d68480724c3902086da6a8647dd7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458063"
---
# <a name="oldfolderid"></a><span data-ttu-id="cf7da-103">олдфолдерид</span><span class="sxs-lookup"><span data-stu-id="cf7da-103">OldFolderId</span></span>

<span data-ttu-id="cf7da-104">Элемент **олдфолдерид** содержит исходный идентификатор папки, которая была перемещена или скопирована.</span><span class="sxs-lookup"><span data-stu-id="cf7da-104">The **OldFolderId** element contains the original identifier of a folder that was moved or copied.</span></span> 
  
```xml
<OldFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="cf7da-105">**фолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="cf7da-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf7da-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cf7da-106">Attributes and elements</span></span>

<span data-ttu-id="cf7da-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cf7da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf7da-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cf7da-108">Attributes</span></span>

|<span data-ttu-id="cf7da-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="cf7da-109">**Attribute**</span></span>|<span data-ttu-id="cf7da-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf7da-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cf7da-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="cf7da-111">**Id**</span></span> <br/> |<span data-ttu-id="cf7da-112">Содержит строку, определяющую папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cf7da-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="cf7da-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="cf7da-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="cf7da-114">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="cf7da-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="cf7da-115">Содержит строку, определяющую версию папки, определяемую атрибутом ID.</span><span class="sxs-lookup"><span data-stu-id="cf7da-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="cf7da-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cf7da-116">This attribute is optional.</span></span> <span data-ttu-id="cf7da-117">Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.</span><span class="sxs-lookup"><span data-stu-id="cf7da-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cf7da-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cf7da-118">Child elements</span></span>

<span data-ttu-id="cf7da-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cf7da-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf7da-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cf7da-120">Parent elements</span></span>

|<span data-ttu-id="cf7da-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf7da-121">**Element**</span></span>|<span data-ttu-id="cf7da-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf7da-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf7da-123">копиедевент</span><span class="sxs-lookup"><span data-stu-id="cf7da-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="cf7da-124">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="cf7da-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="cf7da-125">моведевент</span><span class="sxs-lookup"><span data-stu-id="cf7da-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="cf7da-126">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="cf7da-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf7da-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="cf7da-127">Remarks</span></span>

<span data-ttu-id="cf7da-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cf7da-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf7da-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cf7da-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf7da-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cf7da-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf7da-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cf7da-131">Schema Name</span></span>  <br/> |<span data-ttu-id="cf7da-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cf7da-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf7da-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cf7da-133">Validation File</span></span>  <br/> |<span data-ttu-id="cf7da-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cf7da-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf7da-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cf7da-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="cf7da-136">False</span><span class="sxs-lookup"><span data-stu-id="cf7da-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf7da-137">См. также</span><span class="sxs-lookup"><span data-stu-id="cf7da-137">See also</span></span>



[<span data-ttu-id="cf7da-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="cf7da-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="cf7da-139">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="cf7da-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="cf7da-140">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="cf7da-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="cf7da-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cf7da-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

