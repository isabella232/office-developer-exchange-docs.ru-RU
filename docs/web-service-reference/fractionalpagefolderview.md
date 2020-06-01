---
title: фрактионалпажефолдервиев
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
description: Элемент Фрактионалпажефолдервиев описывает, где начинается страничное представление, и максимальное число папок, возвращаемых в запросе FindFolder.
ms.openlocfilehash: a8627c6277b49655d3933679128b844118633cda
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463071"
---
# <a name="fractionalpagefolderview"></a><span data-ttu-id="903d1-103">фрактионалпажефолдервиев</span><span class="sxs-lookup"><span data-stu-id="903d1-103">FractionalPageFolderView</span></span>

<span data-ttu-id="903d1-104">Элемент **фрактионалпажефолдервиев** описывает, где начинается страничное представление, и максимальное число папок, возвращаемых в запросе [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="903d1-104">The **FractionalPageFolderView** element describes where the paged view starts and the maximum number of folders returned in a [FindFolder](findfolder.md) request.</span></span> 
  
[<span data-ttu-id="903d1-105">FindFolder</span><span class="sxs-lookup"><span data-stu-id="903d1-105">FindFolder</span></span>](findfolder.md)
  
[<span data-ttu-id="903d1-106">фрактионалпажефолдервиев</span><span class="sxs-lookup"><span data-stu-id="903d1-106">FractionalPageFolderView</span></span>](fractionalpagefolderview.md)
  
```xml
<FractionalPageFolderView MaxEntriesReturned="" Numerator="" Denominator=""/>
```

 <span data-ttu-id="903d1-107">**фрактионалпажевиевтипе**</span><span class="sxs-lookup"><span data-stu-id="903d1-107">**FractionalPageViewType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="903d1-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="903d1-108">Attributes and elements</span></span>

<span data-ttu-id="903d1-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="903d1-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="903d1-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="903d1-110">Attributes</span></span>

|<span data-ttu-id="903d1-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="903d1-111">**Attribute**</span></span>|<span data-ttu-id="903d1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="903d1-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="903d1-113">**максентриесретурнед**</span><span class="sxs-lookup"><span data-stu-id="903d1-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="903d1-114">Определяет максимальное число результатов, возвращаемых в ответе [FindFolder](findfolder.md) .</span><span class="sxs-lookup"><span data-stu-id="903d1-114">Identifies the maximum number of results to return in the [FindFolder](findfolder.md) response.</span></span> <span data-ttu-id="903d1-115">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="903d1-115">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="903d1-116">**Числител**</span><span class="sxs-lookup"><span data-stu-id="903d1-116">**Numerator**</span></span> <br/> |<span data-ttu-id="903d1-117">Представляет числитель дробного смещения от начала набора результатов.</span><span class="sxs-lookup"><span data-stu-id="903d1-117">Represents the numerator of the fractional offset from the start of the result set.</span></span> <span data-ttu-id="903d1-118">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="903d1-118">This attribute is required.</span></span> <span data-ttu-id="903d1-119">Числитель должен быть равен или меньше знаменателя.</span><span class="sxs-lookup"><span data-stu-id="903d1-119">The numerator must be equal to or less than the denominator.</span></span> <span data-ttu-id="903d1-120">Этот атрибут должен представлять целое значение, равное или больше 0.</span><span class="sxs-lookup"><span data-stu-id="903d1-120">This attribute must represent an integral value that is equal to or greater than zero.</span></span> <span data-ttu-id="903d1-121">Дополнительные сведения можно найти в разделе "Примечания" Далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="903d1-121">For more information, see Remarks later in this topic.</span></span>  <br/> |
|<span data-ttu-id="903d1-122">**Подробно**</span><span class="sxs-lookup"><span data-stu-id="903d1-122">**Denominator**</span></span> <br/> |<span data-ttu-id="903d1-123">Представляет знаменатель дробного смещения от начала общего числа папок в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="903d1-123">Represents the denominator of the fractional offset from the start of the total number of folders in the result set.</span></span> <span data-ttu-id="903d1-124">Этот атрибут является обязательным.</span><span class="sxs-lookup"><span data-stu-id="903d1-124">This attribute is required.</span></span> <span data-ttu-id="903d1-125">Этот атрибут должен представлять целое значение больше единицы.</span><span class="sxs-lookup"><span data-stu-id="903d1-125">This attribute must represent an integral value that is greater than one.</span></span> <span data-ttu-id="903d1-126">Дополнительные сведения можно найти в разделе "Примечания" Далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="903d1-126">For more information, see Remarks later in this topic.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="903d1-127">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="903d1-127">Child elements</span></span>

<span data-ttu-id="903d1-128">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="903d1-128">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="903d1-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="903d1-129">Parent elements</span></span>

|<span data-ttu-id="903d1-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="903d1-130">**Element**</span></span>|<span data-ttu-id="903d1-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="903d1-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="903d1-132">FindFolder</span><span class="sxs-lookup"><span data-stu-id="903d1-132">FindFolder</span></span>](findfolder.md) <br/> |<span data-ttu-id="903d1-133">Определяет запрос на идентификацию папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="903d1-133">Defines a request to identify folders in a mailbox.</span></span>  <br/> <span data-ttu-id="903d1-134">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="903d1-134">The following is the XPath expression to this element:</span></span>  <br/>  `/FindFolder` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="903d1-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="903d1-135">Remarks</span></span>

<span data-ttu-id="903d1-136">Смещение страничного представления от начала набора найденных папок описывается с помощью дробной части.</span><span class="sxs-lookup"><span data-stu-id="903d1-136">The paged view offset from the start of the set of found folders is described by a fraction.</span></span> <span data-ttu-id="903d1-137">Дробь, которая определяется атрибутами **числительного** и **знаменателя** , описывает, где начинается страница данных.</span><span class="sxs-lookup"><span data-stu-id="903d1-137">The fraction, which is defined by the **Numerator** and **Denominator** attributes, describes where the page of information starts.</span></span> <span data-ttu-id="903d1-138">Например, если **числитель** равен четырем и **знаменателю** равен 5, то страница возвращаемой информации начинается с записи, расположенной четырьмя-пятогоями способа в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="903d1-138">For example, if **Numerator** equals four and **Denominator** equals five, the page of returned information starts at an entry located four-fifths of the way in to the result set.</span></span> 
  
<span data-ttu-id="903d1-139">Если дробная дробь имеет нулевое значение, значит начало набора результатов.</span><span class="sxs-lookup"><span data-stu-id="903d1-139">If the fraction evaluates to zero, that indicates the start of the results set.</span></span> <span data-ttu-id="903d1-140">Если дробь имеет значение 1, то отображается конец набора результатов.</span><span class="sxs-lookup"><span data-stu-id="903d1-140">If the fraction evaluates to one, that indicates the end of the result set.</span></span>
  
> [!NOTE]
> <span data-ttu-id="903d1-141">Дробь представляет начальную точку страницы, а не количество результатов, возвращаемых в наборе результатов.</span><span class="sxs-lookup"><span data-stu-id="903d1-141">The fraction represents the start point of page, not how many results in the result set will be returned.</span></span> 
  
<span data-ttu-id="903d1-142">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="903d1-142">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="903d1-143">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="903d1-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="903d1-144">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="903d1-144">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="903d1-145">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="903d1-145">Schema Name</span></span>  <br/> |<span data-ttu-id="903d1-146">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="903d1-146">Messages schema</span></span>  <br/> |
|<span data-ttu-id="903d1-147">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="903d1-147">Validation File</span></span>  <br/> |<span data-ttu-id="903d1-148">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="903d1-148">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="903d1-149">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="903d1-149">Can be Empty</span></span>  <br/> |<span data-ttu-id="903d1-150">False</span><span class="sxs-lookup"><span data-stu-id="903d1-150">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="903d1-151">См. также</span><span class="sxs-lookup"><span data-stu-id="903d1-151">See also</span></span>



[<span data-ttu-id="903d1-152">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="903d1-152">FindFolder operation</span></span>](findfolder-operation.md)


[<span data-ttu-id="903d1-153">Поиск папок</span><span class="sxs-lookup"><span data-stu-id="903d1-153">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

