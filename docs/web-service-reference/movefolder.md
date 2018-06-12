---
title: MoveFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolder
api_type:
- schema
ms.assetid: f2bb0a73-94d7-4bc7-8902-bd9c69120221
description: Элемент MoveFolder определяет запрос на перемещение в папку в хранилище Exchange.
ms.openlocfilehash: 42a990ced18cc13c7694042df786d33c018f346c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834485"
---
# <a name="movefolder"></a><span data-ttu-id="f3185-103">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="f3185-103">MoveFolder</span></span>

<span data-ttu-id="f3185-104">Элемент **MoveFolder** определяет запрос на перемещение в папку в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="f3185-104">The **MoveFolder** element defines a request to move a folder in the Exchange store.</span></span> 
  
```xml
<MoveFolder>
   <ToFolderId/>
   <FolderIds/>
</MoveFolder>
```

 <span data-ttu-id="f3185-105">**MoveFolderType**</span><span class="sxs-lookup"><span data-stu-id="f3185-105">**MoveFolderType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f3185-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f3185-106">Attributes and elements</span></span>

<span data-ttu-id="f3185-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f3185-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f3185-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f3185-108">Attributes</span></span>

<span data-ttu-id="f3185-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3185-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f3185-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f3185-110">Child elements</span></span>

|<span data-ttu-id="f3185-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f3185-111">**Element**</span></span>|<span data-ttu-id="f3185-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f3185-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f3185-113">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="f3185-113">ToFolderId</span></span>](tofolderid.md) <br/> |<span data-ttu-id="f3185-114">Представляет папку назначения для перемещенной папки.</span><span class="sxs-lookup"><span data-stu-id="f3185-114">Represents the destination folder for a moved folder.</span></span>  <br/> |
|[<span data-ttu-id="f3185-115">FolderIds</span><span class="sxs-lookup"><span data-stu-id="f3185-115">FolderIds</span></span>](folderids.md) <br/> |<span data-ttu-id="f3185-116">Содержит набор папок, которые следует переместить в папку, указанную в элементе [ToFolderId](tofolderid.md) .</span><span class="sxs-lookup"><span data-stu-id="f3185-116">Contains an array of folders to move to the folder identified by the [ToFolderId](tofolderid.md) element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f3185-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f3185-117">Parent elements</span></span>

<span data-ttu-id="f3185-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="f3185-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f3185-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="f3185-119">Remarks</span></span>

<span data-ttu-id="f3185-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f3185-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f3185-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f3185-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f3185-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f3185-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f3185-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f3185-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f3185-124">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f3185-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f3185-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f3185-125">Validation File</span></span>  <br/> |<span data-ttu-id="f3185-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f3185-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f3185-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f3185-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f3185-128">False</span><span class="sxs-lookup"><span data-stu-id="f3185-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f3185-129">См. также</span><span class="sxs-lookup"><span data-stu-id="f3185-129">See also</span></span>



[<span data-ttu-id="f3185-130">Операция MoveFolder</span><span class="sxs-lookup"><span data-stu-id="f3185-130">MoveFolder operation</span></span>](movefolder-operation.md)

