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
description: Элемент ResolveNames определяет запрос на разрешение неоднозначных имен.
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835172"
---
# <a name="resolvenames"></a><span data-ttu-id="f8f59-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="f8f59-103">ResolveNames</span></span>

<span data-ttu-id="f8f59-104">Элемент **ResolveNames** определяет запрос на разрешение неоднозначных имен.</span><span class="sxs-lookup"><span data-stu-id="f8f59-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="f8f59-105">**ресолвенаместипе**</span><span class="sxs-lookup"><span data-stu-id="f8f59-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8f59-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f8f59-106">Attributes and elements</span></span>

<span data-ttu-id="f8f59-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f8f59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8f59-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f8f59-108">Attributes</span></span>

|<span data-ttu-id="f8f59-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f8f59-109">**Attribute**</span></span>|<span data-ttu-id="f8f59-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8f59-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f8f59-111">**ретурнфуллконтактдата**</span><span class="sxs-lookup"><span data-stu-id="f8f59-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="f8f59-112">Показывает, возвращаются ли в ответе полные контактные данные общедоступных контактов для общедоступного имени.</span><span class="sxs-lookup"><span data-stu-id="f8f59-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="f8f59-113">Этот атрибут необходим для общедоступных контактов.</span><span class="sxs-lookup"><span data-stu-id="f8f59-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="f8f59-114">Это значение не влияет на частные и частные списки рассылки, для которых идентификатор [ItemId](itemid.md) всегда возвращается.</span><span class="sxs-lookup"><span data-stu-id="f8f59-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="f8f59-115">**SearchScope**</span><span class="sxs-lookup"><span data-stu-id="f8f59-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="f8f59-116">Определяет порядок и область поиска ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="f8f59-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="f8f59-117">контактдаташапе</span><span class="sxs-lookup"><span data-stu-id="f8f59-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="f8f59-118">Определяет набор свойств, возвращаемый для контактов.</span><span class="sxs-lookup"><span data-stu-id="f8f59-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="f8f59-119">Этот атрибут появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="f8f59-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="f8f59-120">Значения атрибутов Ретурнфуллконтактдата</span><span class="sxs-lookup"><span data-stu-id="f8f59-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="f8f59-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f8f59-121">**Value**</span></span>|<span data-ttu-id="f8f59-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8f59-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f8f59-123">Верно.</span><span class="sxs-lookup"><span data-stu-id="f8f59-123">True</span></span>  <br/> |<span data-ttu-id="f8f59-124">Возвращаются полные контактные данные для общедоступных контактов.</span><span class="sxs-lookup"><span data-stu-id="f8f59-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="f8f59-125">False</span><span class="sxs-lookup"><span data-stu-id="f8f59-125">False</span></span>  <br/> |<span data-ttu-id="f8f59-126">Полные контактные сведения для общедоступных контактов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="f8f59-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="f8f59-127">Значения атрибутов SearchScope</span><span class="sxs-lookup"><span data-stu-id="f8f59-127">SearchScope attribute values</span></span>

|<span data-ttu-id="f8f59-128">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f8f59-128">**Value**</span></span>|<span data-ttu-id="f8f59-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8f59-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f8f59-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="f8f59-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="f8f59-131">Выполняется поиск только в службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8f59-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="f8f59-132">активедиректориконтактс</span><span class="sxs-lookup"><span data-stu-id="f8f59-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="f8f59-133">Сначала выполняется поиск в Active Directory, после чего выполняется поиск по папкам контактов, указанным в свойстве [парентфолдеридс](parentfolderids.md) .</span><span class="sxs-lookup"><span data-stu-id="f8f59-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="f8f59-134">Контакты</span><span class="sxs-lookup"><span data-stu-id="f8f59-134">Contacts</span></span>  <br/> |<span data-ttu-id="f8f59-135">Выполняется поиск только папок контактов, определенных свойством [парентфолдеридс](parentfolderids.md) .</span><span class="sxs-lookup"><span data-stu-id="f8f59-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="f8f59-136">контактсактиведиректори</span><span class="sxs-lookup"><span data-stu-id="f8f59-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="f8f59-137">Папки контактов, идентифицируемые свойством [парентфолдеридс](parentfolderids.md) , сначала просматриваются, а затем в Active Directory выполняется поиск.</span><span class="sxs-lookup"><span data-stu-id="f8f59-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="f8f59-138">Значения атрибутов Контактдаташапе</span><span class="sxs-lookup"><span data-stu-id="f8f59-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="f8f59-139">**Значение**</span><span class="sxs-lookup"><span data-stu-id="f8f59-139">**Value**</span></span>|<span data-ttu-id="f8f59-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8f59-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f8f59-141">идонли</span><span class="sxs-lookup"><span data-stu-id="f8f59-141">IdOnly</span></span>  <br/> |<span data-ttu-id="f8f59-142">Возвращается свойство идентификатора элемента Contact.</span><span class="sxs-lookup"><span data-stu-id="f8f59-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="f8f59-143">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="f8f59-143">Default</span></span>  <br/> |<span data-ttu-id="f8f59-144">Возвращается набор свойств элемента контакта по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f8f59-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="f8f59-145">Дополнительные сведения о [фигурах ответа](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)см.</span><span class="sxs-lookup"><span data-stu-id="f8f59-145">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="f8f59-146">аллпропертиес</span><span class="sxs-lookup"><span data-stu-id="f8f59-146">AllProperties</span></span>  <br/> |<span data-ttu-id="f8f59-147">Возвращается набор Аллпропертиес для свойств элемента Contact.</span><span class="sxs-lookup"><span data-stu-id="f8f59-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="f8f59-148">Дополнительные сведения о [фигурах ответа](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)см.</span><span class="sxs-lookup"><span data-stu-id="f8f59-148">For more information, see [Response shapes in EWS](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f8f59-149">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f8f59-149">Child elements</span></span>

|<span data-ttu-id="f8f59-150">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f8f59-150">**Element**</span></span>|<span data-ttu-id="f8f59-151">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8f59-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8f59-152">парентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="f8f59-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="f8f59-153">Содержит массив идентификаторов папок контактов, в которых будет выполняться поиск, если для атрибута **SearchScope** задано значение Активедиректориконтактс, Contacts или контактсактиведиректори.</span><span class="sxs-lookup"><span data-stu-id="f8f59-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="f8f59-154">Массив Парентфолдеридс может содержать только один идентификатор папки контактов.</span><span class="sxs-lookup"><span data-stu-id="f8f59-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="f8f59-155">Если элемент **парентфолдеридс** отсутствует, выполняется поиск по папке "Контакты" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="f8f59-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="f8f59-156">Идентификатор папки можно использовать для доступа к представителям.</span><span class="sxs-lookup"><span data-stu-id="f8f59-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="f8f59-157">Поиск в Active Directory выполняется с помощью списков управления доступом (ACL).</span><span class="sxs-lookup"><span data-stu-id="f8f59-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="f8f59-158">У некоторых пользователей могут отсутствовать права на просмотр некоторых объектов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f8f59-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="f8f59-159">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="f8f59-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="f8f59-160">унресолведентри</span><span class="sxs-lookup"><span data-stu-id="f8f59-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="f8f59-161">Содержит имя контакта или списка рассылки, которые требуется разрешить.</span><span class="sxs-lookup"><span data-stu-id="f8f59-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8f59-162">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f8f59-162">Parent elements</span></span>

<span data-ttu-id="f8f59-163">Нет.</span><span class="sxs-lookup"><span data-stu-id="f8f59-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f8f59-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="f8f59-164">Remarks</span></span>

<span data-ttu-id="f8f59-165">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f8f59-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8f59-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f8f59-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8f59-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f8f59-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f8f59-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f8f59-168">Schema name</span></span>  <br/> |<span data-ttu-id="f8f59-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f8f59-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f8f59-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f8f59-170">Validation file</span></span>  <br/> |<span data-ttu-id="f8f59-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f8f59-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f8f59-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f8f59-172">Can be empty</span></span>  <br/> |<span data-ttu-id="f8f59-173">False</span><span class="sxs-lookup"><span data-stu-id="f8f59-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8f59-174">См. также</span><span class="sxs-lookup"><span data-stu-id="f8f59-174">See also</span></span>



[<span data-ttu-id="f8f59-175">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="f8f59-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="f8f59-176">ресолвенаместипе</span><span class="sxs-lookup"><span data-stu-id="f8f59-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="f8f59-177">ресолвенамессеарчскопетипе</span><span class="sxs-lookup"><span data-stu-id="f8f59-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="f8f59-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f8f59-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="f8f59-179">Использование разрешения имен</span><span class="sxs-lookup"><span data-stu-id="f8f59-179">Using Name Resolution</span></span>](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

