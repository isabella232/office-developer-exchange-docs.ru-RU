---
title: Удаление
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- schema
ms.assetid: aa45f0c1-a80d-4b6c-8a85-375b6de515f4
description: Элемент Delete указывает, может ли клиент удалить папку или элемент.
ms.openlocfilehash: 5460f9e49b126ca6b039c6f11aaa3c6eb4a40544
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457356"
---
# <a name="delete"></a><span data-ttu-id="2ee79-103">Удаление</span><span class="sxs-lookup"><span data-stu-id="2ee79-103">Delete</span></span>

<span data-ttu-id="2ee79-104">Элемент **Delete** указывает, может ли клиент удалить папку или элемент.</span><span class="sxs-lookup"><span data-stu-id="2ee79-104">The **Delete** element indicates whether a client can delete a folder or item.</span></span> 
  
```XML
<Delete>true or false</Delete>
```

<span data-ttu-id="2ee79-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="2ee79-105">**boolean**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2ee79-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2ee79-106">Attributes and elements</span></span>

<span data-ttu-id="2ee79-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2ee79-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ee79-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2ee79-108">Attributes</span></span>

<span data-ttu-id="2ee79-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2ee79-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ee79-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2ee79-110">Child elements</span></span>

<span data-ttu-id="2ee79-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="2ee79-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ee79-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2ee79-112">Parent elements</span></span>

|<span data-ttu-id="2ee79-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2ee79-113">**Element**</span></span>|<span data-ttu-id="2ee79-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2ee79-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ee79-115">еффективеригхтс</span><span class="sxs-lookup"><span data-stu-id="2ee79-115">EffectiveRights</span></span>](effectiverights.md) <br/> |<span data-ttu-id="2ee79-116">Содержит права клиента на основе параметров разрешений для элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="2ee79-116">Contains the rights of the client based on the permission settings for the item or folder.</span></span>  <br/> |
|[<span data-ttu-id="2ee79-117">Действия</span><span class="sxs-lookup"><span data-stu-id="2ee79-117">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="2ee79-118">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="2ee79-118">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ee79-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2ee79-119">Text value</span></span>

<span data-ttu-id="2ee79-120">Текстовое значение **true** указывает, что клиент может удалить элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="2ee79-120">A text value of **true** indicates that a client can delete an item or folder.</span></span> <span data-ttu-id="2ee79-121">Значение **false** указывает, что клиент не может удалить элемент или папку.</span><span class="sxs-lookup"><span data-stu-id="2ee79-121">A value of **false** indicates that a client cannot delete an item or folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2ee79-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="2ee79-122">Remarks</span></span>

<span data-ttu-id="2ee79-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2ee79-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ee79-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2ee79-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ee79-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2ee79-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ee79-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2ee79-126">Schema Name</span></span>  <br/> |<span data-ttu-id="2ee79-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2ee79-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="2ee79-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2ee79-128">Validation File</span></span>  <br/> |<span data-ttu-id="2ee79-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2ee79-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ee79-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2ee79-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="2ee79-131">False</span><span class="sxs-lookup"><span data-stu-id="2ee79-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2ee79-132">См. также</span><span class="sxs-lookup"><span data-stu-id="2ee79-132">See also</span></span>

- [<span data-ttu-id="2ee79-133">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2ee79-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="2ee79-134">Setting Folder-Level Permissions</span><span class="sxs-lookup"><span data-stu-id="2ee79-134">Setting Folder-Level Permissions</span></span>](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

