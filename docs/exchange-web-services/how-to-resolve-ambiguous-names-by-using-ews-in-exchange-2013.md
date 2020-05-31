---
title: Устранение неоднозначности имен с помощью EWS в Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Узнайте, как использовать управляемый API EWS или EWS для разрешения неоднозначных имен, получая возможные совпадения из доменных служб Active Directory (AD DS) или из папки "Контакты" в почтовом ящике пользователя.
ms.openlocfilehash: 05a88043083a27d2e6d445cd71e5f3919c5a775d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761105"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a><span data-ttu-id="fc1e1-103">Устранение неоднозначности имен с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="fc1e1-103">Resolve ambiguous names by using EWS in Exchange 2013</span></span>

<span data-ttu-id="fc1e1-104">Узнайте, как использовать управляемый API EWS или EWS для разрешения неоднозначных имен, получая возможные совпадения из доменных служб Active Directory (AD DS) или из папки "Контакты" в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-104">Learn how to use the EWS Managed API or EWS to resolve ambiguous names by getting possible matches from Active Directory Domain Services (AD DS) or a contacts folder in your user's mailbox.</span></span>
  
<span data-ttu-id="fc1e1-105">Пользователю в вашей организации предоставляется письменный список имен и адресов для сотрудников, которые проводят обучающий сеанс.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-105">A user in your organization is given a hand-written list of names and addresses for employees that attended a training session.</span></span> <span data-ttu-id="fc1e1-106">Они хотят отправить сообщение электронной почты с дополнительными сведениями о пользователях в списке, но не могут прочитать адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-106">They want to send an email with some additional information to people on the list, but they can't read everyone's email address.</span></span> <span data-ttu-id="fc1e1-107">Если вы хотите решить эту проблему для пользователей в вашем приложении, EWS поможет.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-107">If you want to solve this problem for your users in your application, EWS can help.</span></span> <span data-ttu-id="fc1e1-108">Можно использовать метод управляемого API [ExchangeService. ресолвенаме](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS или [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS для возврата списка потенциальных совпадений для выделенного текста, например части фамилии.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-108">You can use the [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API method or the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to return a list of potential matches for a selection of text, such as part of a last name.</span></span> <span data-ttu-id="fc1e1-109">Возвращаемые элементы могут быть общедоступными почтовыми ящиками пользователей, группами рассылки и контактами.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-109">The returned items can be public user mailboxes, distribution groups, and contacts.</span></span> 
  
<span data-ttu-id="fc1e1-110">Обратите внимание, что Exchange сохраняет адреса электронной почты с предфиксированными типами маршрутизации, такими как SMTP или SIP, в массиве с несколькими значениями.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-110">Note that Exchange saves email addresses with prefixed routing types, such as smtp or sip, in a multivalue array.</span></span> <span data-ttu-id="fc1e1-111">Метод **ресолвенаме** и операция **ResolveNames** выполняют частичное соответствие с каждым значением этого массива при добавлении типа маршрутизации в начале неизвестного имени, например "SIP: Пользователь1".</span><span class="sxs-lookup"><span data-stu-id="fc1e1-111">The **ResolveName** method and the **ResolveNames** operation perform a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1".</span></span> <span data-ttu-id="fc1e1-112">Если не указать тип маршрутизации, метод или операция по умолчанию будут использовать SMTP, сопоставлять их с основным свойством SMTP-адреса, а не выполнять поиск по многозначному массиву.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-112">If you don't specify a routing type, the method or operation will default to smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> <span data-ttu-id="fc1e1-113">Например, если вы ищете Пользователь1 и не включили префикс SIP, вы не будете получать sip:User1@Contoso.com в результате, даже если это действительный почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-113">For example, if you search for User1 and do not include the sip prefix, you will not receive sip:User1@Contoso.com as a result, even if that is a valid mailbox.</span></span> 
  
<span data-ttu-id="fc1e1-114">В одном запросе можно указать только одно неоднозначное имя.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-114">You can only specify one ambiguous name in a single request.</span></span> <span data-ttu-id="fc1e1-115">Если у вас есть список неоднозначных имен для разрешения, вам потребуется перебрать список и вызвать метод или операцию для каждой записи.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-115">If you have a list of ambiguous names to resolve, you will need to loop through the list and call the method or operation for each entry.</span></span> <span data-ttu-id="fc1e1-116">Для кандидатов из папки контактов пользователя будет задано значение идентификатора элемента, отличное от NULL, которое затем можно использовать в запросе метода [Contact. Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) или операции [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-116">Candidates from a user's Contacts folder will have a non-null item ID value, which can then be used in a [Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) method call or [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request to retrieve additional information.</span></span> <span data-ttu-id="fc1e1-117">Если кандидат является группой рассылки, для получения списка элементов можно использовать метод управляемого API [ExpandGroup (ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) EWS или [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-117">If the candidate is a distribution group, you can use the [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS operation to get the list of members.</span></span> <span data-ttu-id="fc1e1-118">Если для параметра _ретурнконтактдетаилс_ или атрибута **ретурнфуллконтактдата** EWS задано значение true, записи Active Directory, возвращаемые с помощью метода **ресолвенаме** или операции **ResolveNames** , будут включать дополнительные свойства, описывающие контакт.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-118">If the  _returnContactDetails_ parameter or the **ReturnFullContactData** EWS attribute is set to true, Active Directory entries returned via a **ResolveName** method or **ResolveNames** operation will include additional properties that describe the contact.</span></span> <span data-ttu-id="fc1e1-119">Параметр _ретурнконтактдетаилс_ или атрибут **ретурнфуллконтактдата** не влияет на данные, возвращаемые для контактов и групп контактов.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-119">The  _returnContactDetails_ parameter or the **ReturnFullContactData** attribute does not affect the data that is returned for contacts and contact groups.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a><span data-ttu-id="fc1e1-120">Разрешение неоднозначных имен с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="fc1e1-120">Resolve ambiguous names by using EWS Managed API</span></span>
<span data-ttu-id="fc1e1-121"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fc1e1-121"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="fc1e1-122">Метод [ресолвенаме](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) можно использовать для поиска кандидатов, которые соответствуют неоднозначному имени, которое вы передавали.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-122">You can use the [ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) method to find candidates that match the ambiguous name you pass.</span></span> <span data-ttu-id="fc1e1-123">С помощью перегрузок метода **ресолвенаме** можно выполнять поиск кандидатов пять различными способами.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-123">You can use overloads of the **ResolveName** method to search for candidates in five different ways.</span></span> 
  
<span data-ttu-id="fc1e1-124">**Таблица 1. Перегруженные методы Ресолвенаме**</span><span class="sxs-lookup"><span data-stu-id="fc1e1-124">**Table 1. Overloaded ResolveName methods**</span></span>

|<span data-ttu-id="fc1e1-125">**Метод**</span><span class="sxs-lookup"><span data-stu-id="fc1e1-125">**Method**</span></span>|<span data-ttu-id="fc1e1-126">**Принцип работы**</span><span class="sxs-lookup"><span data-stu-id="fc1e1-126">**How it works**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc1e1-127">Ресолвенаме (строка)</span><span class="sxs-lookup"><span data-stu-id="fc1e1-127">ResolveName(String)</span></span>](http://msdn.microsoft.com/en-us/library/dd635548%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="fc1e1-128">Поиск контактов в папке "Контакты" пользователя и глобальном списке адресов (GAL) в указанном порядке.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-128">Finds contacts in the user's Contacts folder and the Global Address List (GAL) — in that order.</span></span> <span data-ttu-id="fc1e1-129">Строковая переменная — это неоднозначное имя, которое вы пытаетесь разрешить.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-129">The string variable is the ambiguous name you are trying to resolve.</span></span>  <br/> |
|[<span data-ttu-id="fc1e1-130">Ресолвенаме (String, Ресолвенамесеарчлокатион, Boolean)</span><span class="sxs-lookup"><span data-stu-id="fc1e1-130">ResolveName(String, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/en-us/library/dd634595%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="fc1e1-131">Поиск контактов в папке "Контакты" по умолчанию и/или глобальном списке адресов (GAL).</span><span class="sxs-lookup"><span data-stu-id="fc1e1-131">Finds contacts in the default Contacts folder and/or the Global Address List (GAL).</span></span> <span data-ttu-id="fc1e1-132">Строковое значение — это неоднозначное имя, место поиска указывает папку контактов и/или глобальный список адресов, а логическое значение указывает, следует ли возвратить полные контактные данные.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-132">The string value is the ambiguous name, the search location specifies the Contacts folder and/or the GAL, and the Boolean value indicates whether to return the full contact information.</span></span>  <br/> |
|[<span data-ttu-id="fc1e1-133">Ресолвенаме (String, Ресолвенамесеарчлокатион, Boolean, свойство)</span><span class="sxs-lookup"><span data-stu-id="fc1e1-133">ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/en-us/library/hh532803%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="fc1e1-134">Поиск контактов в папке "Контакты" по умолчанию и/или глобальном списке адресов (GAL).</span><span class="sxs-lookup"><span data-stu-id="fc1e1-134">Finds contacts in the default Contacts folder and/or Global Address List (GAL).</span></span> <span data-ttu-id="fc1e1-135">Этот метод позволяет задать возвращаемые свойства.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-135">This method enables you to set the properties that are returned.</span></span>  <br/> |
|[<span data-ttu-id="fc1e1-136">Ресолвенаме (String, IEnumerable\<FolderId\>, ресолвенамесеарчлокатион, Boolean)</span><span class="sxs-lookup"><span data-stu-id="fc1e1-136">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/en-us/library/dd636014%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="fc1e1-137">Поиск контактов в указанных папках контактов и/или глобальном списке адресов (GAL).</span><span class="sxs-lookup"><span data-stu-id="fc1e1-137">Finds contacts in specified contact folders and/or the Global Address List (GAL).</span></span> <span data-ttu-id="fc1e1-138">Этот метод можно использовать для передачи коллекции папок для поиска.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-138">You can use this method to pass a collection of folders to search.</span></span> <span data-ttu-id="fc1e1-139">Это позволяет искать в папках контактов, отличных от папки контактов по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-139">This enables you to look in contact folders other than the default Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="fc1e1-140">Ресолвенаме (String, IEnumerable\<FolderId\>, Ресолвенамесеарчлокатион, Boolean, свойство)</span><span class="sxs-lookup"><span data-stu-id="fc1e1-140">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/en-us/library/hh532581%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="fc1e1-141">Поиск контактов в глобальном списке адресов (GAL) и/или в определенных папках контактов.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-141">Finds contacts in the Global Address List (GAL) and/or in specific contact folders.</span></span> <span data-ttu-id="fc1e1-142">Этот метод позволяет задать возвращаемые свойства.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-142">This method enables you to set the properties that are returned.</span></span>  <br/> |
   
<span data-ttu-id="fc1e1-143">Начнем с простого примера.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-143">Let's start with a simple example.</span></span> <span data-ttu-id="fc1e1-144">В приведенном ниже примере показано, как разрешить текстовую строку "" "") и вывести имя и адрес электронной почты каждого найденного кандидата.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-144">The following example shows how to resolve the text string "dan" and output the name and email address of each candidate found.</span></span> <span data-ttu-id="fc1e1-145">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Resolve the ambiguous name "dan".
   NameResolutionCollection resolvedNames = service.ResolveName("dan");
   // Output the list of candidates.
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

<span data-ttu-id="fc1e1-146">Ответ возвращает максимум 100 кандидатов, хотя может быть более 100 потенциальных кандидатов.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-146">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates.</span></span> <span data-ttu-id="fc1e1-147">Чтобы определить, были ли возвращены только первые 100 кандидатов большего числа кандидатов, проверьте значение параметра [инклудесаллресолутионс](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) в объекте [намересолутионколлектион](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fc1e1-147">To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of [IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) in the [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="fc1e1-148">Если задано значение true, возможны невероятные варианты. Если значение равно false, метод возвращает только первые 100 с большим количеством потенциальных кандидатов.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-148">If the value is true, there are no more possible candidates; if the value is false, the method only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="fc1e1-149">Если вы работаете в крупной организации, вероятно, что имя, например "" "" "" ", будет возвращать максимальное число кандидатов 100.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-149">If you work in a large organization, it's likely that a name like "dan" will return the maximum number of 100 candidates.</span></span> <span data-ttu-id="fc1e1-150">Чтобы уменьшить количество возвращаемых кандидатов, Ограничьте поиск.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-150">To reduce the number of candidates returned, limit where you search.</span></span> <span data-ttu-id="fc1e1-151">В следующем примере показано, как использовать перечисление [ресолвенамесеарчлокатион](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) , чтобы указать, где искать для устранения неоднозначного имени.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-151">The next example uses the [ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) enumeration to specify where to search to resolve the ambiguous name.</span></span> 
  
```cs
// Resolve the ambiguous name "dan".
// Only use the Contacts folder.
   NameResolutionCollection resolvedNames = service.ResolveName("dan", ResolveNameSearchLocation.ContactsOnly, false);
   // Output the list of candidates.   
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

<span data-ttu-id="fc1e1-152">Если вы храните контакты в папке, отличной от общеизвестных контактов, используйте один из перегруженных методов, чтобы указать, где искать кандидатов.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-152">If you store your contacts in a folder other than the well-known Contacts folder, use one of the overloaded methods to specify where to look for candidates.</span></span> <span data-ttu-id="fc1e1-153">В следующем примере создается список папок для метода **ресолвенаме** на основе идентификатора папки.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-153">The following example creates a folder list for the **ResolveName** method based on the folder ID.</span></span> <span data-ttu-id="fc1e1-154">**FolderId** был сокращен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-154">The **FolderId** has been shortened for readability.</span></span> 
  
```cs
// Create a list to store folders to search.
List<FolderId> folders = new List<FolderId>();
// Add a folder to the list based on the FolderId.
folders.Add(new FolderId("AABR8mboAAA="));
// Resolve the ambiguous name "dan".
// Only use the folders specified.
NameResolutionCollection resolvedNames = service.ResolveName("dan", folders, ResolveNameSearchLocation.ContactsOnly, false);
   foreach (NameResolution nameRes in resolvedNames)
   {
      Console.WriteLine("Contact name: " + nameRes.Mailbox.Name);
      Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
      Console.WriteLine("Mailbox type: " + nameRes.Mailbox.MailboxType);
   }

```

<span data-ttu-id="fc1e1-155">Если вы применяете фильтры и не возвращаете кандидатов, [намересолутионколлектион](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) будет содержать нулевые записи.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-155">If you apply filters and no candidates are returned, the [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) will contain zero entries.</span></span> <span data-ttu-id="fc1e1-156">Это можно проверить, просмотрев свойство [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) коллекции.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-156">You can verify this by looking at the [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) property of the collection.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a><span data-ttu-id="fc1e1-157">Разрешение неоднозначных имен с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="fc1e1-157">Resolve ambiguous names by using EWS</span></span>
<span data-ttu-id="fc1e1-158"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fc1e1-158"><a name="bk_EWSMA"> </a></span></span>

<span data-ttu-id="fc1e1-159">Вы можете использовать операцию [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS для определения возможных кандидатов на неоднозначное имя.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-159">You can use the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to identify possible candidates for an ambiguous name.</span></span> <span data-ttu-id="fc1e1-160">Элемент [унресолведентри](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) содержит неоднозначное имя, которое требуется разрешить.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-160">The [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) element contains the ambiguous name you want to resolve.</span></span> <span data-ttu-id="fc1e1-161">В приведенном ниже примере показано, как разрешить имя Ольга.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-161">The following example shows how to resolve the name Sadie.</span></span> <span data-ttu-id="fc1e1-162">Это также запрос XML, который использует управляемый API EWS при [использовании метода ресолвенаме](#bk_EWSMA), за исключением того, что для допустимых выходных примеров используется другое имя.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-162">This is also the XML request that the EWS Managed API uses when you [use the ResolveName method](#bk_EWSMA), except that it uses a different name for valid output examples.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ResolveNames xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                  ReturnFullContactData="true">
      <UnresolvedEntry>Sadie</UnresolvedEntry>
    </ResolveNames>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="fc1e1-163">Ответ возвращает максимум 100 кандидатов, 100 хотя для определения того, были ли возвращены только первые 100 кандидатов с большим количеством кандидатов, следует проверить значение атрибута [инклудесластитеминранже](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) элемента [Resolution](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fc1e1-163">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of the [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) attribute of the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="fc1e1-164">Если задано значение true, возможны невероятные варианты. Если значение равно false, операция возвращает только первые 100 с большим количеством потенциальных кандидатов.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-164">If the value is true, there are no more possible candidates; if the value is false, the operation only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="fc1e1-165">В следующем примере показан ответ XML при обнаружении одного кандидата.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-165">The following example shows the XML response when one candidate is found.</span></span> <span data-ttu-id="fc1e1-166">Помните [, что дочерний элемент может](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) содержать до 100 кандидатов, каждый из которых представлен элементом [разрешения](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) и его дочерними элементами.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-166">Remember, the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) can contain up to 100 candidates, each one represented by the [Resolution](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) element and its child elements.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>Sadie@Contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">SMTP:Sadie@Contoso.com</t:Entry>
                </t:EmailAddresses>
                <t:ContactSource>ActiveDirectory</t:ContactSource>
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="fc1e1-167">Вы не всегда собираетесь с кандидатами на неоднозначное имя.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-167">You're not always going to come up with candidates for your ambiguous name.</span></span> <span data-ttu-id="fc1e1-168">В следующем примере показан ответ XML в виде ошибки, если кандидатов не найдено.</span><span class="sxs-lookup"><span data-stu-id="fc1e1-168">The following example shows the XML response, as an error, when no candidates are found.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Error">
          <m:MessageText>No results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionNoResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </ResolveNamesResponse>
  </soap:Body>
</soap:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="fc1e1-169">См. также</span><span class="sxs-lookup"><span data-stu-id="fc1e1-169">See also</span></span>


- [<span data-ttu-id="fc1e1-170">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="fc1e1-170">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="fc1e1-171">Как: развернуть группы рассылки с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="fc1e1-171">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

