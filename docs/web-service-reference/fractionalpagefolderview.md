---
title: FractionalPageFolderView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageFolderView
api_type:
- schema
ms.assetid: ef681f8a-136a-4c0e-ade6-ddcdbf2d85ad
description: Элемент FractionalPageFolderView описывается, где начала страничного представления и максимальное число папок, возвращаемых в запросе FindFolder.
ms.openlocfilehash: 3cb5f8333634a0c484ae3ce6a6256631cff57cc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762647"
---
# <a name="fractionalpagefolderview"></a><span data-ttu-id="6cefb-103">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="6cefb-103">FractionalPageFolderView</span></span>

<span data-ttu-id="6cefb-104">Элемент **FractionalPageFolderView** описывается, где начала страничного представления и максимальное число папок, возвращаемых в запросе [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="6cefb-104">The **FractionalPageFolderView** element describes where the paged view starts and the maximum number of folders returned in a [FindFolder](findfolder.md) request.</span></span> 
  
[<span data-ttu-id="6cefb-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="6cefb-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="6cefb-106">FractionalPageFolderView</span><span class="sxs-lookup"><span data-stu-id="6cefb-106">FractionalPageFolderView</span></span>](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="6cefb-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="6cefb-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cefb-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6cefb-108">Attributes and elements</span></span>

<span data-ttu-id="6cefb-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6cefb-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cefb-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6cefb-110">Attributes</span></span>

|<span data-ttu-id="6cefb-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="6cefb-111">**Attribute**</span></span>|<span data-ttu-id="6cefb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6cefb-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6cefb-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="6cefb-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="6cefb-114">Определяет максимальное число результатов, возвращаемых в ответе [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="6cefb-114">Identifies the maximum number of results to return in the [FindFolder](findfolder.md) response.</span></span> <span data-ttu-id="6cefb-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6cefb-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="6cefb-116">**Числитель**</span><span class="sxs-lookup"><span data-stu-id="6cefb-116">**Numerator**</span></span> <br/> |<span data-ttu-id="6cefb-117">Представляет числитель дробная смещения от начала набора результатов.</span><span class="sxs-lookup"><span data-stu-id="6cefb-117">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="6cefb-118">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="6cefb-118">This attribute is required.</span></span> <span data-ttu-id="6cefb-119">Числитель должно быть равно или меньше, чем делителя.</span><span class="sxs-lookup"><span data-stu-id="6cefb-119">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="6cefb-120">Этот атрибут должен представлять целочисленное значение, которое равно или больше нуля.</span><span class="sxs-lookup"><span data-stu-id="6cefb-120">This attribute must represent an integral value that is equal to or greater than zero.</span></span> <span data-ttu-id="6cefb-121">Дополнительные сведения см.</span><span class="sxs-lookup"><span data-stu-id="6cefb-121">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="6cefb-122">**Делителя**</span><span class="sxs-lookup"><span data-stu-id="6cefb-122">**Denominator**</span></span> <br/> |<span data-ttu-id="6cefb-123">Представляет делителя дробная смещением от начала общее число папок в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="6cefb-123">Represents the denominator of the fractional offset from the start of the total number of folders in the result set.</span></span> <span data-ttu-id="6cefb-124">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="6cefb-124">This attribute is required.</span></span> <span data-ttu-id="6cefb-125">Этот атрибут должен представлять целое число, которое больше одного.</span><span class="sxs-lookup"><span data-stu-id="6cefb-125">This attribute must represent an integral value that is greater than one.</span></span> <span data-ttu-id="6cefb-126">Дополнительные сведения см.</span><span class="sxs-lookup"><span data-stu-id="6cefb-126">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6cefb-127">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6cefb-127">Child elements</span></span>

<span data-ttu-id="6cefb-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="6cefb-128">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6cefb-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6cefb-129">Parent elements</span></span>

|<span data-ttu-id="6cefb-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6cefb-130">**Element**</span></span>|<span data-ttu-id="6cefb-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6cefb-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cefb-132">FindFolder</span><span class="sxs-lookup"><span data-stu-id="6cefb-132">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="6cefb-133">Определяет запрос для определения папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6cefb-133">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="6cefb-134">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="6cefb-134">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6cefb-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="6cefb-135">Remarks</span></span>

<span data-ttu-id="6cefb-136">Смещение страничного представления от начала набора папок, обнаруженного описывается функцией.</span><span class="sxs-lookup"><span data-stu-id="6cefb-136">The paged view offset from the start of the set of found folders is described by a fraction.</span></span> <span data-ttu-id="6cefb-137">Дроби, которая определяется **числитель** и **делителя** атрибуты, описание которых начинается страницы сведений.</span><span class="sxs-lookup"><span data-stu-id="6cefb-137">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="6cefb-138">К примеру Если **числитель** равно четыре и **делителя** равно пять, страница возвращенных данных начинается запись находится четыре пятых длины способ в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="6cefb-138">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="6cefb-139">Если дроби равно нулю, это означает начала набора результатов.</span><span class="sxs-lookup"><span data-stu-id="6cefb-139">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="6cefb-140">Если дроби оценивается как одно, это означает конец набора результатов.</span><span class="sxs-lookup"><span data-stu-id="6cefb-140">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="6cefb-141">Дроби представляет начальную точку страницы, будут возвращены не число результатов в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="6cefb-141">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="6cefb-142">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6cefb-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cefb-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6cefb-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cefb-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6cefb-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cefb-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6cefb-145">Schema Name</span></span>  <br/> |<span data-ttu-id="6cefb-146">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6cefb-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6cefb-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6cefb-147">Validation File</span></span>  <br/> |<span data-ttu-id="6cefb-148">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6cefb-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cefb-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6cefb-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="6cefb-150">False</span><span class="sxs-lookup"><span data-stu-id="6cefb-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cefb-151">См. также</span><span class="sxs-lookup"><span data-stu-id="6cefb-151">See also</span></span>



[<span data-ttu-id="6cefb-152">FindFolder Operation</span><span class="sxs-lookup"><span data-stu-id="6cefb-152">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="6cefb-153">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="6cefb-153">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

