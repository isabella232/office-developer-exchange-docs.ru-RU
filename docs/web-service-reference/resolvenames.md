---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: Элемент ResolveNames определяет запрос для разрешения неоднозначных имен.
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835172"
---
# <a name="resolvenames"></a><span data-ttu-id="8b94d-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="8b94d-103">ResolveNames</span></span>

<span data-ttu-id="8b94d-104">Элемент **ResolveNames** определяет запрос для разрешения неоднозначных имен.</span><span class="sxs-lookup"><span data-stu-id="8b94d-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="8b94d-105">**ResolveNamesType**</span><span class="sxs-lookup"><span data-stu-id="8b94d-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b94d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8b94d-106">Attributes and elements</span></span>

<span data-ttu-id="8b94d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8b94d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b94d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8b94d-108">Attributes</span></span>

|<span data-ttu-id="8b94d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8b94d-109">**Attribute**</span></span>|<span data-ttu-id="8b94d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b94d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8b94d-111">**ReturnFullContactData**</span><span class="sxs-lookup"><span data-stu-id="8b94d-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="8b94d-112">Описание, возвращаются ли полные контактные данные для контактов общедоступной для разрешения имени в ответе.</span><span class="sxs-lookup"><span data-stu-id="8b94d-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="8b94d-113">Этот атрибут является обязательным для контактов общедоступной.</span><span class="sxs-lookup"><span data-stu-id="8b94d-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="8b94d-114">Это значение не влияет на закрытый контактов и частные списки рассылки, для которых всегда возвращается [идентификатор элемента](itemid.md) .</span><span class="sxs-lookup"><span data-stu-id="8b94d-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="8b94d-115">**Область поиска**</span><span class="sxs-lookup"><span data-stu-id="8b94d-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="8b94d-116">Определяет порядок и области для поиска ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="8b94d-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="8b94d-117">ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="8b94d-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="8b94d-118">Определяет свойство набор, возвращаемый для контактов.</span><span class="sxs-lookup"><span data-stu-id="8b94d-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="8b94d-119">Этот атрибут появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="8b94d-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="8b94d-120">Значения атрибутов ReturnFullContactData</span><span class="sxs-lookup"><span data-stu-id="8b94d-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="8b94d-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8b94d-121">**Value**</span></span>|<span data-ttu-id="8b94d-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b94d-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8b94d-123">True</span><span class="sxs-lookup"><span data-stu-id="8b94d-123">True</span></span>  <br/> |<span data-ttu-id="8b94d-124">Возвращаются полные контактные данные для контактов общедоступной.</span><span class="sxs-lookup"><span data-stu-id="8b94d-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="8b94d-125">False</span><span class="sxs-lookup"><span data-stu-id="8b94d-125">False</span></span>  <br/> |<span data-ttu-id="8b94d-126">Полное контактные данные для контактов общедоступной не возвращается.</span><span class="sxs-lookup"><span data-stu-id="8b94d-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="8b94d-127">Значения атрибутов область поиска</span><span class="sxs-lookup"><span data-stu-id="8b94d-127">SearchScope attribute values</span></span>

|<span data-ttu-id="8b94d-128">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8b94d-128">**Value**</span></span>|<span data-ttu-id="8b94d-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b94d-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8b94d-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="8b94d-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="8b94d-131">Поиск службы каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8b94d-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="8b94d-132">ActiveDirectoryContacts</span><span class="sxs-lookup"><span data-stu-id="8b94d-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="8b94d-133">Сначала выполняется поиск Active Directory, а затем выполняется поиск контакта папках, указанных в свойстве [ParentFolderIds](parentfolderids.md) .</span><span class="sxs-lookup"><span data-stu-id="8b94d-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="8b94d-134">Контакты</span><span class="sxs-lookup"><span data-stu-id="8b94d-134">Contacts</span></span>  <br/> |<span data-ttu-id="8b94d-135">Поиск осуществляется только папки контактов, указанных в свойстве [ParentFolderIds](parentfolderids.md) .</span><span class="sxs-lookup"><span data-stu-id="8b94d-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="8b94d-136">ContactsActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="8b94d-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="8b94d-137">Сначала выполняется поиск папок контактов, указанных в свойстве [ParentFolderIds](parentfolderids.md) и затем выполняется поиск Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8b94d-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="8b94d-138">Значения атрибутов ContactDataShape</span><span class="sxs-lookup"><span data-stu-id="8b94d-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="8b94d-139">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8b94d-139">**Value**</span></span>|<span data-ttu-id="8b94d-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b94d-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8b94d-141">IdOnly</span><span class="sxs-lookup"><span data-stu-id="8b94d-141">IdOnly</span></span>  <br/> |<span data-ttu-id="8b94d-142">Свойство идентификатора элемента контакта, возвращается.</span><span class="sxs-lookup"><span data-stu-id="8b94d-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="8b94d-143">Значение по умолчанию</span><span class="sxs-lookup"><span data-stu-id="8b94d-143">Default</span></span>  <br/> |<span data-ttu-id="8b94d-144">Возвращается набор по умолчанию свойства элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="8b94d-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="8b94d-145">Для получения дополнительных сведений см [ответа фигур в веб-служб Exchange](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8b94d-145">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="8b94d-146">AllProperties</span><span class="sxs-lookup"><span data-stu-id="8b94d-146">AllProperties</span></span>  <br/> |<span data-ttu-id="8b94d-147">Возвращаются AllProperties набора свойств элемента контакта.</span><span class="sxs-lookup"><span data-stu-id="8b94d-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="8b94d-148">Для получения дополнительных сведений см [ответа фигур в веб-служб Exchange](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8b94d-148">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8b94d-149">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8b94d-149">Child elements</span></span>

|<span data-ttu-id="8b94d-150">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8b94d-150">**Element**</span></span>|<span data-ttu-id="8b94d-151">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8b94d-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b94d-152">ParentFolderIds</span><span class="sxs-lookup"><span data-stu-id="8b94d-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="8b94d-153">Содержит массив идентификаторов папке контактов, которые будет искать, если значение атрибута **область поиска** ActiveDirectoryContacts, контактов или ContactsActiveDirectory.</span><span class="sxs-lookup"><span data-stu-id="8b94d-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="8b94d-154">Массив ParentFolderIds может содержать только идентификатор одной папке контактов.</span><span class="sxs-lookup"><span data-stu-id="8b94d-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="8b94d-155">Если элемент **ParentFolderIds** не задан, выполняется поиск папки Контакты по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b94d-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="8b94d-156">Идентификатор папки можно использовать для доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="8b94d-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="8b94d-157">Поиск Active Directory выполняются с помощью списки управления доступом (ACL).</span><span class="sxs-lookup"><span data-stu-id="8b94d-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="8b94d-158">Некоторым пользователям может не иметь права на доступ, чтобы увидеть некоторые объекты Active Directory.</span><span class="sxs-lookup"><span data-stu-id="8b94d-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="8b94d-159">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="8b94d-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="8b94d-160">UnresolvedEntry</span><span class="sxs-lookup"><span data-stu-id="8b94d-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="8b94d-161">Содержит имя контакта или список рассылки для разрешения.</span><span class="sxs-lookup"><span data-stu-id="8b94d-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8b94d-162">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8b94d-162">Parent elements</span></span>

<span data-ttu-id="8b94d-163">Нет.</span><span class="sxs-lookup"><span data-stu-id="8b94d-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8b94d-164">Замечания</span><span class="sxs-lookup"><span data-stu-id="8b94d-164">Remarks</span></span>

<span data-ttu-id="8b94d-165">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b94d-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b94d-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8b94d-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b94d-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8b94d-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8b94d-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8b94d-168">Schema name</span></span>  <br/> |<span data-ttu-id="8b94d-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="8b94d-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8b94d-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8b94d-170">Validation file</span></span>  <br/> |<span data-ttu-id="8b94d-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8b94d-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8b94d-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8b94d-172">Can be empty</span></span>  <br/> |<span data-ttu-id="8b94d-173">False</span><span class="sxs-lookup"><span data-stu-id="8b94d-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8b94d-174">См. также</span><span class="sxs-lookup"><span data-stu-id="8b94d-174">See also</span></span>



[<span data-ttu-id="8b94d-175">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="8b94d-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="8b94d-176">ResolveNamesType</span><span class="sxs-lookup"><span data-stu-id="8b94d-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="8b94d-177">ResolveNamesSearchScopeType</span><span class="sxs-lookup"><span data-stu-id="8b94d-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="8b94d-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8b94d-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="8b94d-179">С помощью разрешения имен</span><span class="sxs-lookup"><span data-stu-id="8b94d-179">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

