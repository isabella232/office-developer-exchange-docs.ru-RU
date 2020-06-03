---
title: MoveToFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveToFolder
api_type:
- schema
ms.assetid: 991673b9-b627-4848-bfba-59a187b8575f
description: Элемент MoveToFolder указывает идентификатор папки, в которую можно переместить элементы электронной почты.
ms.openlocfilehash: e323b2ac5390855b3db0b5495af667cdf2da5596
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530014"
---
# <a name="movetofolder"></a><span data-ttu-id="cc868-103">MoveToFolder</span><span class="sxs-lookup"><span data-stu-id="cc868-103">MoveToFolder</span></span>

<span data-ttu-id="cc868-104">Элемент **MoveToFolder** указывает идентификатор папки, в которую можно переместить элементы электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cc868-104">The **MoveToFolder** element specifies the identifier of the folder to which email items can be moved.</span></span> 
  
```XML
<MoveToFolder>
    <FolderId></FolderId>
    <DistinguishedFolderId></DistinguisedFolderId>
</MoveToFolder>
```

 <span data-ttu-id="cc868-105">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="cc868-105">**TargetFolderIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc868-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cc868-106">Attributes and elements</span></span>

<span data-ttu-id="cc868-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cc868-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc868-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cc868-108">Attributes</span></span>

<span data-ttu-id="cc868-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cc868-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc868-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cc868-110">Child elements</span></span>

|<span data-ttu-id="cc868-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cc868-111">**Element**</span></span>|<span data-ttu-id="cc868-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cc868-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc868-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="cc868-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="cc868-114">Содержит идентификатор папки назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="cc868-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="cc868-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="cc868-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="cc868-116">Определяет именованную папку назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="cc868-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc868-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cc868-117">Parent elements</span></span>

|<span data-ttu-id="cc868-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cc868-118">**Element**</span></span>|<span data-ttu-id="cc868-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cc868-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc868-120">Действия</span><span class="sxs-lookup"><span data-stu-id="cc868-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="cc868-121">Представляет набор действий, которые могут быть выполнены над сообщением при выполнении условий..</span><span class="sxs-lookup"><span data-stu-id="cc868-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled..</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cc868-122">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cc868-122">Text value</span></span>

<span data-ttu-id="cc868-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="cc868-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cc868-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="cc868-124">Remarks</span></span>

<span data-ttu-id="cc868-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc868-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc868-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cc868-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc868-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cc868-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc868-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cc868-128">Schema Name</span></span>  <br/> |<span data-ttu-id="cc868-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cc868-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cc868-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cc868-130">Validation File</span></span>  <br/> |<span data-ttu-id="cc868-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="cc868-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc868-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cc868-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc868-133">True</span><span class="sxs-lookup"><span data-stu-id="cc868-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc868-134">См. также</span><span class="sxs-lookup"><span data-stu-id="cc868-134">See also</span></span>



[<span data-ttu-id="cc868-135">CopyToFolder</span><span class="sxs-lookup"><span data-stu-id="cc868-135">CopyToFolder</span></span>](copytofolder.md)


- [<span data-ttu-id="cc868-136">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cc868-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

