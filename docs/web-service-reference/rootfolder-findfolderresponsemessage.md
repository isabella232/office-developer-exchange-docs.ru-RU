---
title: Рутфолдер (Финдфолдерреспонсемессаже)
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
description: Элемент Рутфолдер содержит результаты поиска в одной корневой папке во время операции FindFolder.
ms.openlocfilehash: b5601d6abec67196c9991908e272a2122a201d69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457139"
---
# <a name="rootfolder-findfolderresponsemessage"></a><span data-ttu-id="056b4-103">Рутфолдер (Финдфолдерреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="056b4-103">RootFolder (FindFolderResponseMessage)</span></span>

<span data-ttu-id="056b4-104">Элемент **рутфолдер** содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="056b4-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Folders/>
</RootFolder>
```

 <span data-ttu-id="056b4-105">**финдфолдерпаренттипе**</span><span class="sxs-lookup"><span data-stu-id="056b4-105">**FindFolderParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="056b4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="056b4-106">Attributes and elements</span></span>

<span data-ttu-id="056b4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="056b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="056b4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="056b4-108">Attributes</span></span>

|<span data-ttu-id="056b4-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="056b4-109">**Attribute**</span></span>|<span data-ttu-id="056b4-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="056b4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="056b4-111">индекседпагингоффсет</span><span class="sxs-lookup"><span data-stu-id="056b4-111">IndexedPagingOffset</span></span>  <br/> |<span data-ttu-id="056b4-112">Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="056b4-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="056b4-113">нумератороффсет</span><span class="sxs-lookup"><span data-stu-id="056b4-113">NumeratorOffset</span></span>  <br/> |<span data-ttu-id="056b4-114">Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений дробной страницы.</span><span class="sxs-lookup"><span data-stu-id="056b4-114">Represents the new numerator value to use for the next request when using fractional page views.</span></span>  <br/> |
|<span data-ttu-id="056b4-115">абсолутеденоминатор</span><span class="sxs-lookup"><span data-stu-id="056b4-115">AbsoluteDenominator</span></span>  <br/> |<span data-ttu-id="056b4-116">Представляет следующий знаменатель, который будет использоваться для следующего запроса при выполнении дробного разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="056b4-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="056b4-117">инклудесластитеминранже</span><span class="sxs-lookup"><span data-stu-id="056b4-117">IncludesLastItemInRange</span></span>  <br/> |<span data-ttu-id="056b4-118">Указывает, содержит ли текущие результаты последнюю папку в запросе, что не требуется для дальнейшей разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="056b4-118">Indicates whether the current results contain the last folder in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="056b4-119">тоталитемсинвиев</span><span class="sxs-lookup"><span data-stu-id="056b4-119">TotalItemsInView</span></span>  <br/> |<span data-ttu-id="056b4-120">Представляет общее число папок, которые прошли ограничение.</span><span class="sxs-lookup"><span data-stu-id="056b4-120">Represents the total number of folders that pass the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="056b4-121">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="056b4-121">Child elements</span></span>

|<span data-ttu-id="056b4-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="056b4-122">**Element**</span></span>|<span data-ttu-id="056b4-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="056b4-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="056b4-124">Folders</span><span class="sxs-lookup"><span data-stu-id="056b4-124">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="056b4-125">Содержит массив папок, найденных с помощью [операции FindFolder](findfolder-operation.md).</span><span class="sxs-lookup"><span data-stu-id="056b4-125">Contains an array of folders found by using the [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="056b4-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="056b4-126">Parent elements</span></span>

|<span data-ttu-id="056b4-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="056b4-127">**Element**</span></span>|<span data-ttu-id="056b4-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="056b4-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="056b4-129">финдфолдерреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="056b4-129">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md) <br/> |<span data-ttu-id="056b4-130">Содержит состояние и результат запроса [операции FindFolder](findfolder-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="056b4-130">Contains the status and result of a [FindFolder operation](findfolder-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="056b4-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="056b4-131">Remarks</span></span>

<span data-ttu-id="056b4-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="056b4-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="056b4-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="056b4-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="056b4-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="056b4-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="056b4-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="056b4-135">Schema name</span></span>  <br/> |<span data-ttu-id="056b4-136">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="056b4-136">Messages schema</span></span>  <br/> |
|<span data-ttu-id="056b4-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="056b4-137">Validation file</span></span>  <br/> |<span data-ttu-id="056b4-138">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="056b4-138">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="056b4-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="056b4-139">Can be empty</span></span>  <br/> |<span data-ttu-id="056b4-140">False</span><span class="sxs-lookup"><span data-stu-id="056b4-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="056b4-141">См. также</span><span class="sxs-lookup"><span data-stu-id="056b4-141">See also</span></span>



[<span data-ttu-id="056b4-142">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="056b4-142">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="056b4-143">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="056b4-143">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

