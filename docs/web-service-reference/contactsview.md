---
title: ContactsView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsView
api_type:
- schema
ms.assetid: 8534f44b-a5af-4a9f-9621-23a3eff5f9d8
description: Элемент ContactsView определяет поиска на основе алфавитном отображения имен контактов.
ms.openlocfilehash: e578eb4dd0042b8c478e883c7fa54d7f2e984229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761752"
---
# <a name="contactsview"></a><span data-ttu-id="38b88-103">ContactsView</span><span class="sxs-lookup"><span data-stu-id="38b88-103">ContactsView</span></span>

<span data-ttu-id="38b88-104">Элемент **ContactsView** определяет поиска на основе алфавитном отображения имен контактов.</span><span class="sxs-lookup"><span data-stu-id="38b88-104">The **ContactsView** element defines a search for contact items based on alphabetical display names.</span></span> 
  
[<span data-ttu-id="38b88-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="38b88-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="38b88-106">ContactsView</span><span class="sxs-lookup"><span data-stu-id="38b88-106">ContactsView</span></span>](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

<span data-ttu-id="38b88-107">**ContactsViewType**</span><span class="sxs-lookup"><span data-stu-id="38b88-107">**ContactsViewType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="38b88-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="38b88-108">Attributes and elements</span></span>

<span data-ttu-id="38b88-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="38b88-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38b88-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="38b88-110">Attributes</span></span>

|<span data-ttu-id="38b88-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="38b88-111">**Attribute**</span></span>|<span data-ttu-id="38b88-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38b88-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38b88-113">**MaxEntriesReturned**</span><span class="sxs-lookup"><span data-stu-id="38b88-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="38b88-114">Описывает максимальное число результатов, возвращаемых в ответе [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="38b88-114">Describes the maximum number of results to return in the [FindItem](finditem.md) response.</span></span>  <br/> |
|<span data-ttu-id="38b88-115">**InitialName**</span><span class="sxs-lookup"><span data-stu-id="38b88-115">**InitialName**</span></span> <br/> |<span data-ttu-id="38b88-116">Определяет имя в списке контактов, чтобы вернуться в ответе.</span><span class="sxs-lookup"><span data-stu-id="38b88-116">Defines the first name in the contacts list to return in the response.</span></span> <span data-ttu-id="38b88-117">Если указанный начальное имя не в списке контактов, далее алфавитном имя в соответствии с культурные контекста будут возвращены, за исключением Если далее имя идет после **FinalName**.</span><span class="sxs-lookup"><span data-stu-id="38b88-117">If the specified initial name is not in the contacts list, the next alphabetical name as defined by the cultural context will be returned, except if the next name comes after **FinalName**.</span></span> <span data-ttu-id="38b88-118">Если указан атрибут **InitialName** , ответ будет содержать список контактов, начинающимся на имя в списке контактов.</span><span class="sxs-lookup"><span data-stu-id="38b88-118">If the **InitialName** attribute is omitted, the response will contain a list of contacts that starts with the first name in the contact list.</span></span> <span data-ttu-id="38b88-119">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="38b88-119">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="38b88-120">**FinalName**</span><span class="sxs-lookup"><span data-stu-id="38b88-120">**FinalName**</span></span> <br/> |<span data-ttu-id="38b88-121">Определяет имя последнего в списке контактов, чтобы вернуться в ответе.</span><span class="sxs-lookup"><span data-stu-id="38b88-121">Defines the last name in the contacts list to return in the response.</span></span> <span data-ttu-id="38b88-122">Если указан атрибут **FinalName** , ответ будет содержать все последующие контакты в заданный порядок сортировки.</span><span class="sxs-lookup"><span data-stu-id="38b88-122">If the **FinalName** attribute is omitted, the response will contain all subsequent contacts in the specified sort order.</span></span> <span data-ttu-id="38b88-123">Если указанный окончательное имя не в списке контактов, далее алфавитном имя в соответствии с культурные контекста будет исключен.</span><span class="sxs-lookup"><span data-stu-id="38b88-123">If the specified final name is not in the contacts list, the next alphabetical name as defined by the cultural context will be excluded.</span></span>  <br/><br/><span data-ttu-id="38b88-124">Например если FinalName = «Имя», но имя не входит в список контактов, контакты, имеющие отображение имен из Имя1 или не будет включен.</span><span class="sxs-lookup"><span data-stu-id="38b88-124">For example, if FinalName="Name", but Name is not in the contacts list, contacts that have display names of Name1 or NAME will not be included.</span></span>  <br/><br/><span data-ttu-id="38b88-125">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="38b88-125">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="38b88-126">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="38b88-126">Child elements</span></span>

<span data-ttu-id="38b88-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="38b88-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38b88-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="38b88-128">Parent elements</span></span>

|<span data-ttu-id="38b88-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="38b88-129">**Element**</span></span>|<span data-ttu-id="38b88-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38b88-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38b88-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="38b88-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="38b88-132">Определяет запрос для поиска элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="38b88-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="38b88-133">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="38b88-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="38b88-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="38b88-134">Remarks</span></span>

<span data-ttu-id="38b88-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="38b88-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="38b88-136">Пример</span><span class="sxs-lookup"><span data-stu-id="38b88-136">Example</span></span>

<span data-ttu-id="38b88-137">Следующий пример запроса показано, как найти первые три контакты, начиная с контактом, который содержит отображаемое имя Келли Ролин.</span><span class="sxs-lookup"><span data-stu-id="38b88-137">The following example of a request demonstrates how to find the first three contacts starting with the contact that has the display name of Kelly Rollin.</span></span>
  
```xml
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
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ContactsView MaxEntriesReturned="3" InitialName="Kelly Rollin" />
      <SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:FieldOrder>
        </SortOrder>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="38b88-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="38b88-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38b88-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="38b88-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="38b88-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="38b88-140">Schema Name</span></span>  <br/> |<span data-ttu-id="38b88-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="38b88-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="38b88-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="38b88-142">Validation File</span></span>  <br/> |<span data-ttu-id="38b88-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="38b88-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38b88-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="38b88-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="38b88-145">False</span><span class="sxs-lookup"><span data-stu-id="38b88-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38b88-146">См. также</span><span class="sxs-lookup"><span data-stu-id="38b88-146">See also</span></span>

- [<span data-ttu-id="38b88-147">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="38b88-147">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="38b88-148">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="38b88-148">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

