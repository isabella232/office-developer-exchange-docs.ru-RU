---
title: олдитемид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OldItemId
api_type:
- schema
ms.assetid: fb57deee-9cc3-4730-9805-ff34f39e3ab7
description: Элемент Олдитемид содержит уникальный идентификатор скопированного или перемещенного элемента.
ms.openlocfilehash: ced7fc6891e0d1fde42a8cb9cad4f4e55493b5d1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834648"
---
# <a name="olditemid"></a><span data-ttu-id="7c654-103">олдитемид</span><span class="sxs-lookup"><span data-stu-id="7c654-103">OldItemId</span></span>

<span data-ttu-id="7c654-104">Элемент **олдитемид** содержит уникальный идентификатор скопированного или перемещенного элемента.</span><span class="sxs-lookup"><span data-stu-id="7c654-104">The **OldItemId** element contains the unique identifier of the item that was copied or moved.</span></span> 
  
```xml
<OldItemId Id="" ChangeKey=""/>
```

 <span data-ttu-id="7c654-105">**итемидтипе**</span><span class="sxs-lookup"><span data-stu-id="7c654-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c654-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7c654-106">Attributes and elements</span></span>

<span data-ttu-id="7c654-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7c654-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c654-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7c654-108">Attributes</span></span>

|<span data-ttu-id="7c654-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="7c654-109">**Attribute**</span></span>|<span data-ttu-id="7c654-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c654-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7c654-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="7c654-111">**Id**</span></span> <br/> |<span data-ttu-id="7c654-112">Содержит строку, определяющую элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7c654-112">Contains a string that identifies an item in the Exchange store.</span></span> <span data-ttu-id="7c654-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="7c654-113">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="7c654-114">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="7c654-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="7c654-115">Содержит строку, определяющую версию элемента, определяемого атрибутом ID.</span><span class="sxs-lookup"><span data-stu-id="7c654-115">Contains a string that identifies a version of an item that is identified by the Id attribute.</span></span> <span data-ttu-id="7c654-116">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="7c654-116">This attribute is optional.</span></span> <span data-ttu-id="7c654-117">Используйте этот атрибут, чтобы убедиться, что используется правильная версия элемента.</span><span class="sxs-lookup"><span data-stu-id="7c654-117">Use this attribute to make sure that the correct version of an item is used.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7c654-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7c654-118">Child elements</span></span>

<span data-ttu-id="7c654-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="7c654-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7c654-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7c654-120">Parent elements</span></span>

|<span data-ttu-id="7c654-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c654-121">**Element**</span></span>|<span data-ttu-id="7c654-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c654-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c654-123">копиедевент</span><span class="sxs-lookup"><span data-stu-id="7c654-123">CopiedEvent</span></span>](copiedevent.md) <br/> |<span data-ttu-id="7c654-124">Представляет событие, в котором копируется элемент или папка.</span><span class="sxs-lookup"><span data-stu-id="7c654-124">Represents an event in which an item or folder is copied.</span></span>  <br/> |
|[<span data-ttu-id="7c654-125">моведевент</span><span class="sxs-lookup"><span data-stu-id="7c654-125">MovedEvent</span></span>](movedevent.md) <br/> |<span data-ttu-id="7c654-126">Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.</span><span class="sxs-lookup"><span data-stu-id="7c654-126">Represents an event in which an item or folder is moved from one parent folder to another parent folder.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c654-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="7c654-127">Remarks</span></span>

<span data-ttu-id="7c654-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7c654-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c654-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7c654-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c654-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7c654-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c654-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7c654-131">Schema Name</span></span>  <br/> |<span data-ttu-id="7c654-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7c654-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c654-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7c654-133">Validation File</span></span>  <br/> |<span data-ttu-id="7c654-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7c654-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c654-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7c654-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c654-136">False</span><span class="sxs-lookup"><span data-stu-id="7c654-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c654-137">См. также</span><span class="sxs-lookup"><span data-stu-id="7c654-137">See also</span></span>



[<span data-ttu-id="7c654-138">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="7c654-138">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="7c654-139">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="7c654-139">GetEvents operation</span></span>](getevents-operation.md)
  
[<span data-ttu-id="7c654-140">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="7c654-140">Unsubscribe operation</span></span>](unsubscribe-operation.md)


- [<span data-ttu-id="7c654-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7c654-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

