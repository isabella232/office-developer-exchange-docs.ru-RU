---
title: FractionalPageItemView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FractionalPageItemView
api_type:
- schema
ms.assetid: 4111afec-35e7-4c6f-b291-9bbba603f633
description: Элемент FractionalPageItemView описывается, где начала страничного представления и максимальное число элементов, возвращаемых в запросе FindItem.
ms.openlocfilehash: 38c35d2b68dabfca1a43ab034deaf72c47b0ea66
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762650"
---
# <a name="fractionalpageitemview"></a><span data-ttu-id="36c26-103">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="36c26-103">FractionalPageItemView</span></span>

<span data-ttu-id="36c26-104">Элемент **FractionalPageItemView** описывается, где начала страничного представления и максимальное число элементов, возвращаемых в запросе [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="36c26-104">The **FractionalPageItemView** element describes where the paged view starts and the maximum number of items returned in a [FindItem](finditem.md) request.</span></span> 
  
[<span data-ttu-id="36c26-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="36c26-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="36c26-106">FractionalPageItemView</span><span class="sxs-lookup"><span data-stu-id="36c26-106">FractionalPageItemView</span></span>](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="36c26-107">**FractionalPageViewType**</span><span class="sxs-lookup"><span data-stu-id="36c26-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="36c26-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="36c26-108">Attributes and elements</span></span>

<span data-ttu-id="36c26-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="36c26-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="36c26-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="36c26-110">Attributes</span></span>

|<span data-ttu-id="36c26-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="36c26-111">**Attribute**</span></span>|<span data-ttu-id="36c26-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36c26-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="36c26-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="36c26-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="36c26-114">Определяет максимальное число результатов, возвращаемых в ответе [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="36c26-114">Identifies the maximum number of results to return in the [FindItem](finditem.md) response.</span></span> <span data-ttu-id="36c26-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="36c26-115">This attribute is optional.</span></span> <span data-ttu-id="36c26-116">Если этот атрибут не указан, вызов вернет все доступные элементы.</span><span class="sxs-lookup"><span data-stu-id="36c26-116">If this attribute is not specified, the call will return all available items.</span></span>  <br/> |
|<span data-ttu-id="36c26-117">**Числитель**</span><span class="sxs-lookup"><span data-stu-id="36c26-117">**Numerator**</span></span> <br/> |<span data-ttu-id="36c26-118">Представляет числитель дробная смещения от начала набора результатов.</span><span class="sxs-lookup"><span data-stu-id="36c26-118">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="36c26-119">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="36c26-119">This attribute is required.</span></span> <span data-ttu-id="36c26-120">Числитель должно быть равно или меньше, чем делителя.</span><span class="sxs-lookup"><span data-stu-id="36c26-120">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="36c26-121">Этот атрибут должен представлять целочисленное значение, которое равно или больше нуля.</span><span class="sxs-lookup"><span data-stu-id="36c26-121">This attribute must represent an integral value that is equal to or greater than zero.</span></span>  <br/> <span data-ttu-id="36c26-122">Дополнительные сведения см.</span><span class="sxs-lookup"><span data-stu-id="36c26-122">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="36c26-123">**Делителя**</span><span class="sxs-lookup"><span data-stu-id="36c26-123">**Denominator**</span></span> <br/> |<span data-ttu-id="36c26-124">Представляет делителя дробная смещением от начала общее число элементов в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="36c26-124">Represents the denominator of the fractional offset from the start of the total number of items in the result set.</span></span> <span data-ttu-id="36c26-125">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="36c26-125">This attribute is required.</span></span> <span data-ttu-id="36c26-126">Этот атрибут должен представлять целое число, которое больше одного.</span><span class="sxs-lookup"><span data-stu-id="36c26-126">This attribute must represent an integral value that is greater than one.</span></span>  <br/> <span data-ttu-id="36c26-127">Дополнительные сведения см.</span><span class="sxs-lookup"><span data-stu-id="36c26-127">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="36c26-128">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="36c26-128">Child elements</span></span>

<span data-ttu-id="36c26-129">Нет.</span><span class="sxs-lookup"><span data-stu-id="36c26-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="36c26-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="36c26-130">Parent elements</span></span>

|<span data-ttu-id="36c26-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="36c26-131">**Element**</span></span>|<span data-ttu-id="36c26-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="36c26-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="36c26-133">FindItem</span><span class="sxs-lookup"><span data-stu-id="36c26-133">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="36c26-134">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="36c26-134">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="36c26-135">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="36c26-135">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="36c26-136">Замечания</span><span class="sxs-lookup"><span data-stu-id="36c26-136">Remarks</span></span>

<span data-ttu-id="36c26-137">Смещение страничного представления от начала набора элементов, обнаруженные описывается функцией.</span><span class="sxs-lookup"><span data-stu-id="36c26-137">The paged view offset from the start of the set of found items is described by a fraction.</span></span> <span data-ttu-id="36c26-138">Дроби, которая определяется **числитель** и **делителя** атрибуты, описание которых начинается страницы сведений.</span><span class="sxs-lookup"><span data-stu-id="36c26-138">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="36c26-139">К примеру Если **числитель** равно четыре и **делителя** равно пять, страница возвращенных данных начинается запись находится четыре пятых длины способ в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="36c26-139">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="36c26-140">Если дроби равно нулю, это означает начала набора результатов.</span><span class="sxs-lookup"><span data-stu-id="36c26-140">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="36c26-141">Если дроби оценивается как одно, это означает конец набора результатов.</span><span class="sxs-lookup"><span data-stu-id="36c26-141">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="36c26-142">Дроби представляет начальную точку страницы, будут возвращены не число результатов в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="36c26-142">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="36c26-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="36c26-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="36c26-144">Пример</span><span class="sxs-lookup"><span data-stu-id="36c26-144">Example</span></span>

<span data-ttu-id="36c26-145">В следующем примере показано [FindItem](finditem.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="36c26-145">The following example shows a [FindItem](finditem.md) request.</span></span> <span data-ttu-id="36c26-146">Запрос возвращает элементы из результатов поиска, запустите после второй третья очередь элементы в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="36c26-146">The request returns items from the search results that start after the second third of all the items in the result set.</span></span> 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <FractionalPageItemView MaxEntriesReturned="12" Numerator="2" Denominator="3"/>
      <GroupBy Order="Descending">
        <t:FieldURI FieldURI="item:Importance"/>
        <t:AggregateOn Aggregate="Maximum">
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AggregateOn>
      </GroupBy>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="36c26-147">Например если результирующий набор содержит девяти элементов, постраничное представление возвращает до 12 элементов, начиная с элемента обнаруженного две трети способ в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="36c26-147">For example, if the result set contains nine items, the paged view will return up to 12 items, starting at the item found two-thirds of the way in to the result set.</span></span> <span data-ttu-id="36c26-148">В этом случае страница начинается в седьмой элемента.</span><span class="sxs-lookup"><span data-stu-id="36c26-148">In this case, the page starts at the seventh item.</span></span> <span data-ttu-id="36c26-149">Страница будет содержать седьмой восьмой и девятого элементов.</span><span class="sxs-lookup"><span data-stu-id="36c26-149">The page will contain the seventh, eighth, and ninth items.</span></span> <span data-ttu-id="36c26-150">Если числитель нулевое значение, просмотр страницы вернет все элементы в результирующем наборе, до тех пор, пока число меньше, чем атрибут **MaxEntriesReturned** .</span><span class="sxs-lookup"><span data-stu-id="36c26-150">If the numerator is set to zero, the page view will return all the items in the result set as long as the number is less than the **MaxEntriesReturned** attribute.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="36c26-151">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="36c26-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="36c26-152">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="36c26-152">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="36c26-153">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="36c26-153">Schema Name</span></span>  <br/> |<span data-ttu-id="36c26-154">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="36c26-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="36c26-155">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="36c26-155">Validation File</span></span>  <br/> |<span data-ttu-id="36c26-156">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="36c26-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="36c26-157">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="36c26-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="36c26-158">False</span><span class="sxs-lookup"><span data-stu-id="36c26-158">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="36c26-159">См. также</span><span class="sxs-lookup"><span data-stu-id="36c26-159">See also</span></span>



[<span data-ttu-id="36c26-160">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="36c26-160">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="36c26-161">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="36c26-161">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

