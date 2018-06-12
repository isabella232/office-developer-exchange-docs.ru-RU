---
title: UpdateItem Operation
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
ms.openlocfilehash: 009ba16315017c4418fbd71d49744015c4d6d1b1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840353"
---
# <a name="updateitem-operation"></a><span data-ttu-id="ab3de-103">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="ab3de-103">UpdateItem operation</span></span>

<span data-ttu-id="ab3de-104">Операция **UpdateItem** используется для изменения свойств существующего элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab3de-104">The **UpdateItem** operation is used to modify the properties of an existing item in the Exchange store.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ab3de-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="ab3de-105">Remarks</span></span>

<span data-ttu-id="ab3de-106">Можно выполнить три основные обновления действия над элементом.</span><span class="sxs-lookup"><span data-stu-id="ab3de-106">You can perform three basic update actions on an item.</span></span> <span data-ttu-id="ab3de-107">В следующей таблице перечислены действия, которые можно выполнить.</span><span class="sxs-lookup"><span data-stu-id="ab3de-107">The following table lists the actions that you can perform.</span></span>
  
|<span data-ttu-id="ab3de-108">**Действие**</span><span class="sxs-lookup"><span data-stu-id="ab3de-108">**Action**</span></span>|<span data-ttu-id="ab3de-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ab3de-109">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ab3de-110">Добавление</span><span class="sxs-lookup"><span data-stu-id="ab3de-110">Append</span></span>  <br/> |<span data-ttu-id="ab3de-111">Добавляет данные существующего свойства.</span><span class="sxs-lookup"><span data-stu-id="ab3de-111">Adds data to an existing property.</span></span> <span data-ttu-id="ab3de-112">Это действие сохраняет текущих данных.</span><span class="sxs-lookup"><span data-stu-id="ab3de-112">This action preserves the current data.</span></span> <span data-ttu-id="ab3de-113">Добавьте не применяется ко всем свойствам.</span><span class="sxs-lookup"><span data-stu-id="ab3de-113">Append does not apply to all properties.</span></span>  <br/> |
|<span data-ttu-id="ab3de-114">Set</span><span class="sxs-lookup"><span data-stu-id="ab3de-114">Set</span></span>  <br/> |<span data-ttu-id="ab3de-115">Заменяет данных для свойства, если свойство содержит данные, или создает свойство и задает его значение, если свойство не существует.</span><span class="sxs-lookup"><span data-stu-id="ab3de-115">Replaces data for a property if the property contains data, or creates the property and sets its value if the property does not exist.</span></span> <span data-ttu-id="ab3de-116">Набор действий применима только для записи свойств.</span><span class="sxs-lookup"><span data-stu-id="ab3de-116">The set action is only applicable to writable properties.</span></span>  <br/> |
|<span data-ttu-id="ab3de-117">Удаление</span><span class="sxs-lookup"><span data-stu-id="ab3de-117">Delete</span></span>  <br/> |<span data-ttu-id="ab3de-118">Удаляет свойство из элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3de-118">Removes a property from an item.</span></span> <span data-ttu-id="ab3de-119">Это отличается от свойства пустое значение.</span><span class="sxs-lookup"><span data-stu-id="ab3de-119">This differs from setting a property to an empty value.</span></span> <span data-ttu-id="ab3de-120">По завершении этого действия свойство не существует для элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3de-120">When this action is finished, the property does not exist for the item.</span></span> <span data-ttu-id="ab3de-121">Удалить применима только для записи свойств.</span><span class="sxs-lookup"><span data-stu-id="ab3de-121">Delete is only applicable to writable properties.</span></span>  <br/> |
   
<span data-ttu-id="ab3de-122">Вызова **UpdateItem** можно использовать для изменения одного или нескольких элементов и одного или нескольких свойств каждого элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3de-122">An **UpdateItem** call can be used to modify one or more items, and one or more properties on each item.</span></span> <span data-ttu-id="ab3de-123">Элемент [ItemChanges](itemchanges.md) содержит все изменения, которые нужно выполнить в ходе вызова.</span><span class="sxs-lookup"><span data-stu-id="ab3de-123">The [ItemChanges](itemchanges.md) element contains all the modifications that are to be performed as part of this call.</span></span> <span data-ttu-id="ab3de-124">Элемент [ItemChange](itemchange.md) , дочерний элемент [ItemChanges](itemchanges.md) представляет изменения выполняется на один элемент.</span><span class="sxs-lookup"><span data-stu-id="ab3de-124">The [ItemChange](itemchange.md) element, a child of the [ItemChanges](itemchanges.md) element, represents the modifications to be performed on a single item.</span></span> <span data-ttu-id="ab3de-125">Элемент [ItemChange](itemchange.md) содержит набор действия обновления, доступные для отдельных элементов.</span><span class="sxs-lookup"><span data-stu-id="ab3de-125">The [ItemChange](itemchange.md) element contains a set of update actions that can be performed on a single item.</span></span> <span data-ttu-id="ab3de-126">Эти изменения содержащиеся в элементе [обновлений (элемент)](updates-item.md) .</span><span class="sxs-lookup"><span data-stu-id="ab3de-126">These changes are contained in the [Updates (Item)](updates-item.md) element.</span></span> <span data-ttu-id="ab3de-127">Элемент [ItemId](itemid.md) определяет элемент требуется обновить.</span><span class="sxs-lookup"><span data-stu-id="ab3de-127">The [ItemId](itemid.md) element identifies the item to update.</span></span> <span data-ttu-id="ab3de-128">Чтобы обновить более одного свойства элемента, [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md)или [DeleteItemField](deleteitemfield.md) должно быть указано для каждого свойства, которое требуется обновление.</span><span class="sxs-lookup"><span data-stu-id="ab3de-128">To update more than one property on an item, a [SetItemField](setitemfield.md), [AppendToItemField](appendtoitemfield.md), or [DeleteItemField](deleteitemfield.md) must be provided for each property that requires the update.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="ab3de-129">Действия Update, применяются в том порядке, в котором они указаны.</span><span class="sxs-lookup"><span data-stu-id="ab3de-129">Update actions are applied in the order in which they are specified.</span></span> 
  
<span data-ttu-id="ab3de-130">Для каждого изменения необходимо указать путь к свойству для изменения и представление такого элемента с его новое значение.</span><span class="sxs-lookup"><span data-stu-id="ab3de-130">For each change, you have to specify the path of the property to change and a representation of that item with its new value.</span></span> <span data-ttu-id="ab3de-131">Удаление несколько отличается, в том, что является обязательным только путь свойства, подлежащего удалению.</span><span class="sxs-lookup"><span data-stu-id="ab3de-131">The delete action is slightly different in that only the path of the property that should be deleted is required.</span></span> <span data-ttu-id="ab3de-132">Для набора и добавления действия, должен указывать путь, указанный для одного свойства, которое задано в представление элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3de-132">For set and append actions, the path that is specified must refer to the same property that is being set in the item representation.</span></span> <span data-ttu-id="ab3de-133">Если они отличаются, будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="ab3de-133">If these differ, an error will be returned.</span></span>
  
<span data-ttu-id="ab3de-134">Операция **UpdateItem** можно задать время [Start](start.md) и [End](end-ex15websvcsotherref.md) объекта хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="ab3de-134">The **UpdateItem** operation can set the [Start](start.md) and [End ](end-ex15websvcsotherref.md) time of an Exchange store item.</span></span> <span data-ttu-id="ab3de-135">В запросе **UpdateItem** можно задать время [начала](start.md) без предоставления время [окончания](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="ab3de-135">In an **UpdateItem** request, the [Start](start.md) time can be set without also setting the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="ab3de-136">Это может вызвать ошибку, если время [начала](start.md) позднее время [окончания](end-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="ab3de-136">This can cause an error if the [Start](start.md) time is later than the [End ](end-ex15websvcsotherref.md) time.</span></span> <span data-ttu-id="ab3de-137">Обратите внимание, что клиентских приложений необходимо настроить время [окончания](end-ex15websvcsotherref.md) , при изменении время [начала](start.md) для сохранения во время выполнения.</span><span class="sxs-lookup"><span data-stu-id="ab3de-137">Be aware that client applications must adjust the [End ](end-ex15websvcsotherref.md) time when the [Start](start.md) time is changed in order to preserve the duration.</span></span> 
  
<span data-ttu-id="ab3de-138">При обновлении элемента одного календаря стать повторяющегося элемента календаря главных свойство [MeetingTimeZone](meetingtimezone.md) должно быть задано при операции **UpdateItem** для сохранения часового пояса исходного элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="ab3de-138">When a single calendar item is updated to become a recurring master calendar item, the [MeetingTimeZone](meetingtimezone.md) property must be set by the **UpdateItem** operation in order to preserve the calendar item's original time zone.</span></span> 
  
## <a name="setitemfield-request-example"></a><span data-ttu-id="ab3de-139">Пример запроса SetItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-139">SetItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="ab3de-140">Описание</span><span class="sxs-lookup"><span data-stu-id="ab3de-140">Description</span></span>

<span data-ttu-id="ab3de-141">Приведенный ниже запрос **UpdateItem** показано, как задать свойство уровень конфиденциальности сообщения элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3de-141">The following example of an **UpdateItem** request shows how to set the sensitivity property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab3de-142">Программа</span><span class="sxs-lookup"><span data-stu-id="ab3de-142">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ab3de-143">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ab3de-143">Comments</span></span>

<span data-ttu-id="ab3de-144">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ab3de-144">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="setitemfield-request-elements"></a><span data-ttu-id="ab3de-145">Элементы запроса SetItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-145">SetItemField Request Elements</span></span>

<span data-ttu-id="ab3de-146">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ab3de-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ab3de-147">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ab3de-147">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="ab3de-148">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ab3de-148">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="ab3de-149">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ab3de-149">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="ab3de-150">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="ab3de-150">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ab3de-151">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="ab3de-151">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="ab3de-152">SetItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-152">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="ab3de-153">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ab3de-153">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="ab3de-154">Message</span><span class="sxs-lookup"><span data-stu-id="ab3de-154">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ab3de-155">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="ab3de-155">Sensitivity</span></span>](sensitivity.md)
    
## <a name="appendtoitemfield-request-example"></a><span data-ttu-id="ab3de-156">Пример запроса AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-156">AppendToItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="ab3de-157">Описание</span><span class="sxs-lookup"><span data-stu-id="ab3de-157">Description</span></span>

<span data-ttu-id="ab3de-158">В следующем примере запрос **UpdateItem** показано, как добавить текст в свойстве текст элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3de-158">The following example of an **UpdateItem** request shows how to append text to the body property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab3de-159">Программа</span><span class="sxs-lookup"><span data-stu-id="ab3de-159">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ab3de-160">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ab3de-160">Comments</span></span>

<span data-ttu-id="ab3de-161">Следующие свойства поддержка append действия:</span><span class="sxs-lookup"><span data-stu-id="ab3de-161">The following properties support the append action:</span></span>
  
- <span data-ttu-id="ab3de-162">**сообщение: ReplyTo**</span><span class="sxs-lookup"><span data-stu-id="ab3de-162">**message:ReplyTo**</span></span>
    
- <span data-ttu-id="ab3de-163">**основной текст элемента:**</span><span class="sxs-lookup"><span data-stu-id="ab3de-163">**item:Body**</span></span>
    
- <span data-ttu-id="ab3de-164">Всех получателей и attendee коллекции свойств</span><span class="sxs-lookup"><span data-stu-id="ab3de-164">All the recipient and attendee collection properties</span></span>
    
<span data-ttu-id="ab3de-165">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ab3de-165">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="appendtoitemfield-request-elements"></a><span data-ttu-id="ab3de-166">Элементы запроса AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-166">AppendToItemField Request Elements</span></span>

<span data-ttu-id="ab3de-167">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ab3de-167">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ab3de-168">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ab3de-168">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="ab3de-169">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ab3de-169">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="ab3de-170">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ab3de-170">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="ab3de-171">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="ab3de-171">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ab3de-172">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="ab3de-172">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="ab3de-173">AppendToItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-173">AppendToItemField</span></span>](appendtoitemfield.md)
    
- [<span data-ttu-id="ab3de-174">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ab3de-174">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="ab3de-175">Message</span><span class="sxs-lookup"><span data-stu-id="ab3de-175">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ab3de-176">Body</span><span class="sxs-lookup"><span data-stu-id="ab3de-176">Body</span></span>](body.md)
    
## <a name="deleteitemfield-request-example"></a><span data-ttu-id="ab3de-177">Пример запроса DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-177">DeleteItemField request example</span></span>

### <a name="description"></a><span data-ttu-id="ab3de-178">Описание</span><span class="sxs-lookup"><span data-stu-id="ab3de-178">Description</span></span>

<span data-ttu-id="ab3de-179">Приведенный ниже запрос **UpdateItem** показано, как удалить свойство элемента.</span><span class="sxs-lookup"><span data-stu-id="ab3de-179">The following example of an **UpdateItem** request shows how to delete a property on an item.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab3de-180">Программа</span><span class="sxs-lookup"><span data-stu-id="ab3de-180">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AutoResolve" 
                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ab3de-181">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ab3de-181">Comments</span></span>

<span data-ttu-id="ab3de-182">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ab3de-182">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="deleteitemfield-request-elements"></a><span data-ttu-id="ab3de-183">Элементы запроса DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-183">DeleteItemField Request Elements</span></span>

<span data-ttu-id="ab3de-184">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ab3de-184">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ab3de-185">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="ab3de-185">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="ab3de-186">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="ab3de-186">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="ab3de-187">ItemChange</span><span class="sxs-lookup"><span data-stu-id="ab3de-187">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="ab3de-188">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="ab3de-188">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ab3de-189">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="ab3de-189">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="ab3de-190">DeleteItemField</span><span class="sxs-lookup"><span data-stu-id="ab3de-190">DeleteItemField</span></span>](deleteitemfield.md)
    
- [<span data-ttu-id="ab3de-191">FieldURI</span><span class="sxs-lookup"><span data-stu-id="ab3de-191">FieldURI</span></span>](fielduri.md)
    
## <a name="successful-response-example"></a><span data-ttu-id="ab3de-192">Пример успешного ответа</span><span class="sxs-lookup"><span data-stu-id="ab3de-192">Successful response example</span></span>

### <a name="description"></a><span data-ttu-id="ab3de-193">Описание</span><span class="sxs-lookup"><span data-stu-id="ab3de-193">Description</span></span>

<span data-ttu-id="ab3de-194">В следующем примере показано успешного ответа на запрос **UpdateItem** .</span><span class="sxs-lookup"><span data-stu-id="ab3de-194">The following example shows a successful response to an **UpdateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ab3de-195">Программа</span><span class="sxs-lookup"><span data-stu-id="ab3de-195">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
  xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="664" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ab3de-196">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ab3de-196">Comments</span></span>

<span data-ttu-id="ab3de-197">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ab3de-197">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="ab3de-198">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="ab3de-198">Successful response elements</span></span>

<span data-ttu-id="ab3de-199">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ab3de-199">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ab3de-200">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ab3de-200">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ab3de-201">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="ab3de-201">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="ab3de-202">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ab3de-202">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ab3de-203">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ab3de-203">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="ab3de-204">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ab3de-204">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ab3de-205">Элементы</span><span class="sxs-lookup"><span data-stu-id="ab3de-205">Items</span></span>](items.md)
    
- [<span data-ttu-id="ab3de-206">Message</span><span class="sxs-lookup"><span data-stu-id="ab3de-206">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ab3de-207">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="ab3de-207">ItemId</span></span>](itemid.md)
    
## <a name="see-also"></a><span data-ttu-id="ab3de-208">См. также</span><span class="sxs-lookup"><span data-stu-id="ab3de-208">See also</span></span>



[<span data-ttu-id="ab3de-209">Операция UpdateItem (задача)</span><span class="sxs-lookup"><span data-stu-id="ab3de-209">UpdateItem operation (task)</span></span>](updateitem-operation-task.md)
  
[<span data-ttu-id="ab3de-210">Операция UpdateItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="ab3de-210">UpdateItem operation (contact)</span></span>](updateitem-operation-contact.md)


- [<span data-ttu-id="ab3de-211">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ab3de-211">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="ab3de-212">Обновление контактов</span><span class="sxs-lookup"><span data-stu-id="ab3de-212">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
  
[<span data-ttu-id="ab3de-213">Обновление задач</span><span class="sxs-lookup"><span data-stu-id="ab3de-213">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

