---
title: олдпарентфолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldParentFolderId
api_type:
- schema
ms.assetid: da1b8c88-c650-455d-b749-0cd160b012d8
description: Элемент Олдпарентфолдерид содержит идентификатор родительской папки элемента или папки, которая была скопирована или перемещена.
ms.openlocfilehash: ad787e95f95b551393878b15783461d93ac08481
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467230"
---
# <a name="oldparentfolderid"></a><span data-ttu-id="243aa-103">олдпарентфолдерид</span><span class="sxs-lookup"><span data-stu-id="243aa-103">OldParentFolderId</span></span>

<span data-ttu-id="243aa-104">Элемент **олдпарентфолдерид** содержит идентификатор родительской папки элемента или папки, которая была скопирована или перемещена.</span><span class="sxs-lookup"><span data-stu-id="243aa-104">The **OldParentFolderId** element contains the identifier of the parent folder of an item or folder that was copied or moved.</span></span> 
  
```xml
<OldParentFolderId Id="" ChangeKey=""/>
```

 <span data-ttu-id="243aa-105">**фолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="243aa-105">**FolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="243aa-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="243aa-106">Attributes and elements</span></span>

<span data-ttu-id="243aa-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="243aa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="243aa-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="243aa-108">Attributes</span></span>

|<span data-ttu-id="243aa-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="243aa-109">**Attribute**</span></span>|<span data-ttu-id="243aa-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="243aa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="243aa-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="243aa-111">**Id**</span></span> <br/> |<span data-ttu-id="243aa-112">Содержит строку, определяющую папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="243aa-112">Contains a string that identifies a folder in the Exchange store.</span></span> <span data-ttu-id="243aa-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="243aa-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="243aa-114">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="243aa-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="243aa-115">Содержит строку, определяющую версию папки, определяемую атрибутом ID.</span><span class="sxs-lookup"><span data-stu-id="243aa-115">Contains a string that identifies a version of a folder that is identified by the Id attribute.</span></span> <span data-ttu-id="243aa-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="243aa-116">This attribute is optional.</span></span> <span data-ttu-id="243aa-117">Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.</span><span class="sxs-lookup"><span data-stu-id="243aa-117">Use this attribute to make sure that the correct version of a folder is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="243aa-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="243aa-118">Child elements</span></span>

<span data-ttu-id="243aa-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="243aa-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="243aa-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="243aa-120">Parent elements</span></span>

|<span data-ttu-id="243aa-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="243aa-121">**Element**</span></span>|<span data-ttu-id="243aa-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="243aa-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="243aa-123">копиедевент</span><span class="sxs-lookup"><span data-stu-id="243aa-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="243aa-124">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="243aa-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="243aa-125">моведевент</span><span class="sxs-lookup"><span data-stu-id="243aa-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="243aa-126">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="243aa-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="243aa-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="243aa-127">Remarks</span></span>

<span data-ttu-id="243aa-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="243aa-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="243aa-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="243aa-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="243aa-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="243aa-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="243aa-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="243aa-131">Schema Name</span></span>  <br/> |<span data-ttu-id="243aa-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="243aa-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="243aa-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="243aa-133">Validation File</span></span>  <br/> |<span data-ttu-id="243aa-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="243aa-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="243aa-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="243aa-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="243aa-136">False</span><span class="sxs-lookup"><span data-stu-id="243aa-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="243aa-137">См. также</span><span class="sxs-lookup"><span data-stu-id="243aa-137">See also</span></span>



[<span data-ttu-id="243aa-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="243aa-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="243aa-139">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="243aa-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="243aa-140">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="243aa-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="243aa-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="243aa-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

