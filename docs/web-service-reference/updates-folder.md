---
title: Обновления (папка)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Updates
api_type:
- schema
ms.assetid: b047e3a4-a5ab-4098-b7a0-273bc809e702
description: Элемент Updates содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств папки.
ms.openlocfilehash: 3282171dfc188a9d4735a19a97e80fe0e2f79b89
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457181"
---
# <a name="updates-folder"></a><span data-ttu-id="cae2b-103">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="cae2b-103">Updates (Folder)</span></span>

<span data-ttu-id="cae2b-104">Элемент **Updates** содержит набор элементов, определяющих Добавление, установку и удаление изменений свойств папки.</span><span class="sxs-lookup"><span data-stu-id="cae2b-104">The **Updates** element contains a set of elements that define append, set, and delete changes to folder properties.</span></span> 
  
- [<span data-ttu-id="cae2b-105">UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="cae2b-105">UpdateFolder</span></span>](updatefolder.md)
  
- [<span data-ttu-id="cae2b-106">фолдерчанжес</span><span class="sxs-lookup"><span data-stu-id="cae2b-106">FolderChanges</span></span>](folderchanges.md)
  
- [<span data-ttu-id="cae2b-107">FolderChange</span><span class="sxs-lookup"><span data-stu-id="cae2b-107">FolderChange</span></span>](folderchange.md)
  
- [<span data-ttu-id="cae2b-108">Обновления (папка)</span><span class="sxs-lookup"><span data-stu-id="cae2b-108">Updates (Folder)</span></span>](updates-folder.md)
  
```xml
<Updates>
   <AppendToFolderField/>
   <SetFolderField/>
   <DeleteFolderField/>
</Updates>
```

<span data-ttu-id="cae2b-109">**нонемптяррайоффолдерчанжедескриптионстипе**</span><span class="sxs-lookup"><span data-stu-id="cae2b-109">**NonEmptyArrayOfFolderChangeDescriptionsType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cae2b-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cae2b-110">Attributes and elements</span></span>

<span data-ttu-id="cae2b-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cae2b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cae2b-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cae2b-112">Attributes</span></span>

<span data-ttu-id="cae2b-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cae2b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cae2b-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cae2b-114">Child elements</span></span>

|<span data-ttu-id="cae2b-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cae2b-115">**Element**</span></span>|<span data-ttu-id="cae2b-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cae2b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cae2b-117">аппендтофолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="cae2b-117">AppendToFolderField</span></span>](appendtofolderfield.md) <br/> |<span data-ttu-id="cae2b-118">Представляет данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="cae2b-118">Represents data to append to a folder property during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="cae2b-119">сетфолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="cae2b-119">SetFolderField</span></span>](setfolderfield.md) <br/> |<span data-ttu-id="cae2b-120">Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="cae2b-120">Represents an update to a single property on a folder in an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="cae2b-121">делетефолдерфиелд</span><span class="sxs-lookup"><span data-stu-id="cae2b-121">DeleteFolderField</span></span>](deletefolderfield.md) <br/> |<span data-ttu-id="cae2b-122">Представляет операцию удаления определенного свойства из папки во время [операции операцию UpdateFolder](updatefolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="cae2b-122">Represents an operation to delete a given property from a folder during an [UpdateFolder operation](updatefolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cae2b-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cae2b-123">Parent elements</span></span>

|<span data-ttu-id="cae2b-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cae2b-124">**Element**</span></span>|<span data-ttu-id="cae2b-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cae2b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cae2b-126">FolderChange</span><span class="sxs-lookup"><span data-stu-id="cae2b-126">FolderChange</span></span>](folderchange.md) <br/> |<span data-ttu-id="cae2b-127">Представляет коллекцию изменений, выполняемых над одной папкой.</span><span class="sxs-lookup"><span data-stu-id="cae2b-127">Represents a collection of changes to be performed on a single folder.</span></span>  <br/> <span data-ttu-id="cae2b-128">Ниже приведено выражение XPath для этого элемента:`/UpdateFolder/FolderChanges/FolderChange[i]`</span><span class="sxs-lookup"><span data-stu-id="cae2b-128">The following is the XPath expression to this element:  `/UpdateFolder/FolderChanges/FolderChange[i]`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cae2b-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="cae2b-129">Remarks</span></span>

<span data-ttu-id="cae2b-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cae2b-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cae2b-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cae2b-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cae2b-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cae2b-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cae2b-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cae2b-133">Schema Name</span></span>  <br/> |<span data-ttu-id="cae2b-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cae2b-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="cae2b-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cae2b-135">Validation File</span></span>  <br/> |<span data-ttu-id="cae2b-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cae2b-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cae2b-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cae2b-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="cae2b-138">False</span><span class="sxs-lookup"><span data-stu-id="cae2b-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cae2b-139">См. также</span><span class="sxs-lookup"><span data-stu-id="cae2b-139">See also</span></span>

- [<span data-ttu-id="cae2b-140">Операция UpdateFolder</span><span class="sxs-lookup"><span data-stu-id="cae2b-140">UpdateFolder operation</span></span>](updatefolder-operation.md)
- [<span data-ttu-id="cae2b-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cae2b-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

