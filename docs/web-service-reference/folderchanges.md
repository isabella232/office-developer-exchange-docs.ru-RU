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
ms.openlocfilehash: 5481496100512584fd0b9745ee42d5b9516bd7fb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458385"
---
# <a name="folderchanges"></a><span data-ttu-id="820b1-103">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="820b1-103">FolderChanges</span></span>

<span data-ttu-id="820b1-104">Элемент **фолдерчанжес** представляет коллекцию изменений для папки.</span><span class="sxs-lookup"><span data-stu-id="820b1-104">The **FolderChanges** element represents a collection of changes for a folder.</span></span> 
  
[<span data-ttu-id="820b1-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="820b1-105">UpdateFolder</span></span>](updatefolder.md)
  
[<span data-ttu-id="820b1-106">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="820b1-106">FolderChanges</span></span>](folderchanges.md)
  
```xml
<FolderChanges>
   <FolderChange/>
</FolderChanges>
```

 <span data-ttu-id="820b1-107">**нонемптяррайоффолдерчанжестипе**</span><span class="sxs-lookup"><span data-stu-id="820b1-107">**NonEmptyArrayOfFolderChangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="820b1-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="820b1-108">Attributes and elements</span></span>

<span data-ttu-id="820b1-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="820b1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="820b1-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="820b1-110">Attributes</span></span>

<span data-ttu-id="820b1-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="820b1-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="820b1-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="820b1-112">Child elements</span></span>

|<span data-ttu-id="820b1-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="820b1-113">**Element**</span></span>|<span data-ttu-id="820b1-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="820b1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="820b1-115">FolderChange</span><span class="sxs-lookup"><span data-stu-id="820b1-115">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="820b1-116">Представляет одно изменение, которое необходимо выполнить для одной папки.</span><span class="sxs-lookup"><span data-stu-id="820b1-116">Represents a single change to be performed on a single folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="820b1-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="820b1-117">Parent elements</span></span>

|<span data-ttu-id="820b1-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="820b1-118">**Element**</span></span>|<span data-ttu-id="820b1-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="820b1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="820b1-120">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="820b1-120">UpdateFolder</span></span>](updatefolder.md) <br/> |<span data-ttu-id="820b1-121">Представляет операцию, используемую для обновления свойств папки.</span><span class="sxs-lookup"><span data-stu-id="820b1-121">Represents the operation that is used to update properties for a folder.</span></span>  <br/> <span data-ttu-id="820b1-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="820b1-122">The following is the XPath expression to this element:</span></span>  <br/>  `/UpdateFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="820b1-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="820b1-123">Remarks</span></span>

<span data-ttu-id="820b1-124">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="820b1-124">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="820b1-125">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="820b1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="820b1-126">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="820b1-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="820b1-127">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="820b1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="820b1-128">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="820b1-128">Messages schema</span></span>  <br/> |
|<span data-ttu-id="820b1-129">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="820b1-129">Validation File</span></span>  <br/> |<span data-ttu-id="820b1-130">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="820b1-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="820b1-131">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="820b1-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="820b1-132">False</span><span class="sxs-lookup"><span data-stu-id="820b1-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="820b1-133">См. также</span><span class="sxs-lookup"><span data-stu-id="820b1-133">See also</span></span>



[<span data-ttu-id="820b1-134">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="820b1-134">UpdateFolder operation</span></span>](updatefolder-operation.md)

