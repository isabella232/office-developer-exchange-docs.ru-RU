---
title: контактсвиев
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
description: Элемент Контактсвиев определяет Поиск элементов контакта в соответствии с отображаемыми именами в алфавитном порядке.
ms.openlocfilehash: e578eb4dd0042b8c478e883c7fa54d7f2e984229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761752"
---
# <a name="contactsview"></a><span data-ttu-id="ea51a-103">контактсвиев</span><span class="sxs-lookup"><span data-stu-id="ea51a-103">ContactsView</span></span>

<span data-ttu-id="ea51a-104">Элемент **контактсвиев** определяет Поиск элементов контакта в соответствии с отображаемыми именами в алфавитном порядке.</span><span class="sxs-lookup"><span data-stu-id="ea51a-104">The **ContactsView** element defines a search for contact items based on alphabetical display names.</span></span> 
  
[<span data-ttu-id="ea51a-105">FindItem</span><span class="sxs-lookup"><span data-stu-id="ea51a-105">FindItem</span></span>](finditem.md)
  
[<span data-ttu-id="ea51a-106">контактсвиев</span><span class="sxs-lookup"><span data-stu-id="ea51a-106">ContactsView</span></span>](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

<span data-ttu-id="ea51a-107">**контактсвиевтипе**</span><span class="sxs-lookup"><span data-stu-id="ea51a-107">**ContactsViewType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="ea51a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ea51a-108">Attributes and elements</span></span>

<span data-ttu-id="ea51a-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ea51a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea51a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ea51a-110">Attributes</span></span>

|<span data-ttu-id="ea51a-111">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ea51a-111">**Attribute**</span></span>|<span data-ttu-id="ea51a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea51a-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea51a-113">**максентриесретурнед**</span><span class="sxs-lookup"><span data-stu-id="ea51a-113">**MaxEntriesReturned**</span></span> <br/> |<span data-ttu-id="ea51a-114">Описывает максимальное число результатов, возвращаемых в ответе [FindItem](finditem.md) .</span><span class="sxs-lookup"><span data-stu-id="ea51a-114">Describes the maximum number of results to return in the [FindItem](finditem.md) response.</span></span>  <br/> |
|<span data-ttu-id="ea51a-115">**инитиалнаме**</span><span class="sxs-lookup"><span data-stu-id="ea51a-115">**InitialName**</span></span> <br/> |<span data-ttu-id="ea51a-116">Определяет первое имя в списке контактов для возврата в ответе.</span><span class="sxs-lookup"><span data-stu-id="ea51a-116">Defines the first name in the contacts list to return in the response.</span></span> <span data-ttu-id="ea51a-117">Если указанное начальное имя отсутствует в списке Contacts (контакты), будет возвращено следующее буквенное имя, заданное культурным контекстом, за исключением случаев, когда следующее имя предшествует **финалнаме**.</span><span class="sxs-lookup"><span data-stu-id="ea51a-117">If the specified initial name is not in the contacts list, the next alphabetical name as defined by the cultural context will be returned, except if the next name comes after **FinalName**.</span></span> <span data-ttu-id="ea51a-118">Если атрибут **инитиалнаме** опущен, ответ будет содержать список контактов, начинающихся с первого имени в списке контактов.</span><span class="sxs-lookup"><span data-stu-id="ea51a-118">If the **InitialName** attribute is omitted, the response will contain a list of contacts that starts with the first name in the contact list.</span></span> <span data-ttu-id="ea51a-119">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="ea51a-119">This attribute is optional.</span></span>  <br/> |
|<span data-ttu-id="ea51a-120">**финалнаме**</span><span class="sxs-lookup"><span data-stu-id="ea51a-120">**FinalName**</span></span> <br/> |<span data-ttu-id="ea51a-121">Определяет фамилию в списке контактов, возвращаемой в ответе.</span><span class="sxs-lookup"><span data-stu-id="ea51a-121">Defines the last name in the contacts list to return in the response.</span></span> <span data-ttu-id="ea51a-122">Если атрибут **финалнаме** опущен, ответ будет содержать все последующие контакты в указанном порядке сортировки.</span><span class="sxs-lookup"><span data-stu-id="ea51a-122">If the **FinalName** attribute is omitted, the response will contain all subsequent contacts in the specified sort order.</span></span> <span data-ttu-id="ea51a-123">Если указанное итоговое имя отсутствует в списке Contacts (контакты), то следующее буквенное имя, заданное культурным контекстом, будет исключено.</span><span class="sxs-lookup"><span data-stu-id="ea51a-123">If the specified final name is not in the contacts list, the next alphabetical name as defined by the cultural context will be excluded.</span></span>  <br/><br/><span data-ttu-id="ea51a-124">Например, если Финалнаме = "Name", но имя отсутствует в списке Contacts (контакты), то контакты, у которых отображаются имена Имя1 или NAME, не будут включены.</span><span class="sxs-lookup"><span data-stu-id="ea51a-124">For example, if FinalName="Name", but Name is not in the contacts list, contacts that have display names of Name1 or NAME will not be included.</span></span>  <br/><br/><span data-ttu-id="ea51a-125">Этот атрибут является необязательным.</span><span class="sxs-lookup"><span data-stu-id="ea51a-125">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ea51a-126">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ea51a-126">Child elements</span></span>

<span data-ttu-id="ea51a-127">Нет.</span><span class="sxs-lookup"><span data-stu-id="ea51a-127">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ea51a-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ea51a-128">Parent elements</span></span>

|<span data-ttu-id="ea51a-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ea51a-129">**Element**</span></span>|<span data-ttu-id="ea51a-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ea51a-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea51a-131">FindItem</span><span class="sxs-lookup"><span data-stu-id="ea51a-131">FindItem</span></span>](finditem.md) <br/> |<span data-ttu-id="ea51a-132">Определяет запрос на поиск элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ea51a-132">Defines a request to find items in a mailbox.</span></span><br/><br/> <span data-ttu-id="ea51a-133">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="ea51a-133">The following is the XPath expression to this element:</span></span>  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea51a-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="ea51a-134">Remarks</span></span>

<span data-ttu-id="ea51a-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ea51a-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="ea51a-136">Пример</span><span class="sxs-lookup"><span data-stu-id="ea51a-136">Example</span></span>

<span data-ttu-id="ea51a-137">В приведенном ниже примере запроса показано, как найти первые три контакта, начиная с контакта с отображаемым именем Kelly.</span><span class="sxs-lookup"><span data-stu-id="ea51a-137">The following example of a request demonstrates how to find the first three contacts starting with the contact that has the display name of Kelly Rollin.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="ea51a-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ea51a-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea51a-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ea51a-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ea51a-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ea51a-140">Schema Name</span></span>  <br/> |<span data-ttu-id="ea51a-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="ea51a-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ea51a-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ea51a-142">Validation File</span></span>  <br/> |<span data-ttu-id="ea51a-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="ea51a-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea51a-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ea51a-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea51a-145">False</span><span class="sxs-lookup"><span data-stu-id="ea51a-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea51a-146">См. также</span><span class="sxs-lookup"><span data-stu-id="ea51a-146">See also</span></span>

- [<span data-ttu-id="ea51a-147">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="ea51a-147">FindItem operation</span></span>](finditem-operation.md)
- [<span data-ttu-id="ea51a-148">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="ea51a-148">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

