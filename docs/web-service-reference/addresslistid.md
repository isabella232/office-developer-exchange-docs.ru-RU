---
title: аддресслистид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a3334bb2-90dc-4fe1-96d9-890b13d9ff30
description: Элемент Аддресслистид указывает идентификатор списка адресов.
ms.openlocfilehash: d8a513559b7d127559537b43d7c6c0a4db121702
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761359"
---
# <a name="addresslistid"></a><span data-ttu-id="b1ab3-103">аддресслистид</span><span class="sxs-lookup"><span data-stu-id="b1ab3-103">AddressListId</span></span>

<span data-ttu-id="b1ab3-104">Элемент **аддресслистид** указывает идентификатор списка адресов.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-104">The **AddressListId** element specifies the identifier of an address list.</span></span> 
  
```XML
<AddressListId Id="">
</AddressListId>
```

 <span data-ttu-id="b1ab3-105">**аддресслистидтипе**</span><span class="sxs-lookup"><span data-stu-id="b1ab3-105">**AddressListIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b1ab3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b1ab3-106">Attributes and elements</span></span>

<span data-ttu-id="b1ab3-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b1ab3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b1ab3-108">Attributes</span></span>

|<span data-ttu-id="b1ab3-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b1ab3-109">**Attribute**</span></span>|<span data-ttu-id="b1ab3-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b1ab3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b1ab3-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="b1ab3-111">**Id**</span></span> <br/> |<span data-ttu-id="b1ab3-112">Идентификатор списка адресов строкового типа.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-112">A string address list identifier.</span></span> <span data-ttu-id="b1ab3-113">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-113">This attribute is required.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b1ab3-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b1ab3-114">Child elements</span></span>

<span data-ttu-id="b1ab3-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b1ab3-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b1ab3-116">Parent elements</span></span>

|<span data-ttu-id="b1ab3-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b1ab3-117">**Element**</span></span>|<span data-ttu-id="b1ab3-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b1ab3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b1ab3-119">контекстфолдерид</span><span class="sxs-lookup"><span data-stu-id="b1ab3-119">ContextFolderId</span></span>](contextfolderid.md) <br/> |<span data-ttu-id="b1ab3-120">Указывает папку, предназначенную для действий, в которых используются папки.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-120">Indicates the folder that is targeted for actions that use folders.</span></span> <span data-ttu-id="b1ab3-121">Этот элемент должен присутствовать при копировании, удалении, перемещении и установке состояния чтения элементов беседы в целевой папке.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-121">This element must be present when copying, deleting, moving, and setting read state on conversation items in a target folder.</span></span>  <br/> |
|[<span data-ttu-id="b1ab3-122">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="b1ab3-122">CopyToFolder</span></span>](copytofolder.md) <br/> |<span data-ttu-id="b1ab3-123">Задает идентификатор папки, в которую будут скопированы элементы электронной почты.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-123">Specifies the identifier of the folder to which email items are copied.</span></span>  <br/> |
|[<span data-ttu-id="b1ab3-124">дестинатионфолдерид</span><span class="sxs-lookup"><span data-stu-id="b1ab3-124">DestinationFolderId</span></span>](destinationfolderid.md) <br/> |<span data-ttu-id="b1ab3-125">Указывает целевую папку для действий по копированию и перемещению.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-125">Indicates the destination folder for copy and move actions.</span></span>  <br/> |
|[<span data-ttu-id="b1ab3-126">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="b1ab3-126">MoveToFolder</span></span>](movetofolder.md) <br/> |<span data-ttu-id="b1ab3-127">Указывает идентификатор папки, в которую будут перемещены элементы электронной почты</span><span class="sxs-lookup"><span data-stu-id="b1ab3-127">Specifies the identifier of the folder to which email items are moved</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b1ab3-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="b1ab3-128">Remarks</span></span>

<span data-ttu-id="b1ab3-129">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b1ab3-130">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b1ab3-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b1ab3-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b1ab3-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b1ab3-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b1ab3-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b1ab3-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b1ab3-133">Schema Name</span></span>  <br/> |<span data-ttu-id="b1ab3-134">Схема типа</span><span class="sxs-lookup"><span data-stu-id="b1ab3-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="b1ab3-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b1ab3-135">Validation File</span></span>  <br/> |<span data-ttu-id="b1ab3-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b1ab3-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b1ab3-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b1ab3-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b1ab3-138">См. также</span><span class="sxs-lookup"><span data-stu-id="b1ab3-138">See also</span></span>

- [<span data-ttu-id="b1ab3-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b1ab3-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

