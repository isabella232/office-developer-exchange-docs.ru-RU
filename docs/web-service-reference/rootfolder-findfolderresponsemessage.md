---
title: RootFolder (FindFolderResponseMessage)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 5089c815-663f-46be-bc59-aed9ee20f94a
description: Элемент RootFolder содержит результаты поиска в одной корневой папке во время операции FindFolder.
ms.openlocfilehash: 1cd79d5fa34318e7fe29606df84cbf0ef0520b93
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835253"
---
# <a name="rootfolder-findfolderresponsemessage"></a><span data-ttu-id="90bdb-103">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="90bdb-103">RootFolder (FindFolderResponseMessage)</span></span>

<span data-ttu-id="90bdb-104">Элемент **RootFolder** содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="90bdb-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 <span data-ttu-id="90bdb-105">**FindFolderParentType**</span><span class="sxs-lookup"><span data-stu-id="90bdb-105">**FindFolderParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="90bdb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="90bdb-106">Attributes and elements</span></span>

<span data-ttu-id="90bdb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="90bdb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="90bdb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="90bdb-108">Attributes</span></span>

|<span data-ttu-id="90bdb-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="90bdb-109">**Attribute**</span></span>|<span data-ttu-id="90bdb-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="90bdb-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="90bdb-111">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="90bdb-111">IndexedPagingOffset</span></span>  <br/> |<span data-ttu-id="90bdb-112">Представляет следующий индекс, который следует использовать для следующего запроса при использовании индексированного представления разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="90bdb-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="90bdb-113">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="90bdb-113">NumeratorOffset</span></span>  <br/> |<span data-ttu-id="90bdb-114">Представляет новое значение перечислителя использовать для следующего запроса при использовании дробная страницы представлений.</span><span class="sxs-lookup"><span data-stu-id="90bdb-114">Represents the new numerator value to use for the next request when using fractional page views.</span></span>  <br/> |
|<span data-ttu-id="90bdb-115">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="90bdb-115">AbsoluteDenominator</span></span>  <br/> |<span data-ttu-id="90bdb-116">Представляет Далее делителя для использования в следующем запросе при выполнении дробная разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="90bdb-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="90bdb-117">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="90bdb-117">IncludesLastItemInRange</span></span>  <br/> |<span data-ttu-id="90bdb-118">Указывает, содержат ли текущие результаты последнюю папку запроса, таким образом, что не требуется, дальнейшей постраничного просмотра.</span><span class="sxs-lookup"><span data-stu-id="90bdb-118">Indicates whether the current results contain the last folder in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="90bdb-119">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="90bdb-119">TotalItemsInView</span></span>  <br/> |<span data-ttu-id="90bdb-120">Представляет общее число папок, ограничение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="90bdb-120">Represents the total number of folders that pass the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="90bdb-121">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="90bdb-121">Child elements</span></span>

|<span data-ttu-id="90bdb-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="90bdb-122">**Element**</span></span>|<span data-ttu-id="90bdb-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="90bdb-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90bdb-124">Папки</span><span class="sxs-lookup"><span data-stu-id="90bdb-124">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="90bdb-125">Содержит набор папок, найденных с помощью [операции FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="90bdb-125">Contains an array of folders found by using the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="90bdb-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="90bdb-126">Parent elements</span></span>

|<span data-ttu-id="90bdb-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="90bdb-127">**Element**</span></span>|<span data-ttu-id="90bdb-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="90bdb-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="90bdb-129">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="90bdb-129">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="90bdb-130">Содержит состояние и результат [операции FindFolder](findfolder-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="90bdb-130">Contains the status and result of a [FindFolder operation](findfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="90bdb-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="90bdb-131">Remarks</span></span>

<span data-ttu-id="90bdb-132">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="90bdb-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="90bdb-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="90bdb-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="90bdb-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="90bdb-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="90bdb-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="90bdb-135">Schema name</span></span>  <br/> |<span data-ttu-id="90bdb-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="90bdb-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="90bdb-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="90bdb-137">Validation file</span></span>  <br/> |<span data-ttu-id="90bdb-138">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="90bdb-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="90bdb-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="90bdb-139">Can be empty</span></span>  <br/> |<span data-ttu-id="90bdb-140">False</span><span class="sxs-lookup"><span data-stu-id="90bdb-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="90bdb-141">См. также</span><span class="sxs-lookup"><span data-stu-id="90bdb-141">See also</span></span>



[<span data-ttu-id="90bdb-142">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="90bdb-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="90bdb-143">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="90bdb-143">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

