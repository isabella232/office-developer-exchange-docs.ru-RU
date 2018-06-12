---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: Элемент CreateAttachment определяет запрос для создания вложения в элемент в хранилище Exchange.
ms.openlocfilehash: d403eb5ca15623d3a973f7b224dbcde5529cf1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761857"
---
# <a name="createattachment"></a><span data-ttu-id="1a4e1-103">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="1a4e1-103">CreateAttachment</span></span>

<span data-ttu-id="1a4e1-104">Элемент **CreateAttachment** определяет запрос для создания вложения в элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-104">The **CreateAttachment** element defines a request to create an attachment to an item in the Exchange store.</span></span> 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 <span data-ttu-id="1a4e1-105">**CreateAttachmentType**</span><span class="sxs-lookup"><span data-stu-id="1a4e1-105">**CreateAttachmentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a4e1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1a4e1-106">Attributes and elements</span></span>

<span data-ttu-id="1a4e1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a4e1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1a4e1-108">Attributes</span></span>

<span data-ttu-id="1a4e1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a4e1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1a4e1-110">Child elements</span></span>

|<span data-ttu-id="1a4e1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1a4e1-111">**Element**</span></span>|<span data-ttu-id="1a4e1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a4e1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a4e1-113">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="1a4e1-113">ParentItemId</span></span>](parentitemid.md) <br/> |<span data-ttu-id="1a4e1-114">Идентифицирует родительского элемента хранилища Exchange, который содержит созданный вложения.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-114">Identifies the parent Exchange store item that contains the created attachment.</span></span> <span data-ttu-id="1a4e1-115">Элемент [ParentItemId](parentitemid.md) необходимо предоставить идентификатор реальных Exchange хранения элемента.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-115">The [ParentItemId](parentitemid.md) element must provide the ID of a real Exchange store item.</span></span> <span data-ttu-id="1a4e1-116">Реальные хранения элементов можно извлечь с помощью [операции GetItem](getitem-operation.md); вложения извлекаются с помощью [операции GetAttachment](getattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1a4e1-116">Real store items can be retrieved by using the [GetItem operation](getitem-operation.md); attachments are retrieved by using the [GetAttachment operation](getattachment-operation.md).</span></span> <span data-ttu-id="1a4e1-117">Если [ParentItemId](parentitemid.md) передается, идентификатор файла вложения, возникает ошибка.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-117">An error occurs if the [ParentItemId](parentitemid.md) is passed the ID of a file attachment.</span></span> <span data-ttu-id="1a4e1-118">Если [ParentItemId](parentitemid.md) представляет идентификатор вложения существующего элемента, [операция CreateAttachment](createattachment-operation.md) добавляет новый вложения в существующие вложения.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-118">If the [ParentItemId](parentitemid.md) represents the ID of an existing item attachment, the [CreateAttachment operation](createattachment-operation.md) adds the new attachment to the existing attachment.</span></span>  <br/> <span data-ttu-id="1a4e1-119">Этот элемент является обязательным для [CreateAttachment операции](createattachment-operation.md).</span><span class="sxs-lookup"><span data-stu-id="1a4e1-119">This element is required for the [CreateAttachment operation](createattachment-operation.md).</span></span>  <br/> |
|[<span data-ttu-id="1a4e1-120">Вложения</span><span class="sxs-lookup"><span data-stu-id="1a4e1-120">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="1a4e1-121">Содержит элементы или файлы для присоединения к элементу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-121">Contains the items or files to attach to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1a4e1-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1a4e1-122">Parent elements</span></span>

<span data-ttu-id="1a4e1-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a4e1-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="1a4e1-124">Remarks</span></span>

<span data-ttu-id="1a4e1-125">Элемент вложения не существует как элемент хранилища.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-125">An item attachment does not exist as a store item.</span></span> <span data-ttu-id="1a4e1-126">Он существует только как вложения в элемент или другой вложения.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-126">It only exists as an attachment to an item or another attachment.</span></span> <span data-ttu-id="1a4e1-127">Элемент вложения можно получить только с помощью запроса [GetAttachment](getattachment.md) .</span><span class="sxs-lookup"><span data-stu-id="1a4e1-127">Item attachments can only be retrieved by using the [GetAttachment](getattachment.md) request.</span></span> 
  
<span data-ttu-id="1a4e1-128">Можно создать следующие вложений элемента:</span><span class="sxs-lookup"><span data-stu-id="1a4e1-128">The following item attachments can be created:</span></span>
  
- <span data-ttu-id="1a4e1-129">Элемент</span><span class="sxs-lookup"><span data-stu-id="1a4e1-129">Item</span></span>
    
- <span data-ttu-id="1a4e1-130">Message</span><span class="sxs-lookup"><span data-stu-id="1a4e1-130">Message</span></span>
    
- <span data-ttu-id="1a4e1-131">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="1a4e1-131">CalendarItem</span></span>
    
- <span data-ttu-id="1a4e1-132">Контакт</span><span class="sxs-lookup"><span data-stu-id="1a4e1-132">Contact</span></span>
    
- <span data-ttu-id="1a4e1-133">Задача</span><span class="sxs-lookup"><span data-stu-id="1a4e1-133">Task</span></span>
    
- <span data-ttu-id="1a4e1-134">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="1a4e1-134">MeetingMessage</span></span>
    
- <span data-ttu-id="1a4e1-135">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="1a4e1-135">MeetingRequest</span></span>
    
<span data-ttu-id="1a4e1-136">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-136">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="1a4e1-137">Пример</span><span class="sxs-lookup"><span data-stu-id="1a4e1-137">Example</span></span>

<span data-ttu-id="1a4e1-138">Следующем примере показано, как создавать и присоединение элемент в другой элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a4e1-138">The following example shows how to create and attach an item to another item in the Exchange store.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="1a4e1-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1a4e1-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a4e1-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1a4e1-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1a4e1-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1a4e1-141">Schema Name</span></span>  <br/> |<span data-ttu-id="1a4e1-142">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="1a4e1-142">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1a4e1-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1a4e1-143">Validation File</span></span>  <br/> |<span data-ttu-id="1a4e1-144">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1a4e1-144">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1a4e1-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1a4e1-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a4e1-146">False</span><span class="sxs-lookup"><span data-stu-id="1a4e1-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a4e1-147">См. также</span><span class="sxs-lookup"><span data-stu-id="1a4e1-147">See also</span></span>



[<span data-ttu-id="1a4e1-148">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="1a4e1-148">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="1a4e1-149">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="1a4e1-149">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="1a4e1-150">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="1a4e1-150">GetAttachment operation</span></span>](getattachment-operation.md)

