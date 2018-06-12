---
title: AddressListId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: Элемент AddressListId указывает идентификатор элемента списка адресов.
ms.openlocfilehash: d8a513559b7d127559537b43d7c6c0a4db121702
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761359"
---
# <a name="addresslistid"></a><span data-ttu-id="427ce-103">AddressListId</span><span class="sxs-lookup"><span data-stu-id="427ce-103">AddressListId</span></span>

<span data-ttu-id="427ce-104">Элемент **AddressListId** указывает идентификатор элемента списка адресов.</span><span class="sxs-lookup"><span data-stu-id="427ce-104">The **AddressListId** element specifies the identifier of an address list.</span></span> 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 <span data-ttu-id="427ce-105">**AddressListIdType**</span><span class="sxs-lookup"><span data-stu-id="427ce-105">**AddressListIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="427ce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="427ce-106">Attributes and elements</span></span>

<span data-ttu-id="427ce-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="427ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="427ce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="427ce-108">Attributes</span></span>

|<span data-ttu-id="427ce-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="427ce-109">**Attribute**</span></span>|<span data-ttu-id="427ce-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="427ce-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="427ce-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="427ce-111">**Id**</span></span> <br/> |<span data-ttu-id="427ce-112">Строковый идентификатор списка адресов.</span><span class="sxs-lookup"><span data-stu-id="427ce-112">A string address list identifier.</span></span> <span data-ttu-id="427ce-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="427ce-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="427ce-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="427ce-114">Child elements</span></span>

<span data-ttu-id="427ce-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="427ce-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="427ce-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="427ce-116">Parent elements</span></span>

|<span data-ttu-id="427ce-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="427ce-117">**Element**</span></span>|<span data-ttu-id="427ce-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="427ce-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="427ce-119">ContextFolderId</span><span class="sxs-lookup"><span data-stu-id="427ce-119">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="427ce-120">Указывает папку, предназначенное для действий, использующих папок.</span><span class="sxs-lookup"><span data-stu-id="427ce-120">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="427ce-121">Этот элемент должен присутствовать при копирование, удаление, перемещение и настройка состояние чтения элементов беседы в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="427ce-121">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="427ce-122">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="427ce-122">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="427ce-123">Задает идентификатор папки, в который копируются элементы электронной почты.</span><span class="sxs-lookup"><span data-stu-id="427ce-123">Specifies the identifier of the folder to which email items are copied.</span></span>  <br/> |
|[<span data-ttu-id="427ce-124">DestinationFolderId</span><span class="sxs-lookup"><span data-stu-id="427ce-124">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="427ce-125">Определяет папку назначения для копирования и перемещения действия.</span><span class="sxs-lookup"><span data-stu-id="427ce-125">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="427ce-126">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="427ce-126">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="427ce-127">Указывает идентификатор папки, на который перемещаются элементов электронной почты</span><span class="sxs-lookup"><span data-stu-id="427ce-127">Specifies the identifier of the folder to which email items are moved</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="427ce-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="427ce-128">Remarks</span></span>

<span data-ttu-id="427ce-129">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="427ce-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="427ce-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="427ce-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="427ce-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="427ce-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="427ce-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="427ce-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="427ce-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="427ce-133">Schema Name</span></span>  <br/> |<span data-ttu-id="427ce-134">Схема типа</span><span class="sxs-lookup"><span data-stu-id="427ce-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="427ce-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="427ce-135">Validation File</span></span>  <br/> |<span data-ttu-id="427ce-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="427ce-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="427ce-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="427ce-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="427ce-138">См. также</span><span class="sxs-lookup"><span data-stu-id="427ce-138">See also</span></span>

- [<span data-ttu-id="427ce-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="427ce-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

