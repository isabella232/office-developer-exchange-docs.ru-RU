---
title: Операция UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4
description: Операция UpdateItem используется для изменения свойств существующего элемента в хранилище Exchange.
ms.openlocfilehash: c001b7656862144023e9704cb04e6b4c0030f9df
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459393"
---
# <a name="updateitem-operation"></a><span data-ttu-id="a5aea-103">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a5aea-103">UpdateItem operation</span></span>

<span data-ttu-id="a5aea-104">Операция **UpdateItem** используется для изменения свойств существующего элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5aea-104">The **UpdateItem** operation is used to modify the properties of an existing item in the Exchange store.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a5aea-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="a5aea-105">Remarks</span></span>

<span data-ttu-id="a5aea-106">Для элемента можно выполнить три основные действия по обновлению.</span><span class="sxs-lookup"><span data-stu-id="a5aea-106">You can perform three basic update actions on an item.</span></span> <span data-ttu-id="a5aea-107">В следующей таблице перечислены действия, которые можно выполнить.</span><span class="sxs-lookup"><span data-stu-id="a5aea-107">The following table lists the actions that you can perform.</span></span>
  
|<span data-ttu-id="a5aea-108">**Действие**</span><span class="sxs-lookup"><span data-stu-id="a5aea-108">**Action**</span></span>|<span data-ttu-id="a5aea-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a5aea-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a5aea-110">Error</span><span class="sxs-lookup"><span data-stu-id="a5aea-110">Append</span></span>  <br/> |<span data-ttu-id="a5aea-111">Добавляет данные к существующему свойству.</span><span class="sxs-lookup"><span data-stu-id="a5aea-111">Adds data to an existing property.</span></span> <span data-ttu-id="a5aea-112">Это действие сохранит текущие данные.</span><span class="sxs-lookup"><span data-stu-id="a5aea-112">This action preserves the current data.</span></span> <span data-ttu-id="a5aea-113">Append не применяется ко всем свойствам.</span><span class="sxs-lookup"><span data-stu-id="a5aea-113">Append does not apply to all properties.</span></span>  <br/> |
|<span data-ttu-id="a5aea-114">Set</span><span class="sxs-lookup"><span data-stu-id="a5aea-114">Set</span></span>  <br/> |<span data-ttu-id="a5aea-115">Заменяет данные для свойства, если свойство содержит данные, или создает свойство и задает его значение, если свойство не существует.</span><span class="sxs-lookup"><span data-stu-id="a5aea-115">Replaces data for a property if the property contains data, or creates the property and sets its value if the property does not exist.</span></span> <span data-ttu-id="a5aea-116">Действие Set применяется только к записываемым свойствам.</span><span class="sxs-lookup"><span data-stu-id="a5aea-116">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="a5aea-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="a5aea-117">Delete</span></span>  <br/> |<span data-ttu-id="a5aea-118">Удаляет свойство из элемента.</span><span class="sxs-lookup"><span data-stu-id="a5aea-118">Removes a property from an item.</span></span> <span data-ttu-id="a5aea-119">Это отличается от присвоения свойству пустого значения.</span><span class="sxs-lookup"><span data-stu-id="a5aea-119">This differs from setting a property to an empty value.</span></span> <span data-ttu-id="a5aea-120">По завершении этого действия свойство для элемента не существует.</span><span class="sxs-lookup"><span data-stu-id="a5aea-120">When this action is finished, the property does not exist for the item.</span></span> <span data-ttu-id="a5aea-121">DELETE применяется только к записываемым свойствам.</span><span class="sxs-lookup"><span data-stu-id="a5aea-121">Delete is only applicable to writable properties.</span></span>  <br/> |
   
<span data-ttu-id="a5aea-122">Вызов **UpdateItem** можно использовать для изменения одного или нескольких элементов и одного или нескольких свойств каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="a5aea-122">An **UpdateItem** call can be used to modify one or more items, and one or more properties on each item.</span></span> <span data-ttu-id="a5aea-123">Элемент [итемчанжес](itemchanges.md) содержит все изменения, которые необходимо выполнить в рамках этого вызова.</span><span class="sxs-lookup"><span data-stu-id="a5aea-123">The [ItemChanges](itemchanges.md) element contains all the modifications that are to be performed as part of this call.</span></span> <span data-ttu-id="a5aea-124">Элемент [итемчанже](itemchange.md) , являющийся дочерним по отношению к элементу [итемчанжес](itemchanges.md) , представляет изменения, которые необходимо выполнить для одного элемента.</span><span class="sxs-lookup"><span data-stu-id="a5aea-124">The [ItemChange](itemchange.md) element, a child of the [ItemChanges](itemchanges.md) element, represents the modifications to be performed on a single item.</span></span> <span data-ttu-id="a5aea-125">Элемент [итемчанже](itemchange.md) содержит набор действий обновления, которые можно выполнить для одного элемента.</span><span class="sxs-lookup"><span data-stu-id="a5aea-125">The [ItemChange](itemchange.md) element contains a set of update actions that can be performed on a single item.</span></span> <span data-ttu-id="a5aea-126">Эти изменения включены в элемент [Updates (Item)](updates-item.md) .</span><span class="sxs-lookup"><span data-stu-id="a5aea-126">These changes are contained in the [Updates (Item)](updates-item.md) element.</span></span> <span data-ttu-id="a5aea-127">Элемент [ItemId](itemid.md) определяет обновляемый элемент.</span><span class="sxs-lookup"><span data-stu-id="a5aea-127">The [ItemId](itemid.md) element identifies the item to update.</span></span> <span data-ttu-id="a5aea-128">Чтобы обновить несколько свойств элемента, необходимо предоставить [сетитемфиелд](setitemfield.md), [аппендтоитемфиелд](appendtoitemfield.md)или [делетеитемфиелд](deleteitemfield.md) для каждого свойства, для которого требуется обновление.</span><span class="sxs-lookup"><span data-stu-id="a5aea-128">To update more than one property on an item, a [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md), or [DeleteItemField](deleteitemfield.md) must be provided for each property that requires the update.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a5aea-129">Действия по обновлению применяются в том порядке, в котором они указаны.</span><span class="sxs-lookup"><span data-stu-id="a5aea-129">Update actions are applied in the order in which they are specified.</span></span> 
  
<span data-ttu-id="a5aea-130">Для каждого изменения необходимо указать путь к свойству, которое необходимо изменить, и представление этого элемента с новым значением.</span><span class="sxs-lookup"><span data-stu-id="a5aea-130">For each change, you have to specify the path of the property to change and a representation of that item with its new value.</span></span> <span data-ttu-id="a5aea-131">Действие DELETE слегка отличается от того, что требуется только путь к удаляемому свойству.</span><span class="sxs-lookup"><span data-stu-id="a5aea-131">The delete action is slightly different in that only the path of the property that should be deleted is required.</span></span> <span data-ttu-id="a5aea-132">Для действий Set и Append указанный путь должен относиться к тому же свойству, которое задается в представлении элемента.</span><span class="sxs-lookup"><span data-stu-id="a5aea-132">For set and append actions, the path that is specified must refer to the same property that is being set in the item representation.</span></span> <span data-ttu-id="a5aea-133">Если они отличаются, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="a5aea-133">If these differ, an error will be returned.</span></span>
  
<span data-ttu-id="a5aea-134">Для операции **UpdateItem** можно задать время [начала](start.md) и [окончания](end-ex15websvcsotherref.md) для элемента хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="a5aea-134">The **UpdateItem** operation can set the [Start](start.md) and [End ](end-ex15websvcsotherref.md) time of an Exchange store item.</span></span> <span data-ttu-id="a5aea-135">В запросе **UpdateItem** время [начала](start.md) может быть задано без указания времени [окончания](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="a5aea-135">In an **UpdateItem** request, the [Start](start.md) time can be set without also setting the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="a5aea-136">Это может привести к ошибке, если время [начала](start.md) позже времени [окончания](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="a5aea-136">This can cause an error if the [Start](start.md) time is later than the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="a5aea-137">Имейте в виду, что клиентские приложения должны настроить время [окончания](end-ex15websvcsotherref.md) при изменении времени [начала](start.md) , чтобы сохранить длительность.</span><span class="sxs-lookup"><span data-stu-id="a5aea-137">Be aware that client applications must adjust the [End ](end-ex15websvcsotherref.md) time when the [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
<span data-ttu-id="a5aea-138">Когда один элемент календаря обновляется, чтобы стать повторяющимся элементом основного календаря, свойство [митингтимезоне](meetingtimezone.md) должно быть задано операцией **UpdateItem** для сохранения исходного часового пояса элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="a5aea-138">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) property must be set by the **UpdateItem** operation in order to preserve the calendar item's original time zone.</span></span> 
  
## <a name="setitemfield-request-example"></a><span data-ttu-id="a5aea-139">Пример запроса Сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-139">SetItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="a5aea-140">Description</span><span class="sxs-lookup"><span data-stu-id="a5aea-140">Description</span></span>

<span data-ttu-id="a5aea-141">В приведенном ниже примере запроса **UpdateItem** показано, как задать свойство "чувствительность" для элемента.</span><span class="sxs-lookup"><span data-stu-id="a5aea-141">The following example of an **UpdateItem** request shows how to set the sensitivity property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a5aea-142">Код</span><span class="sxs-lookup"><span data-stu-id="a5aea-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkb..." ChangeKey="CQAAABYAAAB..."/>
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Sensitivity"/>
              <t:Message>
                <t:Sensitivity>Normal</t:Sensitivity>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a5aea-143">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a5aea-143">Comments</span></span>

<span data-ttu-id="a5aea-144">Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a5aea-144">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="setitemfield-request-elements"></a><span data-ttu-id="a5aea-145">Элементы запроса Сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-145">SetItemField Request Elements</span></span>

<span data-ttu-id="a5aea-146">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5aea-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a5aea-147">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a5aea-147">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="a5aea-148">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="a5aea-148">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="a5aea-149">ItemChange</span><span class="sxs-lookup"><span data-stu-id="a5aea-149">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="a5aea-150">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a5aea-150">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="a5aea-151">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="a5aea-151">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="a5aea-152">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-152">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="a5aea-153">фиелдури</span><span class="sxs-lookup"><span data-stu-id="a5aea-153">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="a5aea-154">Сообщение</span><span class="sxs-lookup"><span data-stu-id="a5aea-154">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a5aea-155">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="a5aea-155">Sensitivity</span></span>](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a><span data-ttu-id="a5aea-156">Пример запроса Аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-156">AppendToItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="a5aea-157">Description</span><span class="sxs-lookup"><span data-stu-id="a5aea-157">Description</span></span>

<span data-ttu-id="a5aea-158">В приведенном ниже примере запроса **UpdateItem** показано, как добавить текст в свойство Body элемента.</span><span class="sxs-lookup"><span data-stu-id="a5aea-158">The following example of an **UpdateItem** request shows how to append text to the body property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a5aea-159">Код</span><span class="sxs-lookup"><span data-stu-id="a5aea-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYA..."/>
          <t:Updates>
            <t:AppendToItemField>
              <t:FieldURI FieldURI="item:Body"/>
              <t:Message>
                <t:Body BodyType="Text">Some additional text to append</t:Body>
              </t:Message>
            </t:AppendToItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a5aea-160">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a5aea-160">Comments</span></span>

<span data-ttu-id="a5aea-161">Действие Append поддерживается следующими свойствами:</span><span class="sxs-lookup"><span data-stu-id="a5aea-161">The following properties support the append action:</span></span>
  
- <span data-ttu-id="a5aea-162">**сообщение: ReplyTo**</span><span class="sxs-lookup"><span data-stu-id="a5aea-162">**message:ReplyTo**</span></span>
    
- <span data-ttu-id="a5aea-163">**элемент: Body**</span><span class="sxs-lookup"><span data-stu-id="a5aea-163">**item:Body**</span></span>
    
- <span data-ttu-id="a5aea-164">Все свойства коллекции получателей и участников</span><span class="sxs-lookup"><span data-stu-id="a5aea-164">All the recipient and attendee collection properties</span></span>
    
<span data-ttu-id="a5aea-165">Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a5aea-165">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="appendtoitemfield-request-elements"></a><span data-ttu-id="a5aea-166">Элементы запроса Аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-166">AppendToItemField Request Elements</span></span>

<span data-ttu-id="a5aea-167">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5aea-167">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a5aea-168">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a5aea-168">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="a5aea-169">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="a5aea-169">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="a5aea-170">ItemChange</span><span class="sxs-lookup"><span data-stu-id="a5aea-170">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="a5aea-171">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a5aea-171">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="a5aea-172">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="a5aea-172">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="a5aea-173">аппендтоитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-173">AppendToItemField</span></span>](appendtoitemfield.md)
    
- [<span data-ttu-id="a5aea-174">фиелдури</span><span class="sxs-lookup"><span data-stu-id="a5aea-174">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="a5aea-175">Сообщение</span><span class="sxs-lookup"><span data-stu-id="a5aea-175">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a5aea-176">Body</span><span class="sxs-lookup"><span data-stu-id="a5aea-176">Body</span></span>](body.md)
    
## <a name="deleteitemfield-request-example"></a><span data-ttu-id="a5aea-177">Пример запроса Делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-177">DeleteItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="a5aea-178">Description</span><span class="sxs-lookup"><span data-stu-id="a5aea-178">Description</span></span>

<span data-ttu-id="a5aea-179">В следующем примере запроса **UpdateItem** показано, как удалить свойство элемента.</span><span class="sxs-lookup"><span data-stu-id="a5aea-179">The following example of an **UpdateItem** request shows how to delete a property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a5aea-180">Код</span><span class="sxs-lookup"><span data-stu-id="a5aea-180">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEFkbWluaXN0cm..." ChangeKey="CQAAABYAA..."/>
          <t:Updates>
            <t:DeleteItemField>
              <t:FieldURI FieldURI="item:Body"/>
            </t:DeleteItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a5aea-181">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a5aea-181">Comments</span></span>

<span data-ttu-id="a5aea-182">Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a5aea-182">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="deleteitemfield-request-elements"></a><span data-ttu-id="a5aea-183">Элементы запроса Делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-183">DeleteItemField Request Elements</span></span>

<span data-ttu-id="a5aea-184">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5aea-184">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a5aea-185">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="a5aea-185">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="a5aea-186">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="a5aea-186">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="a5aea-187">ItemChange</span><span class="sxs-lookup"><span data-stu-id="a5aea-187">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="a5aea-188">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a5aea-188">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="a5aea-189">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="a5aea-189">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="a5aea-190">делетеитемфиелд</span><span class="sxs-lookup"><span data-stu-id="a5aea-190">DeleteItemField</span></span>](deleteitemfield.md)
    
- [<span data-ttu-id="a5aea-191">фиелдури</span><span class="sxs-lookup"><span data-stu-id="a5aea-191">FieldURI</span></span>](fielduri.md)
    
## <a name="successful-response-example"></a><span data-ttu-id="a5aea-192">Пример успешного ответа</span><span class="sxs-lookup"><span data-stu-id="a5aea-192">Successful response example</span></span>

### <a name="description"></a><span data-ttu-id="a5aea-193">Description</span><span class="sxs-lookup"><span data-stu-id="a5aea-193">Description</span></span>

<span data-ttu-id="a5aea-194">В следующем примере показан успешный ответ на запрос **UpdateItem** .</span><span class="sxs-lookup"><span data-stu-id="a5aea-194">The following example shows a successful response to an **UpdateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a5aea-195">Код</span><span class="sxs-lookup"><span data-stu-id="a5aea-195">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAAtAEFkbW..." ChangeKey="CQAAABYAAA..."/>
            </t:Message>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a5aea-196">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a5aea-196">Comments</span></span>

<span data-ttu-id="a5aea-197">Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a5aea-197">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="a5aea-198">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="a5aea-198">Successful response elements</span></span>

<span data-ttu-id="a5aea-199">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a5aea-199">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a5aea-200">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="a5aea-200">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a5aea-201">упдатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="a5aea-201">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="a5aea-202">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="a5aea-202">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a5aea-203">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a5aea-203">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="a5aea-204">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a5aea-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a5aea-205">Items</span><span class="sxs-lookup"><span data-stu-id="a5aea-205">Items</span></span>](items.md)
    
- [<span data-ttu-id="a5aea-206">Сообщение</span><span class="sxs-lookup"><span data-stu-id="a5aea-206">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a5aea-207">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="a5aea-207">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="a5aea-208">См. также</span><span class="sxs-lookup"><span data-stu-id="a5aea-208">See also</span></span>



[<span data-ttu-id="a5aea-209">Операция UpdateItem (Task)</span><span class="sxs-lookup"><span data-stu-id="a5aea-209">UpdateItem operation (task)</span></span>](updateitem-operation-task.md)
  
[<span data-ttu-id="a5aea-210">Операция UpdateItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="a5aea-210">UpdateItem operation (contact)</span></span>](updateitem-operation-contact.md)


- [<span data-ttu-id="a5aea-211">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a5aea-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="a5aea-212">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="a5aea-212">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="a5aea-213">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="a5aea-213">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

