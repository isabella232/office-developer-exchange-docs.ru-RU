---
title: фолдерчанжес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChanges
api_type:
- schema
ms.assetid: d3f611ed-56a4-43f8-aa65-cbd7844b827f
description: Элемент Фолдерчанжес представляет коллекцию изменений для папки.
ms.openlocfilehash: 7ab89e79f6babb5e93863974835685c6975d96dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762611"
---
# <a name="folderchanges"></a><span data-ttu-id="1ac02-103">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="1ac02-103">FolderChanges</span></span>

<span data-ttu-id="1ac02-104">Элемент **фолдерчанжес** представляет коллекцию изменений для папки.</span><span class="sxs-lookup"><span data-stu-id="1ac02-104">The **FolderChanges** element represents a collection of changes for a folder.</span></span> 
  
[<span data-ttu-id="1ac02-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1ac02-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="1ac02-106">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="1ac02-106">FolderChanges</span></span>](folderchanges.md)
  
```xml
<FolderChanges>
   <FolderChange/>
</FolderChanges>
```

 <span data-ttu-id="1ac02-107">**нонемптяррайоффолдерчанжестипе**</span><span class="sxs-lookup"><span data-stu-id="1ac02-107">**NonEmptyArrayOfFolderChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ac02-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1ac02-108">Attributes and elements</span></span>

<span data-ttu-id="1ac02-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1ac02-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ac02-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1ac02-110">Attributes</span></span>

<span data-ttu-id="1ac02-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1ac02-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ac02-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1ac02-112">Child elements</span></span>

|<span data-ttu-id="1ac02-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1ac02-113">**Element**</span></span>|<span data-ttu-id="1ac02-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1ac02-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ac02-115">FolderChange</span><span class="sxs-lookup"><span data-stu-id="1ac02-115">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="1ac02-116">Представляет одно изменение, которое необходимо выполнить для одной папки.</span><span class="sxs-lookup"><span data-stu-id="1ac02-116">Represents a single change to be performed on a single folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1ac02-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1ac02-117">Parent elements</span></span>

|<span data-ttu-id="1ac02-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1ac02-118">**Element**</span></span>|<span data-ttu-id="1ac02-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1ac02-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ac02-120">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1ac02-120">UpdateFolder</span></span>](updatefolder.md) <br/> |<span data-ttu-id="1ac02-121">Представляет операцию, используемую для обновления свойств папки.</span><span class="sxs-lookup"><span data-stu-id="1ac02-121">Represents the operation that is used to update properties for a folder.</span></span>  <br/> <span data-ttu-id="1ac02-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="1ac02-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1ac02-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="1ac02-123">Remarks</span></span>

<span data-ttu-id="1ac02-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1ac02-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ac02-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1ac02-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ac02-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1ac02-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ac02-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1ac02-127">Schema Name</span></span>  <br/> |<span data-ttu-id="1ac02-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1ac02-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ac02-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1ac02-129">Validation File</span></span>  <br/> |<span data-ttu-id="1ac02-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="1ac02-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ac02-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1ac02-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ac02-132">False</span><span class="sxs-lookup"><span data-stu-id="1ac02-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ac02-133">См. также</span><span class="sxs-lookup"><span data-stu-id="1ac02-133">See also</span></span>



[<span data-ttu-id="1ac02-134">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="1ac02-134">UpdateFolder operation</span></span>](updatefolder-operation.md)

