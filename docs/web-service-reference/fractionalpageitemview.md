---
title: фрактионалпажеитемвиев
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
description: Элемент Фрактионалпажеитемвиев описывает, где начинается страничное представление, и максимальное количество элементов, возвращаемых в запросе FindItem.
ms.openlocfilehash: cbf45838558873dc5846823c2d1b26cf2c8af514
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461312"
---
# <a name="fractionalpageitemview"></a><span data-ttu-id="e04d6-103">фрактионалпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="e04d6-103">FractionalPageItemView</span></span>

<span data-ttu-id="e04d6-104">Элемент **фрактионалпажеитемвиев** описывает, где начинается страничное представление, и максимальное количество элементов, возвращаемых в запросе [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="e04d6-104">The **FractionalPageItemView** element describes where the paged view starts and the maximum number of items returned in a [FindItem](finditem.md) request.</span></span> 
  
[<span data-ttu-id="e04d6-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="e04d6-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="e04d6-106">фрактионалпажеитемвиев</span><span class="sxs-lookup"><span data-stu-id="e04d6-106">FractionalPageItemView</span></span>](fractionalpageitemview.md)
  
```xml
<FractionalPageItemView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="e04d6-107">**фрактионалпажевиевтипе**</span><span class="sxs-lookup"><span data-stu-id="e04d6-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e04d6-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e04d6-108">Attributes and elements</span></span>

<span data-ttu-id="e04d6-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e04d6-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e04d6-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e04d6-110">Attributes</span></span>

|<span data-ttu-id="e04d6-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e04d6-111">**Attribute**</span></span>|<span data-ttu-id="e04d6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e04d6-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e04d6-113">**максентриесретурнед**</span><span class="sxs-lookup"><span data-stu-id="e04d6-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="e04d6-114">Определяет максимальное число результатов, возвращаемых в ответе [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="e04d6-114">Identifies the maximum number of results to return in the [FindItem](finditem.md) response.</span></span> <span data-ttu-id="e04d6-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="e04d6-115">This attribute is optional.</span></span> <span data-ttu-id="e04d6-116">Если этот атрибут не указан, вызов возвратит все доступные элементы.</span><span class="sxs-lookup"><span data-stu-id="e04d6-116">If this attribute is not specified, the call will return all available items.</span></span>  <br/> |
|<span data-ttu-id="e04d6-117">**Числител**</span><span class="sxs-lookup"><span data-stu-id="e04d6-117">**Numerator**</span></span> <br/> |<span data-ttu-id="e04d6-118">Представляет числитель дробного смещения от начала набора результатов.</span><span class="sxs-lookup"><span data-stu-id="e04d6-118">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="e04d6-119">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e04d6-119">This attribute is required.</span></span> <span data-ttu-id="e04d6-120">Числитель должен быть равен или меньше знаменателя.</span><span class="sxs-lookup"><span data-stu-id="e04d6-120">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="e04d6-121">Этот атрибут должен представлять целое значение, равное или больше 0.</span><span class="sxs-lookup"><span data-stu-id="e04d6-121">This attribute must represent an integral value that is equal to or greater than zero.</span></span>  <br/> <span data-ttu-id="e04d6-122">Дополнительные сведения можно найти в разделе "Примечания" Далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="e04d6-122">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="e04d6-123">**Подробно**</span><span class="sxs-lookup"><span data-stu-id="e04d6-123">**Denominator**</span></span> <br/> |<span data-ttu-id="e04d6-124">Представляет знаменатель дробного смещения от начала общего числа элементов в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="e04d6-124">Represents the denominator of the fractional offset from the start of the total number of items in the result set.</span></span> <span data-ttu-id="e04d6-125">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e04d6-125">This attribute is required.</span></span> <span data-ttu-id="e04d6-126">Этот атрибут должен представлять целое значение больше единицы.</span><span class="sxs-lookup"><span data-stu-id="e04d6-126">This attribute must represent an integral value that is greater than one.</span></span>  <br/> <span data-ttu-id="e04d6-127">Дополнительные сведения можно найти в разделе "Примечания" Далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="e04d6-127">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e04d6-128">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e04d6-128">Child elements</span></span>

<span data-ttu-id="e04d6-129">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e04d6-129">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e04d6-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e04d6-130">Parent elements</span></span>

|<span data-ttu-id="e04d6-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e04d6-131">**Element**</span></span>|<span data-ttu-id="e04d6-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e04d6-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e04d6-133">FindItem</span><span class="sxs-lookup"><span data-stu-id="e04d6-133">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="e04d6-134">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e04d6-134">Defines a request to find items in a mailbox.</span></span>  <br/> <span data-ttu-id="e04d6-135">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e04d6-135">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e04d6-136">Примечания</span><span class="sxs-lookup"><span data-stu-id="e04d6-136">Remarks</span></span>

<span data-ttu-id="e04d6-137">Смещение страничного представления от начала набора найденных элементов описывается с помощью дробной части.</span><span class="sxs-lookup"><span data-stu-id="e04d6-137">The paged view offset from the start of the set of found items is described by a fraction.</span></span> <span data-ttu-id="e04d6-138">Дробь, которая определяется атрибутами **числительного** и **знаменателя** , описывает, где начинается страница данных.</span><span class="sxs-lookup"><span data-stu-id="e04d6-138">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="e04d6-139">Например, если **числитель** равен четырем и **знаменателю** равен 5, то страница возвращаемой информации начинается с записи, расположенной четырьмя-пятогоями способа в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="e04d6-139">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="e04d6-140">Если дробная дробь имеет нулевое значение, значит начало набора результатов.</span><span class="sxs-lookup"><span data-stu-id="e04d6-140">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="e04d6-141">Если дробь имеет значение 1, то отображается конец набора результатов.</span><span class="sxs-lookup"><span data-stu-id="e04d6-141">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="e04d6-142">Дробь представляет начальную точку страницы, а не количество результатов, возвращаемых в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="e04d6-142">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="e04d6-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e04d6-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="e04d6-144">Пример</span><span class="sxs-lookup"><span data-stu-id="e04d6-144">Example</span></span>

<span data-ttu-id="e04d6-145">В приведенном ниже примере показан запрос [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="e04d6-145">The following example shows a [FindItem](finditem.md) request.</span></span> <span data-ttu-id="e04d6-146">Запрос возвращает элементы из результатов поиска, которые начинаются после второй третьей части всех элементов в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="e04d6-146">The request returns items from the search results that start after the second third of all the items in the result set.</span></span> 
  
```
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="e04d6-147">Например, если результирующий набор содержит девять элементов, то Постраничное представление будет возвращать до 12 элементов, начиная с элемента, который находится в двух третьихх в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="e04d6-147">For example, if the result set contains nine items, the paged view will return up to 12 items, starting at the item found two-thirds of the way in to the result set.</span></span> <span data-ttu-id="e04d6-148">В этом случае страница начинается с седьмого элемента.</span><span class="sxs-lookup"><span data-stu-id="e04d6-148">In this case, the page starts at the seventh item.</span></span> <span data-ttu-id="e04d6-149">На странице будут содержаться седьмые, восьмые и девятые элементы.</span><span class="sxs-lookup"><span data-stu-id="e04d6-149">The page will contain the seventh, eighth, and ninth items.</span></span> <span data-ttu-id="e04d6-150">Если для числителя задано значение 0, то представление страницы будет возвращать все элементы в наборе результатов, если оно меньше, чем значение атрибута **максентриесретурнед** .</span><span class="sxs-lookup"><span data-stu-id="e04d6-150">If the numerator is set to zero, the page view will return all the items in the result set as long as the number is less than the **MaxEntriesReturned** attribute.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e04d6-151">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e04d6-151">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e04d6-152">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e04d6-152">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e04d6-153">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e04d6-153">Schema Name</span></span>  <br/> |<span data-ttu-id="e04d6-154">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e04d6-154">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e04d6-155">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e04d6-155">Validation File</span></span>  <br/> |<span data-ttu-id="e04d6-156">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e04d6-156">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e04d6-157">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e04d6-157">Can be Empty</span></span>  <br/> |<span data-ttu-id="e04d6-158">False</span><span class="sxs-lookup"><span data-stu-id="e04d6-158">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e04d6-159">См. также</span><span class="sxs-lookup"><span data-stu-id="e04d6-159">See also</span></span>



[<span data-ttu-id="e04d6-160">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="e04d6-160">FindItem operation</span></span>](finditem-operation.md)


[<span data-ttu-id="e04d6-161">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="e04d6-161">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

