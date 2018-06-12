---
title: IndexedPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndexedPageFolderView
api_type:
- schema
ms.assetid: c6dac232-244b-4db0-9a15-5e01b8aa7a7d
description: Элемент IndexedPageFolderView описывает, как выгружаемый элемента сведения возвращаются в ответ FindFolder.
ms.openlocfilehash: f32f778daa6fa3fea93ab2bc1951f2407dcf7f80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833910"
---
# <a name="indexedpagefolderview"></a><span data-ttu-id="cb331-103">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="cb331-103">IndexedPageFolderView</span></span>

<span data-ttu-id="cb331-104">Элемент **IndexedPageFolderView** описывает, как выгружаемый элемента сведения возвращаются в ответ [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="cb331-104">The **IndexedPageFolderView** element describes how paged item information is returned in a [FindFolder](findfolder.md) response.</span></span> 
  
[<span data-ttu-id="cb331-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="cb331-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="cb331-106">IndexedPageFolderView</span><span class="sxs-lookup"><span data-stu-id="cb331-106">IndexedPageFolderView</span></span>](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 <span data-ttu-id="cb331-107">**IndexedPageViewType**</span><span class="sxs-lookup"><span data-stu-id="cb331-107">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb331-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cb331-108">Attributes and elements</span></span>

<span data-ttu-id="cb331-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="cb331-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb331-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cb331-110">Attributes</span></span>

|<span data-ttu-id="cb331-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="cb331-111">**Attribute**</span></span>|<span data-ttu-id="cb331-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb331-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb331-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="cb331-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="cb331-114">Описывает максимальное число папок для возврата в ответе.</span><span class="sxs-lookup"><span data-stu-id="cb331-114">Describes the maximum number of folders to return in the response.</span></span> <span data-ttu-id="cb331-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cb331-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="cb331-116">**Смещение**</span><span class="sxs-lookup"><span data-stu-id="cb331-116">**Offset**</span></span> <br/> |<span data-ttu-id="cb331-117">Описание смещения от **Базисная точка**.</span><span class="sxs-lookup"><span data-stu-id="cb331-117">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="cb331-118">Смещение должно быть больше или равно нулю.</span><span class="sxs-lookup"><span data-stu-id="cb331-118">Offset must be greater than or equal to zero.</span></span> <span data-ttu-id="cb331-119">Если **Базисная точка** равна начала, смещение является положительным.</span><span class="sxs-lookup"><span data-stu-id="cb331-119">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="cb331-120">Если **Базисная точка** равна End, смещение обрабатывается как если бы он был отрицательным.</span><span class="sxs-lookup"><span data-stu-id="cb331-120">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span>  <br/> <span data-ttu-id="cb331-121">Определяет, какие папки будут первой папки доставлено в ответе.</span><span class="sxs-lookup"><span data-stu-id="cb331-121">This identifies which folder will be the first folder delivered in the response.</span></span> <span data-ttu-id="cb331-122">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="cb331-122">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="cb331-123">**Базисная точка**</span><span class="sxs-lookup"><span data-stu-id="cb331-123">**BasePoint**</span></span> <br/> |<span data-ttu-id="cb331-124">Описывает ли страницы папок будет запущен процесс от начала или окончания в набор папок, найденных с условия поиска.</span><span class="sxs-lookup"><span data-stu-id="cb331-124">Describes whether the page of folders will start from the start or the end of the set of folders that are found with the search criteria.</span></span> <span data-ttu-id="cb331-125">При поиске с конца всегда ищет в обратном направлении.</span><span class="sxs-lookup"><span data-stu-id="cb331-125">Seeking from the end always searches backward.</span></span> <span data-ttu-id="cb331-126">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="cb331-126">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="cb331-127">Атрибут Базисная точка</span><span class="sxs-lookup"><span data-stu-id="cb331-127">BasePoint Attribute</span></span>

|<span data-ttu-id="cb331-128">**Значение**</span><span class="sxs-lookup"><span data-stu-id="cb331-128">**Value**</span></span>|<span data-ttu-id="cb331-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb331-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb331-130">Начало</span><span class="sxs-lookup"><span data-stu-id="cb331-130">Beginning</span></span>  <br/> |<span data-ttu-id="cb331-131">Постраничное представление начинается с начала набора обнаруженного папки.</span><span class="sxs-lookup"><span data-stu-id="cb331-131">The paged view starts at the beginning of the found folder set.</span></span>  <br/> |
|<span data-ttu-id="cb331-132">End</span><span class="sxs-lookup"><span data-stu-id="cb331-132">End</span></span>  <br/> |<span data-ttu-id="cb331-133">Постраничное представление начинается в конце набора обнаруженного папок.</span><span class="sxs-lookup"><span data-stu-id="cb331-133">The paged view starts at the end of the found folder set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cb331-134">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cb331-134">Child elements</span></span>

<span data-ttu-id="cb331-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="cb331-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cb331-136">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cb331-136">Parent elements</span></span>

|<span data-ttu-id="cb331-137">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cb331-137">**Element**</span></span>|<span data-ttu-id="cb331-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb331-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb331-139">FindFolder</span><span class="sxs-lookup"><span data-stu-id="cb331-139">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="cb331-140">Определяет запрос для поиска папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="cb331-140">Defines a request to find folders in a mailbox.</span></span>  <br/> <span data-ttu-id="cb331-141">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="cb331-141">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cb331-142">Замечания</span><span class="sxs-lookup"><span data-stu-id="cb331-142">Remarks</span></span>

<span data-ttu-id="cb331-143">Поиск из плана включает в себя перемещение происхождения, определяемую средством смещение.</span><span class="sxs-lookup"><span data-stu-id="cb331-143">Seeking from end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="cb331-144">Кроме того указатель возвращается назад на число запрошенных записей.</span><span class="sxs-lookup"><span data-stu-id="cb331-144">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="cb331-145">Например если существует 100 записей и смещение равно 25 с конца, поиск начинается с 75.</span><span class="sxs-lookup"><span data-stu-id="cb331-145">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="cb331-146">Если будет возвращено 10 записей, указатель мыши перемещается назад дополнительные 10 записывает 65 и возвращает записи 65 через 75.</span><span class="sxs-lookup"><span data-stu-id="cb331-146">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="cb331-147">Следующий индекс — 64.</span><span class="sxs-lookup"><span data-stu-id="cb331-147">The next index is 64.</span></span> <span data-ttu-id="cb331-148">Далее смещение с конца страницы равно 100 минус 64, которое равно 36.</span><span class="sxs-lookup"><span data-stu-id="cb331-148">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="cb331-149">Значение для следующего смещения с конца для получения следующей страницы индексированных — 36.</span><span class="sxs-lookup"><span data-stu-id="cb331-149">The value for the next offset from the end to get the next indexed page is 36.</span></span>
  
<span data-ttu-id="cb331-150">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cb331-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb331-151">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cb331-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb331-152">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cb331-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cb331-153">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cb331-153">Schema Name</span></span>  <br/> |<span data-ttu-id="cb331-154">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="cb331-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cb331-155">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cb331-155">Validation File</span></span>  <br/> |<span data-ttu-id="cb331-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cb331-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cb331-157">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cb331-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb331-158">False</span><span class="sxs-lookup"><span data-stu-id="cb331-158">False</span></span>  <br/> |
   

