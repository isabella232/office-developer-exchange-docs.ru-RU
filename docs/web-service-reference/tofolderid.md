---
title: тофолдерид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: Элемент Тофолдерид представляет папку назначения для скопированного или перемещенного элемента или папки.
ms.openlocfilehash: c9cceb17fd55b7357d54b37bf4c8da1137d39b6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/02/2020
ms.locfileid: "44468777"
---
# <a name="tofolderid"></a><span data-ttu-id="4cd83-103">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="4cd83-103">ToFolderId</span></span>

<span data-ttu-id="4cd83-104">Элемент **тофолдерид** представляет папку назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="4cd83-104">The **ToFolderId** element represents the destination folder for a copied or moved item or folder.</span></span> 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
</ToFolderId>
```

<span data-ttu-id="4cd83-105">**таржетфолдеридтипе**</span><span class="sxs-lookup"><span data-stu-id="4cd83-105">**TargetFolderIdType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4cd83-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4cd83-106">Attributes and elements</span></span>

<span data-ttu-id="4cd83-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4cd83-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4cd83-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4cd83-108">Attributes</span></span>

<span data-ttu-id="4cd83-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4cd83-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4cd83-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4cd83-110">Child elements</span></span>

|<span data-ttu-id="4cd83-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cd83-111">**Element**</span></span>|<span data-ttu-id="4cd83-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cd83-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cd83-113">FolderId</span><span class="sxs-lookup"><span data-stu-id="4cd83-113">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="4cd83-114">Содержит идентификатор папки назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="4cd83-114">Contains the identifier of a destination folder for a copied or moved item or folder.</span></span>  <br/> |
|[<span data-ttu-id="4cd83-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="4cd83-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md) <br/> |<span data-ttu-id="4cd83-116">Определяет именованную папку назначения для скопированного или перемещенного элемента или папки.</span><span class="sxs-lookup"><span data-stu-id="4cd83-116">Identifies a named destination folder for a copied or moved item or folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4cd83-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4cd83-117">Parent elements</span></span>

|<span data-ttu-id="4cd83-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4cd83-118">**Element**</span></span>|<span data-ttu-id="4cd83-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4cd83-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4cd83-120">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="4cd83-120">MoveFolder</span></span>](movefolder.md) <br/> |<span data-ttu-id="4cd83-121">Определяет запрос на перемещение папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cd83-121">Defines a request to move a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="4cd83-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="4cd83-122">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveFolder` <br/> |
|[<span data-ttu-id="4cd83-123">CopyFolder</span><span class="sxs-lookup"><span data-stu-id="4cd83-123">CopyFolder</span></span>](copyfolder.md) <br/> |<span data-ttu-id="4cd83-124">Определяет запрос на копирование папки в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cd83-124">Defines a request to copy a folder in the Exchange store.</span></span>  <br/> <span data-ttu-id="4cd83-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="4cd83-125">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyFolder` <br/> |
|[<span data-ttu-id="4cd83-126">MoveItem</span><span class="sxs-lookup"><span data-stu-id="4cd83-126">MoveItem</span></span>](moveitem.md) <br/> |<span data-ttu-id="4cd83-127">Определяет запрос на перемещение элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cd83-127">Defines a request to move an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="4cd83-128">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="4cd83-128">The following is the XPath expression to this element:</span></span>  <br/>  `/MoveItem` <br/> |
|[<span data-ttu-id="4cd83-129">CopyItem</span><span class="sxs-lookup"><span data-stu-id="4cd83-129">CopyItem</span></span>](copyitem.md) <br/> |<span data-ttu-id="4cd83-130">Определяет запрос на копирование элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="4cd83-130">Defines a request to copy an item in the Exchange store.</span></span>  <br/> <span data-ttu-id="4cd83-131">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="4cd83-131">The following is the XPath expression to this element:</span></span>  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4cd83-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="4cd83-132">Remarks</span></span>

<span data-ttu-id="4cd83-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4cd83-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4cd83-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4cd83-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4cd83-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4cd83-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4cd83-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4cd83-136">Schema Name</span></span>  <br/> |<span data-ttu-id="4cd83-137">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="4cd83-137">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4cd83-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4cd83-138">Validation File</span></span>  <br/> |<span data-ttu-id="4cd83-139">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="4cd83-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4cd83-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4cd83-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="4cd83-141">False</span><span class="sxs-lookup"><span data-stu-id="4cd83-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4cd83-142">См. также</span><span class="sxs-lookup"><span data-stu-id="4cd83-142">See also</span></span>

- [<span data-ttu-id="4cd83-143">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="4cd83-143">MoveFolder operation</span></span>](movefolder-operation.md)  
- [<span data-ttu-id="4cd83-144">Операция CopyFolder</span><span class="sxs-lookup"><span data-stu-id="4cd83-144">CopyFolder operation</span></span>](copyfolder-operation.md) 
- [<span data-ttu-id="4cd83-145">Операция MoveItem</span><span class="sxs-lookup"><span data-stu-id="4cd83-145">MoveItem operation</span></span>](moveitem-operation.md) 
- [<span data-ttu-id="4cd83-146">Операция CopyItem</span><span class="sxs-lookup"><span data-stu-id="4cd83-146">CopyItem operation</span></span>](copyitem-operation.md)

