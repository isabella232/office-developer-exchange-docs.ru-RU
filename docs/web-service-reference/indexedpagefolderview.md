---
title: индекседпажефолдервиев
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
description: Элемент Индекседпажефолдервиев описывает, как возвращаются сведения о страничном элементе в отклике FindFolder.
ms.openlocfilehash: f32f778daa6fa3fea93ab2bc1951f2407dcf7f80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833910"
---
# <a name="indexedpagefolderview"></a><span data-ttu-id="b7896-103">индекседпажефолдервиев</span><span class="sxs-lookup"><span data-stu-id="b7896-103">IndexedPageFolderView</span></span>

<span data-ttu-id="b7896-104">Элемент **индекседпажефолдервиев** описывает, как возвращаются сведения о страничном элементе в отклике [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="b7896-104">The **IndexedPageFolderView** element describes how paged item information is returned in a [FindFolder](findfolder.md) response.</span></span> 
  
[<span data-ttu-id="b7896-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="b7896-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="b7896-106">индекседпажефолдервиев</span><span class="sxs-lookup"><span data-stu-id="b7896-106">IndexedPageFolderView</span></span>](indexedpagefolderview.md)
  
```xml
<IndexedPageFolderView MaxEntriesReturned="" Offset="" BasePoint="" />
```

 <span data-ttu-id="b7896-107">**индекседпажевиевтипе**</span><span class="sxs-lookup"><span data-stu-id="b7896-107">**IndexedPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7896-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b7896-108">Attributes and elements</span></span>

<span data-ttu-id="b7896-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b7896-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7896-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b7896-110">Attributes</span></span>

|<span data-ttu-id="b7896-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b7896-111">**Attribute**</span></span>|<span data-ttu-id="b7896-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b7896-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b7896-113">**максентриесретурнед**</span><span class="sxs-lookup"><span data-stu-id="b7896-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="b7896-114">Описывает максимальное число папок, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="b7896-114">Describes the maximum number of folders to return in the response.</span></span> <span data-ttu-id="b7896-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="b7896-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="b7896-116">**Offset**</span><span class="sxs-lookup"><span data-stu-id="b7896-116">**Offset**</span></span> <br/> |<span data-ttu-id="b7896-117">Описывает смещение от **басепоинт**.</span><span class="sxs-lookup"><span data-stu-id="b7896-117">Describes the offset from the **BasePoint**.</span></span> <span data-ttu-id="b7896-118">Смещение должно быть больше или равно нулю.</span><span class="sxs-lookup"><span data-stu-id="b7896-118">Offset must be greater than or equal to zero.</span></span> <span data-ttu-id="b7896-119">Если **басепоинт** равно "начало", смещение является положительным.</span><span class="sxs-lookup"><span data-stu-id="b7896-119">If **BasePoint** is equal to Beginning, the offset is positive.</span></span> <span data-ttu-id="b7896-120">Если **басепоинт** равен end, то смещение обрабатывается так, как если бы оно было отрицательным.</span><span class="sxs-lookup"><span data-stu-id="b7896-120">If **BasePoint** is equal to End, the offset is handled as if it were negative.</span></span>  <br/> <span data-ttu-id="b7896-121">Этот параметр определяет, какая папка будет первой папкой, доставляемой в ответе.</span><span class="sxs-lookup"><span data-stu-id="b7896-121">This identifies which folder will be the first folder delivered in the response.</span></span> <span data-ttu-id="b7896-122">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b7896-122">This attribute is required.</span></span>  <br/> |
|<span data-ttu-id="b7896-123">**басепоинт**</span><span class="sxs-lookup"><span data-stu-id="b7896-123">**BasePoint**</span></span> <br/> |<span data-ttu-id="b7896-124">Указывает, будет ли страница папок начинаться с начала или с конца набора папок, найденных с помощью условий поиска.</span><span class="sxs-lookup"><span data-stu-id="b7896-124">Describes whether the page of folders will start from the start or the end of the set of folders that are found with the search criteria.</span></span> <span data-ttu-id="b7896-125">Поиск от End всегда выполняет поиск в обратном направлении.</span><span class="sxs-lookup"><span data-stu-id="b7896-125">Seeking from the end always searches backward.</span></span> <span data-ttu-id="b7896-126">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b7896-126">This attribute is required.</span></span>  <br/> |
   
#### <a name="basepoint-attribute"></a><span data-ttu-id="b7896-127">Атрибут Басепоинт</span><span class="sxs-lookup"><span data-stu-id="b7896-127">BasePoint Attribute</span></span>

|<span data-ttu-id="b7896-128">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b7896-128">**Value**</span></span>|<span data-ttu-id="b7896-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b7896-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b7896-130">Слайд</span><span class="sxs-lookup"><span data-stu-id="b7896-130">Beginning</span></span>  <br/> |<span data-ttu-id="b7896-131">Постраничное представление начинается с начала найденного набора папок.</span><span class="sxs-lookup"><span data-stu-id="b7896-131">The paged view starts at the beginning of the found folder set.</span></span>  <br/> |
|<span data-ttu-id="b7896-132">Конец</span><span class="sxs-lookup"><span data-stu-id="b7896-132">End</span></span>  <br/> |<span data-ttu-id="b7896-133">Постраничное представление начинается в конце найденного набора папок.</span><span class="sxs-lookup"><span data-stu-id="b7896-133">The paged view starts at the end of the found folder set.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b7896-134">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b7896-134">Child elements</span></span>

<span data-ttu-id="b7896-135">Нет.</span><span class="sxs-lookup"><span data-stu-id="b7896-135">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b7896-136">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b7896-136">Parent elements</span></span>

|<span data-ttu-id="b7896-137">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b7896-137">**Element**</span></span>|<span data-ttu-id="b7896-138">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b7896-138">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7896-139">FindFolder</span><span class="sxs-lookup"><span data-stu-id="b7896-139">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="b7896-140">Определяет запрос на поиск папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="b7896-140">Defines a request to find folders in a mailbox.</span></span>  <br/> <span data-ttu-id="b7896-141">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="b7896-141">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b7896-142">Примечания</span><span class="sxs-lookup"><span data-stu-id="b7896-142">Remarks</span></span>

<span data-ttu-id="b7896-143">Поиск с конца включает переход к началу, определяемому смещением.</span><span class="sxs-lookup"><span data-stu-id="b7896-143">Seeking from end involves moving to the origin identified by the offset.</span></span> <span data-ttu-id="b7896-144">Кроме того, указатель перемещается обратно на число запрошенных записей.</span><span class="sxs-lookup"><span data-stu-id="b7896-144">Additionally, the pointer is moved back by the number of requested records.</span></span> <span data-ttu-id="b7896-145">Например, если имеется 100 записей, а смещение — 25 из конца, поиск начинается с 75.</span><span class="sxs-lookup"><span data-stu-id="b7896-145">For example, if there are 100 records and the offset is 25 from the end, the search starts from 75.</span></span> <span data-ttu-id="b7896-146">Если возвращено 10 записей, указатель перемещается обратно в обратное 10 записей в 65 и возвращает записи от 65 до 75.</span><span class="sxs-lookup"><span data-stu-id="b7896-146">If 10 records are returned, the pointer is moved backward an additional 10 records to 65 and returns records 65 through 75.</span></span> <span data-ttu-id="b7896-147">Следующий индекс — 64.</span><span class="sxs-lookup"><span data-stu-id="b7896-147">The next index is 64.</span></span> <span data-ttu-id="b7896-148">Следующее смещение от конца для страницы составляет 100 минус 64, что равно 36.</span><span class="sxs-lookup"><span data-stu-id="b7896-148">The next offset from the end for a page is 100 minus 64 which equals 36.</span></span> <span data-ttu-id="b7896-149">Значение для следующего смещения из конца для получения следующей индексированной страницы — 36.</span><span class="sxs-lookup"><span data-stu-id="b7896-149">The value for the next offset from the end to get the next indexed page is 36.</span></span>
  
<span data-ttu-id="b7896-150">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b7896-150">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7896-151">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b7896-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7896-152">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b7896-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b7896-153">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b7896-153">Schema Name</span></span>  <br/> |<span data-ttu-id="b7896-154">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="b7896-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b7896-155">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b7896-155">Validation File</span></span>  <br/> |<span data-ttu-id="b7896-156">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="b7896-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7896-157">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b7896-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="b7896-158">False</span><span class="sxs-lookup"><span data-stu-id="b7896-158">False</span></span>  <br/> |
   

