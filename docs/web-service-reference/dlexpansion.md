---
title: DLExpansion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: Элемент DLExpansion содержит массив почтовых ящиков, которые содержатся в списке рассылки.
ms.openlocfilehash: 06081b4aba761a7137f921b3bc1c8d6b2afab88c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762199"
---
# <a name="dlexpansion"></a><span data-ttu-id="8a588-103">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="8a588-103">DLExpansion</span></span>

<span data-ttu-id="8a588-104">Элемент **DLExpansion** содержит массив почтовых ящиков, которые содержатся в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="8a588-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="8a588-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="8a588-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="8a588-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8a588-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="8a588-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8a588-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="8a588-108">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="8a588-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="8a588-109">**ArrayOfDLExpansionType**</span><span class="sxs-lookup"><span data-stu-id="8a588-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8a588-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8a588-110">Attributes and elements</span></span>

<span data-ttu-id="8a588-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8a588-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8a588-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8a588-112">Attributes</span></span>

|<span data-ttu-id="8a588-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8a588-113">**Attribute**</span></span>|<span data-ttu-id="8a588-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a588-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8a588-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="8a588-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="8a588-116">Представляет следующий индекс, который необходимо использовать для следующего запроса при использовании индексированного страницы представления.</span><span class="sxs-lookup"><span data-stu-id="8a588-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="8a588-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="8a588-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="8a588-118">Представляет новое значение перечислителя использовать для следующего запроса при использовании просмотров страниц дроби.</span><span class="sxs-lookup"><span data-stu-id="8a588-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="8a588-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="8a588-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="8a588-120">Представляет Далее делителя будет использоваться для следующего запроса при использовании просмотров страниц дроби.</span><span class="sxs-lookup"><span data-stu-id="8a588-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="8a588-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="8a588-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="8a588-122">Указывает, содержат ли текущие результаты последнего элемента в запросе, чтобы дополнительные разбиение на страницы не требуется.</span><span class="sxs-lookup"><span data-stu-id="8a588-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="8a588-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="8a588-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="8a588-124">Представляет общее число элементов в представлении.</span><span class="sxs-lookup"><span data-stu-id="8a588-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8a588-125">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8a588-125">Child elements</span></span>

|<span data-ttu-id="8a588-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a588-126">**Element**</span></span>|<span data-ttu-id="8a588-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a588-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a588-128">Mailbox</span><span class="sxs-lookup"><span data-stu-id="8a588-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="8a588-129">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8a588-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8a588-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8a588-130">Parent elements</span></span>

|<span data-ttu-id="8a588-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8a588-131">**Element**</span></span>|<span data-ttu-id="8a588-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8a588-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8a588-133">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8a588-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="8a588-134">Содержит состояние и результат одного запроса ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="8a588-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8a588-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="8a588-135">Remarks</span></span>

<span data-ttu-id="8a588-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8a588-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8a588-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8a588-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8a588-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8a588-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8a588-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8a588-139">Schema Name</span></span>  <br/> |<span data-ttu-id="8a588-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8a588-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="8a588-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8a588-141">Validation File</span></span>  <br/> |<span data-ttu-id="8a588-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8a588-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8a588-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8a588-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="8a588-144">False</span><span class="sxs-lookup"><span data-stu-id="8a588-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8a588-145">См. также</span><span class="sxs-lookup"><span data-stu-id="8a588-145">See also</span></span>

- [<span data-ttu-id="8a588-146">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="8a588-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="8a588-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a588-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- [<span data-ttu-id="8a588-148">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="8a588-148">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

