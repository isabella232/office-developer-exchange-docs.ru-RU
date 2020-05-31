---
title: аппендтоитемфиелд
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: Элемент Аппендтоитемфиелд определяет данные, добавляемые к одному свойству элемента во время операции UpdateItem.
ms.openlocfilehash: b432399e84ee4a3fd7edc5d3f803079435c79143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761396"
---
# <a name="appendtoitemfield"></a><span data-ttu-id="6dda0-103">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="6dda0-103">AppendToItemField</span></span>

<span data-ttu-id="6dda0-104">Элемент **аппендтоитемфиелд** определяет данные, добавляемые к одному свойству элемента во время [операции UpdateItem](updateitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="6dda0-104">The **AppendToItemField** element identifies data to append to a single property of an item during an [UpdateItem operation](updateitem-operation.md).</span></span>
  
- [<span data-ttu-id="6dda0-105">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="6dda0-105">UpdateItem</span></span>](updateitem.md)
  
- [<span data-ttu-id="6dda0-106">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="6dda0-106">ItemChanges</span></span>](itemchanges.md)
  
- [<span data-ttu-id="6dda0-107">ItemChange</span><span class="sxs-lookup"><span data-stu-id="6dda0-107">ItemChange</span></span>](itemchange.md)
  
- [<span data-ttu-id="6dda0-108">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="6dda0-108">Updates (Item)</span></span>](updates-item.md)
  
- [<span data-ttu-id="6dda0-109">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="6dda0-109">AppendToItemField</span></span>](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 <span data-ttu-id="6dda0-110">**аппендтоитемфиелдтипе**</span><span class="sxs-lookup"><span data-stu-id="6dda0-110">**AppendToItemFieldType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6dda0-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6dda0-111">Attributes and elements</span></span>

<span data-ttu-id="6dda0-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6dda0-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6dda0-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6dda0-113">Attributes</span></span>

<span data-ttu-id="6dda0-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="6dda0-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6dda0-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6dda0-115">Child elements</span></span>

|<span data-ttu-id="6dda0-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6dda0-116">**Element**</span></span>|<span data-ttu-id="6dda0-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6dda0-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dda0-118">фиелдури</span><span class="sxs-lookup"><span data-stu-id="6dda0-118">FieldURI</span></span>](fielduri.md) <br/> |<span data-ttu-id="6dda0-119">Определяет часто упоминаемые свойства по URI.</span><span class="sxs-lookup"><span data-stu-id="6dda0-119">Identifies frequently referenced properties by URI.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-120">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="6dda0-120">IndexedFieldURI</span></span>](indexedfielduri.md) <br/> |<span data-ttu-id="6dda0-121">Определяет отдельные элементы словаря.</span><span class="sxs-lookup"><span data-stu-id="6dda0-121">Identifies individual members of a dictionary.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-122">екстендедфиелдури</span><span class="sxs-lookup"><span data-stu-id="6dda0-122">ExtendedFieldURI</span></span>](extendedfielduri.md) <br/> |<span data-ttu-id="6dda0-123">Указывает расширенные свойства MAPI, которые требуется добавить.</span><span class="sxs-lookup"><span data-stu-id="6dda0-123">Identifies extended MAPI properties to append.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-124">Элемент</span><span class="sxs-lookup"><span data-stu-id="6dda0-124">Item</span></span>](item.md) <br/> |<span data-ttu-id="6dda0-125">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-125">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-126">Message</span><span class="sxs-lookup"><span data-stu-id="6dda0-126">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="6dda0-127">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-127">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-128">календаритем</span><span class="sxs-lookup"><span data-stu-id="6dda0-128">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="6dda0-129">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-129">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-130">Контакт</span><span class="sxs-lookup"><span data-stu-id="6dda0-130">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="6dda0-131">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-131">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-132">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="6dda0-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="6dda0-133">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="6dda0-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-134">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="6dda0-134">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="6dda0-135">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-135">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-136">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="6dda0-136">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="6dda0-137">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-137">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-138">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="6dda0-138">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="6dda0-139">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-139">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-140">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="6dda0-140">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="6dda0-141">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-141">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="6dda0-142">Задача</span><span class="sxs-lookup"><span data-stu-id="6dda0-142">Task</span></span>](task.md) <br/> |<span data-ttu-id="6dda0-143">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6dda0-143">Represents a task in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6dda0-144">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6dda0-144">Parent elements</span></span>

|<span data-ttu-id="6dda0-145">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6dda0-145">**Element**</span></span>|<span data-ttu-id="6dda0-146">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6dda0-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6dda0-147">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="6dda0-147">Updates (Item)</span></span>](updates-item.md) <br/> |<span data-ttu-id="6dda0-148">Содержит массив, определяющий Добавление, установку и удаление изменений свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="6dda0-148">Contains an array that defines append, set, and delete changes to item properties.</span></span>  <br/> <span data-ttu-id="6dda0-149">Ниже приведено выражение XPath для этого элемента:`/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span><span class="sxs-lookup"><span data-stu-id="6dda0-149">The following is the XPath expression to this element:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates`</span></span> <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6dda0-150">Примечания</span><span class="sxs-lookup"><span data-stu-id="6dda0-150">Remarks</span></span>

<span data-ttu-id="6dda0-151">Операции добавления поддерживаются только для определенных свойств.</span><span class="sxs-lookup"><span data-stu-id="6dda0-151">Only certain properties support append operations.</span></span> <span data-ttu-id="6dda0-152">Попытка добавиться к свойству, которое не поддерживает добавление, приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="6dda0-152">An attempt to append to a property that does not support appending will result in an error.</span></span>
  
<span data-ttu-id="6dda0-153">Для операций обновления в одном запросе можно изменить только одно свойство.</span><span class="sxs-lookup"><span data-stu-id="6dda0-153">For update operations, only one property can be modified within a single request.</span></span> <span data-ttu-id="6dda0-154">В элементе [path](path.md) необходимо ссылаться на единственное свойство.</span><span class="sxs-lookup"><span data-stu-id="6dda0-154">That single property must be referenced in the [Path](path.md) element.</span></span> <span data-ttu-id="6dda0-155">В этом случае элемент **Item** в производных классах может хранить только одно свойство в соглашении с одним элементом **path** .</span><span class="sxs-lookup"><span data-stu-id="6dda0-155">The **Item** element in the derived classes can then only hold a single property that is in agreement with the single **Path** element.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6dda0-156">Элемент [path](path.md) является абстрактным.</span><span class="sxs-lookup"><span data-stu-id="6dda0-156">The [Path](path.md) element is abstract.</span></span> <span data-ttu-id="6dda0-157">Он должен быть замещен элементом [фиелдури](fielduri.md), [индекседфиелдури](indexedfielduri.md)или [екстендедфиелдури](extendedfielduri.md) .</span><span class="sxs-lookup"><span data-stu-id="6dda0-157">It must be substituted by the [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md), or [ExtendedFieldURI](extendedfielduri.md) element.</span></span> 
  
<span data-ttu-id="6dda0-158">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6dda0-158">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6dda0-159">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6dda0-159">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6dda0-160">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6dda0-160">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6dda0-161">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6dda0-161">Schema Name</span></span>  <br/> |<span data-ttu-id="6dda0-162">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6dda0-162">Types schema</span></span>  <br/> |
|<span data-ttu-id="6dda0-163">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6dda0-163">Validation File</span></span>  <br/> |<span data-ttu-id="6dda0-164">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="6dda0-164">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6dda0-165">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6dda0-165">Can be Empty</span></span>  <br/> |<span data-ttu-id="6dda0-166">False</span><span class="sxs-lookup"><span data-stu-id="6dda0-166">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6dda0-167">См. также</span><span class="sxs-lookup"><span data-stu-id="6dda0-167">See also</span></span>

- [<span data-ttu-id="6dda0-168">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="6dda0-168">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="6dda0-169">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6dda0-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

