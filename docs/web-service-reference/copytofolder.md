---
title: CopyToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyToFolder
api_type:
- schema
ms.assetid: 6fd8a6b8-d813-43ff-991b-0e9e782fe00e
description: Элемент CopyToFolder указывает идентификатор папки, в которую можно копировать элементы электронной почты.
ms.openlocfilehash: 7cdda0f9769f909255c9b76f78ac7094a8dfc8f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463176"
---
# <a name="copytofolder"></a><span data-ttu-id="97808-103">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="97808-103">CopyToFolder</span></span>

<span data-ttu-id="97808-104">Элемент **CopyToFolder** указывает идентификатор папки, в которую можно копировать элементы электронной почты.</span><span class="sxs-lookup"><span data-stu-id="97808-104">The **CopyToFolder** element specifies the identifier of the folder that email items can be copied to.</span></span> 
  
```XML
<CopyToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</CopyToFolder>
```

 <span data-ttu-id="97808-105">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="97808-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="97808-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="97808-106">Attributes and elements</span></span>

<span data-ttu-id="97808-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="97808-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="97808-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="97808-108">Attributes</span></span>

<span data-ttu-id="97808-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="97808-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="97808-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="97808-110">Child elements</span></span>

|<span data-ttu-id="97808-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97808-111">**Element**</span></span>|<span data-ttu-id="97808-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97808-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97808-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="97808-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="97808-114">Содержит идентификатор папки назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="97808-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="97808-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="97808-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="97808-116">Определяет именованную папку назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="97808-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="97808-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="97808-117">Parent elements</span></span>

|<span data-ttu-id="97808-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="97808-118">**Element**</span></span>|<span data-ttu-id="97808-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="97808-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="97808-120">Действия</span><span class="sxs-lookup"><span data-stu-id="97808-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="97808-121">Представляет набор действий, которые доступны для выполнения на сообщение при условия будут выполнены.</span><span class="sxs-lookup"><span data-stu-id="97808-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="97808-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="97808-122">Text value</span></span>

<span data-ttu-id="97808-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="97808-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="97808-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="97808-124">Remarks</span></span>

<span data-ttu-id="97808-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="97808-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="97808-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="97808-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="97808-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="97808-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="97808-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="97808-128">Schema Name</span></span>  <br/> |<span data-ttu-id="97808-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="97808-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="97808-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="97808-130">Validation File</span></span>  <br/> |<span data-ttu-id="97808-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="97808-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="97808-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="97808-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="97808-133">True</span><span class="sxs-lookup"><span data-stu-id="97808-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="97808-134">См. также</span><span class="sxs-lookup"><span data-stu-id="97808-134">See also</span></span>



[<span data-ttu-id="97808-135">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="97808-135">MoveToFolder</span></span>](movetofolder.md)


- [<span data-ttu-id="97808-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="97808-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

