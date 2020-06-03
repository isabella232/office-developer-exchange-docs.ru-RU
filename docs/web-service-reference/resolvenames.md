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
ms.openlocfilehash: 9c36a5f84451f91e90a8e7148cf384b5cacd7f29
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467951"
---
# <a name="resolvenames"></a><span data-ttu-id="0d247-103">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0d247-103">ResolveNames</span></span>

<span data-ttu-id="0d247-104">Элемент **ResolveNames** определяет запрос на разрешение неоднозначных имен.</span><span class="sxs-lookup"><span data-stu-id="0d247-104">The **ResolveNames** element defines a request to resolve ambiguous names.</span></span> 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 <span data-ttu-id="0d247-105">**ресолвенаместипе**</span><span class="sxs-lookup"><span data-stu-id="0d247-105">**ResolveNamesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0d247-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0d247-106">Attributes and elements</span></span>

<span data-ttu-id="0d247-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0d247-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0d247-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0d247-108">Attributes</span></span>

|<span data-ttu-id="0d247-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0d247-109">**Attribute**</span></span>|<span data-ttu-id="0d247-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d247-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d247-111">**ретурнфуллконтактдата**</span><span class="sxs-lookup"><span data-stu-id="0d247-111">**ReturnFullContactData**</span></span> <br/> |<span data-ttu-id="0d247-112">Показывает, возвращаются ли в ответе полные контактные данные общедоступных контактов для общедоступного имени.</span><span class="sxs-lookup"><span data-stu-id="0d247-112">Describes whether the full contact details for public contacts for a resolved name are returned in the response.</span></span> <span data-ttu-id="0d247-113">Этот атрибут необходим для общедоступных контактов.</span><span class="sxs-lookup"><span data-stu-id="0d247-113">This attribute is required for public contacts.</span></span> <span data-ttu-id="0d247-114">Это значение не влияет на частные и частные списки рассылки, для которых идентификатор [ItemId](itemid.md) всегда возвращается.</span><span class="sxs-lookup"><span data-stu-id="0d247-114">This value does not affect private contacts and private distribution lists, for which [ItemId](itemid.md) is always returned.</span></span>  <br/> |
|<span data-ttu-id="0d247-115">**SearchScope**</span><span class="sxs-lookup"><span data-stu-id="0d247-115">**SearchScope**</span></span> <br/> |<span data-ttu-id="0d247-116">Определяет порядок и область поиска ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="0d247-116">Identifies the order and scope for a ResolveNames search.</span></span>  <br/> |
|<span data-ttu-id="0d247-117">контактдаташапе</span><span class="sxs-lookup"><span data-stu-id="0d247-117">ContactDataShape</span></span>  <br/> |<span data-ttu-id="0d247-118">Определяет набор свойств, возвращаемый для контактов.</span><span class="sxs-lookup"><span data-stu-id="0d247-118">Identifies the property set returned for contacts.</span></span> <span data-ttu-id="0d247-119">Этот атрибут появился в Exchange Server 2010 с пакетом обновления 2 (SP2).</span><span class="sxs-lookup"><span data-stu-id="0d247-119">This attribute was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a><span data-ttu-id="0d247-120">Значения атрибутов Ретурнфуллконтактдата</span><span class="sxs-lookup"><span data-stu-id="0d247-120">ReturnFullContactData attribute values</span></span>

|<span data-ttu-id="0d247-121">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0d247-121">**Value**</span></span>|<span data-ttu-id="0d247-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d247-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d247-123">Верно.</span><span class="sxs-lookup"><span data-stu-id="0d247-123">True</span></span>  <br/> |<span data-ttu-id="0d247-124">Возвращаются полные контактные данные для общедоступных контактов.</span><span class="sxs-lookup"><span data-stu-id="0d247-124">Full contact details for public contacts are returned.</span></span>  <br/> |
|<span data-ttu-id="0d247-125">False</span><span class="sxs-lookup"><span data-stu-id="0d247-125">False</span></span>  <br/> |<span data-ttu-id="0d247-126">Полные контактные сведения для общедоступных контактов не возвращаются.</span><span class="sxs-lookup"><span data-stu-id="0d247-126">Full contact details for public contacts are not returned.</span></span>  <br/> |
   
#### <a name="searchscope-attribute-values"></a><span data-ttu-id="0d247-127">Значения атрибутов SearchScope</span><span class="sxs-lookup"><span data-stu-id="0d247-127">SearchScope attribute values</span></span>

|<span data-ttu-id="0d247-128">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0d247-128">**Value**</span></span>|<span data-ttu-id="0d247-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d247-129">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d247-130">ActiveDirectory</span><span class="sxs-lookup"><span data-stu-id="0d247-130">ActiveDirectory</span></span>  <br/> |<span data-ttu-id="0d247-131">Выполняется поиск только в службе каталогов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0d247-131">Only the Active Directory directory service is searched.</span></span>  <br/> |
|<span data-ttu-id="0d247-132">активедиректориконтактс</span><span class="sxs-lookup"><span data-stu-id="0d247-132">ActiveDirectoryContacts</span></span>  <br/> |<span data-ttu-id="0d247-133">Сначала выполняется поиск в Active Directory, после чего выполняется поиск по папкам контактов, указанным в свойстве [парентфолдеридс](parentfolderids.md) .</span><span class="sxs-lookup"><span data-stu-id="0d247-133">Active Directory is searched first, and then the contact folders that are specified in the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="0d247-134">Контакты</span><span class="sxs-lookup"><span data-stu-id="0d247-134">Contacts</span></span>  <br/> |<span data-ttu-id="0d247-135">Выполняется поиск только папок контактов, определенных свойством [парентфолдеридс](parentfolderids.md) .</span><span class="sxs-lookup"><span data-stu-id="0d247-135">Only the contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched.</span></span>  <br/> |
|<span data-ttu-id="0d247-136">контактсактиведиректори</span><span class="sxs-lookup"><span data-stu-id="0d247-136">ContactsActiveDirectory</span></span>  <br/> |<span data-ttu-id="0d247-137">Папки контактов, идентифицируемые свойством [парентфолдеридс](parentfolderids.md) , сначала просматриваются, а затем в Active Directory выполняется поиск.</span><span class="sxs-lookup"><span data-stu-id="0d247-137">Contact folders that are identified by the [ParentFolderIds](parentfolderids.md) property are searched first and then Active Directory is searched.</span></span>  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a><span data-ttu-id="0d247-138">Значения атрибутов Контактдаташапе</span><span class="sxs-lookup"><span data-stu-id="0d247-138">ContactDataShape attribute values</span></span>

|<span data-ttu-id="0d247-139">**Значение**</span><span class="sxs-lookup"><span data-stu-id="0d247-139">**Value**</span></span>|<span data-ttu-id="0d247-140">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d247-140">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0d247-141">идонли</span><span class="sxs-lookup"><span data-stu-id="0d247-141">IdOnly</span></span>  <br/> |<span data-ttu-id="0d247-142">Возвращается свойство идентификатора элемента Contact.</span><span class="sxs-lookup"><span data-stu-id="0d247-142">The contact item identifier property is returned.</span></span>  <br/> |
|<span data-ttu-id="0d247-143">По умолчанию</span><span class="sxs-lookup"><span data-stu-id="0d247-143">Default</span></span>  <br/> |<span data-ttu-id="0d247-144">Возвращается набор свойств элемента контакта по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d247-144">The Default set of contact item properties is returned.</span></span> <span data-ttu-id="0d247-145">Дополнительные сведения о [фигурах ответа](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)см.</span><span class="sxs-lookup"><span data-stu-id="0d247-145">For more information, see [Response shapes in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="0d247-146">аллпропертиес</span><span class="sxs-lookup"><span data-stu-id="0d247-146">AllProperties</span></span>  <br/> |<span data-ttu-id="0d247-147">Возвращается набор Аллпропертиес для свойств элемента Contact.</span><span class="sxs-lookup"><span data-stu-id="0d247-147">The AllProperties set of contact item properties are returned.</span></span> <span data-ttu-id="0d247-148">Дополнительные сведения о [фигурах ответа](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)см.</span><span class="sxs-lookup"><span data-stu-id="0d247-148">For more information, see [Response shapes in EWS](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0d247-149">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0d247-149">Child elements</span></span>

|<span data-ttu-id="0d247-150">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0d247-150">**Element**</span></span>|<span data-ttu-id="0d247-151">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0d247-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0d247-152">парентфолдеридс</span><span class="sxs-lookup"><span data-stu-id="0d247-152">ParentFolderIds</span></span>](parentfolderids.md) <br/> |<span data-ttu-id="0d247-153">Содержит массив идентификаторов папок контактов, в которых будет выполняться поиск, если для атрибута **SearchScope** задано значение Активедиректориконтактс, Contacts или контактсактиведиректори.</span><span class="sxs-lookup"><span data-stu-id="0d247-153">Contains an array of contact folder identifiers that would be searched if the **SearchScope** attribute is set to ActiveDirectoryContacts, Contacts, or ContactsActiveDirectory.</span></span> <span data-ttu-id="0d247-154">Массив Парентфолдеридс может содержать только один идентификатор папки контактов.</span><span class="sxs-lookup"><span data-stu-id="0d247-154">The ParentFolderIds array can only contain a single contact folder identifier.</span></span> <span data-ttu-id="0d247-155">Если элемент **парентфолдеридс** отсутствует, выполняется поиск по папке "Контакты" по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="0d247-155">If the **ParentFolderIds** element is not present, the default Contacts folder is searched.</span></span>  <br/> <span data-ttu-id="0d247-156">Идентификатор папки можно использовать для доступа к представителям.</span><span class="sxs-lookup"><span data-stu-id="0d247-156">The folder identifier can be used for delegate access.</span></span>  <br/> <span data-ttu-id="0d247-157">Поиск в Active Directory выполняется с помощью списков управления доступом (ACL).</span><span class="sxs-lookup"><span data-stu-id="0d247-157">Active Directory searches are performed by using access control lists (ACLs).</span></span> <span data-ttu-id="0d247-158">У некоторых пользователей могут отсутствовать права на просмотр некоторых объектов Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0d247-158">Some users might not have the rights to see some Active Directory objects.</span></span>  <br/> <span data-ttu-id="0d247-159">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="0d247-159">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="0d247-160">унресолведентри</span><span class="sxs-lookup"><span data-stu-id="0d247-160">UnresolvedEntry</span></span>](unresolvedentry.md) <br/> |<span data-ttu-id="0d247-161">Содержит имя контакта или списка рассылки, которые требуется разрешить.</span><span class="sxs-lookup"><span data-stu-id="0d247-161">Contains the name of a contact or distribution list to resolve.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0d247-162">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0d247-162">Parent elements</span></span>

<span data-ttu-id="0d247-163">Нет.</span><span class="sxs-lookup"><span data-stu-id="0d247-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0d247-164">Примечания</span><span class="sxs-lookup"><span data-stu-id="0d247-164">Remarks</span></span>

<span data-ttu-id="0d247-165">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0d247-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0d247-166">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0d247-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0d247-167">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0d247-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0d247-168">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0d247-168">Schema name</span></span>  <br/> |<span data-ttu-id="0d247-169">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="0d247-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0d247-170">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0d247-170">Validation file</span></span>  <br/> |<span data-ttu-id="0d247-171">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0d247-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0d247-172">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0d247-172">Can be empty</span></span>  <br/> |<span data-ttu-id="0d247-173">False</span><span class="sxs-lookup"><span data-stu-id="0d247-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0d247-174">См. также</span><span class="sxs-lookup"><span data-stu-id="0d247-174">See also</span></span>



[<span data-ttu-id="0d247-175">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0d247-175">ResolveNames operation</span></span>](resolvenames-operation.md)
  
[<span data-ttu-id="0d247-176">ресолвенаместипе</span><span class="sxs-lookup"><span data-stu-id="0d247-176">ResolveNamesType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[<span data-ttu-id="0d247-177">ресолвенамессеарчскопетипе</span><span class="sxs-lookup"><span data-stu-id="0d247-177">ResolveNamesSearchScopeType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [<span data-ttu-id="0d247-178">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="0d247-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="0d247-179">Использование разрешения имен</span><span class="sxs-lookup"><span data-stu-id="0d247-179">Using Name Resolution</span></span>](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

