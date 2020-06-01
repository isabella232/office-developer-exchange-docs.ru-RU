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
ms.openlocfilehash: 079ad1c0f114d201f5d1b91c3fd9bb45b943cc1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456999"
---
# <a name="dlexpansion"></a><span data-ttu-id="71bed-103">длекспансион</span><span class="sxs-lookup"><span data-stu-id="71bed-103">DLExpansion</span></span>

<span data-ttu-id="71bed-104">Элемент **длекспансион** содержит массив почтовых ящиков, содержащихся в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="71bed-104">The **DLExpansion** element contains an array of mailboxes that are contained in a distribution list.</span></span> 
  
- [<span data-ttu-id="71bed-105">експанддлреспонсе</span><span class="sxs-lookup"><span data-stu-id="71bed-105">ExpandDLResponse</span></span>](expanddlresponse.md) 
- [<span data-ttu-id="71bed-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="71bed-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="71bed-107">експанддлреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="71bed-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
- [<span data-ttu-id="71bed-108">длекспансион</span><span class="sxs-lookup"><span data-stu-id="71bed-108">DLExpansion</span></span>](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 <span data-ttu-id="71bed-109">**аррайофдлекспансионтипе**</span><span class="sxs-lookup"><span data-stu-id="71bed-109">**ArrayOfDLExpansionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71bed-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71bed-110">Attributes and elements</span></span>

<span data-ttu-id="71bed-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="71bed-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71bed-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="71bed-112">Attributes</span></span>

|<span data-ttu-id="71bed-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="71bed-113">**Attribute**</span></span>|<span data-ttu-id="71bed-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71bed-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="71bed-115">**индекседпагингоффсет**</span><span class="sxs-lookup"><span data-stu-id="71bed-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="71bed-116">Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления страницы.</span><span class="sxs-lookup"><span data-stu-id="71bed-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="71bed-117">**нумератороффсет**</span><span class="sxs-lookup"><span data-stu-id="71bed-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="71bed-118">Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений страницы дробей.</span><span class="sxs-lookup"><span data-stu-id="71bed-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="71bed-119">**абсолутеденоминатор**</span><span class="sxs-lookup"><span data-stu-id="71bed-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="71bed-120">Представляет следующий знаменатель, который будет использоваться для следующего запроса при использовании представлений страницы дробной части.</span><span class="sxs-lookup"><span data-stu-id="71bed-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="71bed-121">**инклудесластитеминранже**</span><span class="sxs-lookup"><span data-stu-id="71bed-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="71bed-122">Указывает, содержат ли текущие результаты последний элемент в запросе, чтобы не требовалось дополнительное разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="71bed-122">Indicates whether the current results contain the last item in the query so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="71bed-123">**тоталитемсинвиев**</span><span class="sxs-lookup"><span data-stu-id="71bed-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="71bed-124">Представляет общее число элементов в представлении.</span><span class="sxs-lookup"><span data-stu-id="71bed-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="71bed-125">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="71bed-125">Child elements</span></span>

|<span data-ttu-id="71bed-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71bed-126">**Element**</span></span>|<span data-ttu-id="71bed-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71bed-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71bed-128">Mailbox</span><span class="sxs-lookup"><span data-stu-id="71bed-128">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="71bed-129">Определяет объект службы каталогов с включенной поддержкой почты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="71bed-129">Identifies a mail-enabled Active Directory directory service object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71bed-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="71bed-130">Parent elements</span></span>

|<span data-ttu-id="71bed-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71bed-131">**Element**</span></span>|<span data-ttu-id="71bed-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71bed-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71bed-133">експанддлреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="71bed-133">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md) <br/> |<span data-ttu-id="71bed-134">Содержит состояние и результат одного запроса ExpandDL.</span><span class="sxs-lookup"><span data-stu-id="71bed-134">Contains the status and result of a single ExpandDL request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="71bed-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="71bed-135">Remarks</span></span>

<span data-ttu-id="71bed-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="71bed-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71bed-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="71bed-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71bed-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="71bed-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71bed-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="71bed-139">Schema Name</span></span>  <br/> |<span data-ttu-id="71bed-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="71bed-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="71bed-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="71bed-141">Validation File</span></span>  <br/> |<span data-ttu-id="71bed-142">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="71bed-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71bed-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="71bed-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="71bed-144">False</span><span class="sxs-lookup"><span data-stu-id="71bed-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71bed-145">См. также</span><span class="sxs-lookup"><span data-stu-id="71bed-145">See also</span></span>

- [<span data-ttu-id="71bed-146">Операция ExpandDL</span><span class="sxs-lookup"><span data-stu-id="71bed-146">ExpandDL operation</span></span>](expanddl-operation.md)
- [<span data-ttu-id="71bed-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="71bed-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md) 
- [<span data-ttu-id="71bed-148">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="71bed-148">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

