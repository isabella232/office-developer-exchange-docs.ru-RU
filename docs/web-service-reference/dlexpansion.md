---
title: длекспансион
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
description: Элемент Длекспансион содержит массив почтовых ящиков, содержащихся в списке рассылки.
ms.openlocfilehash: 06081b4aba761a7137f921b3bc1c8d6b2afab88c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762199"
---
# <a name="dlexpansion"></a><span data-ttu-id="754ca-103">длекспансион</span><span class="sxs-lookup"><span data-stu-id="754ca-103">DLExpansion</span></span>

<span data-ttu-id="754ca-104">Элемент **длекспансион** содержит массив почтовых ящиков, содержащихся в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="754ca-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="754ca-105">експанддлреспонсе</span><span class="sxs-lookup"><span data-stu-id="754ca-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="754ca-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="754ca-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="754ca-107">експанддлреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="754ca-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="754ca-108">длекспансион</span><span class="sxs-lookup"><span data-stu-id="754ca-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="754ca-109">**аррайофдлекспансионтипе**</span><span class="sxs-lookup"><span data-stu-id="754ca-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="754ca-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="754ca-110">Attributes and elements</span></span>

<span data-ttu-id="754ca-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="754ca-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="754ca-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="754ca-112">Attributes</span></span>

|<span data-ttu-id="754ca-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="754ca-113">**Attribute**</span></span>|<span data-ttu-id="754ca-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="754ca-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="754ca-115">**индекседпагингоффсет**</span><span class="sxs-lookup"><span data-stu-id="754ca-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="754ca-116">Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления страницы.</span><span class="sxs-lookup"><span data-stu-id="754ca-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="754ca-117">**нумератороффсет**</span><span class="sxs-lookup"><span data-stu-id="754ca-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="754ca-118">Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений страницы дробей.</span><span class="sxs-lookup"><span data-stu-id="754ca-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="754ca-119">**абсолутеденоминатор**</span><span class="sxs-lookup"><span data-stu-id="754ca-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="754ca-120">Представляет следующий знаменатель, который будет использоваться для следующего запроса при использовании представлений страницы дробной части.</span><span class="sxs-lookup"><span data-stu-id="754ca-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="754ca-121">**инклудесластитеминранже**</span><span class="sxs-lookup"><span data-stu-id="754ca-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="754ca-122">Указывает, содержат ли текущие результаты последний элемент в запросе, чтобы не требовалось дополнительное разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="754ca-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="754ca-123">**тоталитемсинвиев**</span><span class="sxs-lookup"><span data-stu-id="754ca-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="754ca-124">Представляет общее число элементов в представлении.</span><span class="sxs-lookup"><span data-stu-id="754ca-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="754ca-125">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="754ca-125">Child elements</span></span>

|<span data-ttu-id="754ca-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="754ca-126">**Element**</span></span>|<span data-ttu-id="754ca-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="754ca-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="754ca-128">Mailbox</span><span class="sxs-lookup"><span data-stu-id="754ca-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="754ca-129">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="754ca-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="754ca-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="754ca-130">Parent elements</span></span>

|<span data-ttu-id="754ca-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="754ca-131">**Element**</span></span>|<span data-ttu-id="754ca-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="754ca-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="754ca-133">експанддлреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="754ca-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="754ca-134">Содержит состояние и результат одного запроса ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="754ca-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="754ca-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="754ca-135">Remarks</span></span>

<span data-ttu-id="754ca-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="754ca-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="754ca-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="754ca-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="754ca-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="754ca-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="754ca-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="754ca-139">Schema Name</span></span>  <br/> |<span data-ttu-id="754ca-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="754ca-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="754ca-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="754ca-141">Validation File</span></span>  <br/> |<span data-ttu-id="754ca-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="754ca-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="754ca-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="754ca-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="754ca-144">False</span><span class="sxs-lookup"><span data-stu-id="754ca-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="754ca-145">См. также</span><span class="sxs-lookup"><span data-stu-id="754ca-145">See also</span></span>

- [<span data-ttu-id="754ca-146">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="754ca-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="754ca-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="754ca-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- [<span data-ttu-id="754ca-148">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="754ca-148">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

