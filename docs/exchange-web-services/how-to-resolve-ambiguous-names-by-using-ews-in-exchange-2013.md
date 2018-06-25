---
title: Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 1ba21c54-ecd2-4a1e-80d4-0f4171dea84f
description: Узнайте, как использовать управляемый API EWS или веб-служб Exchange для разрешения неоднозначных имен, получив возможные варианты из доменных служб Active Directory (AD DS) или папку контактов в почтовом ящике пользователя.
ms.openlocfilehash: 05a88043083a27d2e6d445cd71e5f3919c5a775d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761105"
---
# <a name="resolve-ambiguous-names-by-using-ews-in-exchange-2013"></a><span data-ttu-id="8b222-103">Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8b222-103">Resolve ambiguous names by using EWS in Exchange 2013</span></span>

<span data-ttu-id="8b222-104">Узнайте, как использовать управляемый API EWS или веб-служб Exchange для разрешения неоднозначных имен, получив возможные варианты из доменных служб Active Directory (AD DS) или папку контактов в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="8b222-104">Learn how to use the EWS Managed API or EWS to resolve ambiguous names by getting possible matches from Active Directory Domain Services (AD DS) or a contacts folder in your user's mailbox.</span></span>
  
<span data-ttu-id="8b222-105">Пользователь в вашей организации, получает рукописное список имен и адресов для сотрудников, которые посетившие обучения.</span><span class="sxs-lookup"><span data-stu-id="8b222-105">A user in your organization is given a hand-written list of names and addresses for employees that attended a training session.</span></span> <span data-ttu-id="8b222-106">Требуется отправить сообщение электронной почты с некоторые дополнительные сведения для пользователей в списке, но они не могут читать все адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8b222-106">They want to send an email with some additional information to people on the list, but they can't read everyone's email address.</span></span> <span data-ttu-id="8b222-107">Если необходимо решить эту проблему для пользователей в приложении, может помочь веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b222-107">If you want to solve this problem for your users in your application, EWS can help.</span></span> <span data-ttu-id="8b222-108">Чтобы возвратить список возможных соответствий для выбора текста, такие как часть имени последнего можно использовать метод управляемый API EWS [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) или [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b222-108">You can use the [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) EWS Managed API method or the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to return a list of potential matches for a selection of text, such as part of a last name.</span></span> <span data-ttu-id="8b222-109">Возвращаемых элементов может быть почтовые ящики пользователей общедоступных служб, группы рассылки и контакты.</span><span class="sxs-lookup"><span data-stu-id="8b222-109">The returned items can be public user mailboxes, distribution groups, and contacts.</span></span> 
  
<span data-ttu-id="8b222-110">Обратите внимание на то, что Exchange сохраняет адреса электронной почты с с префиксами типов маршрутизации, например smtp или sip в массиве нескольких значений.</span><span class="sxs-lookup"><span data-stu-id="8b222-110">Note that Exchange saves email addresses with prefixed routing types, such as smtp or sip, in a multivalue array.</span></span> <span data-ttu-id="8b222-111">Метод **ResolveName** и операции **ResolveNames** выполните частичное соответствие каждого значения этого массива при добавлении типа маршрутизации в начале неизвестное имя, например, «sip: User1».</span><span class="sxs-lookup"><span data-stu-id="8b222-111">The **ResolveName** method and the **ResolveNames** operation perform a partial match against each value of that array when you add the routing type at the beginning of the unresolved name, such as "sip:User1".</span></span> <span data-ttu-id="8b222-112">Если не указать тип маршрутизации, метод или операция будет по умолчанию установлено равным smtp, соответствует свойству основной адрес smtp и поиск нескольких значений массива.</span><span class="sxs-lookup"><span data-stu-id="8b222-112">If you don't specify a routing type, the method or operation will default to smtp, match it to a primary smtp address property, and not search the multivalue array.</span></span> <span data-ttu-id="8b222-113">К примеру Если поиск User1 и не используйте код sip не появится sip:User1@Contoso.com в результате даже в том случае, если это допустимый почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8b222-113">For example, if you search for User1 and do not include the sip prefix, you will not receive sip:User1@Contoso.com as a result, even if that is a valid mailbox.</span></span> 
  
<span data-ttu-id="8b222-114">В одном запросе можно указать только одного неоднозначное имя.</span><span class="sxs-lookup"><span data-stu-id="8b222-114">You can only specify one ambiguous name in a single request.</span></span> <span data-ttu-id="8b222-115">Если у вас есть список неоднозначные имена для решения, необходимо цикл по списку и вызовите метод или операции для каждой записи.</span><span class="sxs-lookup"><span data-stu-id="8b222-115">If you have a list of ambiguous names to resolve, you will need to loop through the list and call the method or operation for each entry.</span></span> <span data-ttu-id="8b222-116">Кандидатов из папки Контакты будут иметь значение идентификатора элемента ненулевое, которую можно использовать в вызове метода [Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) или запрос операции [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) для получения дополнительных сведений.</span><span class="sxs-lookup"><span data-stu-id="8b222-116">Candidates from a user's Contacts folder will have a non-null item ID value, which can then be used in a [Contact.Bind](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) method call or [GetItem](http://msdn.microsoft.com/library/769df8eb-9c72-48b5-a49f-82c6b86bc5fc%28Office.15%29.aspx) operation request to retrieve additional information.</span></span> <span data-ttu-id="8b222-117">Если объект группы рассылки, можно использовать операцию EWS [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) или метод [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) управляемый API EWS для получения списка элементов.</span><span class="sxs-lookup"><span data-stu-id="8b222-117">If the candidate is a distribution group, you can use the [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/affe84a5-ad98-4aba-83f4-8732938b763d%28Office.15%29.aspx) EWS operation to get the list of members.</span></span> <span data-ttu-id="8b222-118">Если параметр _returnContactDetails_ или **ReturnFullContactData** EWS атрибута задано значение true, возвращаемых записей Active Directory с помощью метода **ResolveName** или **ResolveNames** операция будет включать дополнительные свойства описывающие контакт.</span><span class="sxs-lookup"><span data-stu-id="8b222-118">If the  _returnContactDetails_ parameter or the **ReturnFullContactData** EWS attribute is set to true, Active Directory entries returned via a **ResolveName** method or **ResolveNames** operation will include additional properties that describe the contact.</span></span> <span data-ttu-id="8b222-119">Параметр _returnContactDetails_ или атрибут **ReturnFullContactData** не влияет на данные, возвращаемые для контактов и группы контактов.</span><span class="sxs-lookup"><span data-stu-id="8b222-119">The  _returnContactDetails_ parameter or the **ReturnFullContactData** attribute does not affect the data that is returned for contacts and contact groups.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews-managed-api"></a><span data-ttu-id="8b222-120">Разрешения неоднозначных имен с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8b222-120">Resolve ambiguous names by using EWS Managed API</span></span>
<span data-ttu-id="8b222-121"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8b222-121"></span></span>

<span data-ttu-id="8b222-122">Метод [ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) поиск кандидатов, которые соответствуют неоднозначное имя, передаваемого.</span><span class="sxs-lookup"><span data-stu-id="8b222-122">You can use the [ResolveName](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) method to find candidates that match the ambiguous name you pass.</span></span> <span data-ttu-id="8b222-123">Перегрузки метода **ResolveName** можно использовать для поиска кандидатов пять различными способами.</span><span class="sxs-lookup"><span data-stu-id="8b222-123">You can use overloads of the **ResolveName** method to search for candidates in five different ways.</span></span> 
  
<span data-ttu-id="8b222-124">**В таблице 1. Перегруженные методы ResolveName**</span><span class="sxs-lookup"><span data-stu-id="8b222-124">**Table 1. Overloaded ResolveName methods**</span></span>

|<span data-ttu-id="8b222-125">**Способ**</span><span class="sxs-lookup"><span data-stu-id="8b222-125">**Method**</span></span>|<span data-ttu-id="8b222-126">**Как это работает**</span><span class="sxs-lookup"><span data-stu-id="8b222-126">**How it works**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8b222-127">ResolveName(String)</span><span class="sxs-lookup"><span data-stu-id="8b222-127">ResolveName(String)</span></span>](http://msdn.microsoft.com/en-us/library/dd635548%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8b222-128">Поиск контактов в папке контактов пользователя и глобальный список адресов (GAL) — в указанном порядке.</span><span class="sxs-lookup"><span data-stu-id="8b222-128">Finds contacts in the user's Contacts folder and the Global Address List (GAL) — in that order.</span></span> <span data-ttu-id="8b222-129">Строковой переменной является неоднозначным имя, которое вы пытаетесь решить.</span><span class="sxs-lookup"><span data-stu-id="8b222-129">The string variable is the ambiguous name you are trying to resolve.</span></span>  <br/> |
|[<span data-ttu-id="8b222-130">ResolveName (строка, ResolveNameSearchLocation, Boolean)</span><span class="sxs-lookup"><span data-stu-id="8b222-130">ResolveName(String, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/en-us/library/dd634595%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8b222-131">Поиск контактов в папке контактов по умолчанию и/или глобального списка адресов (GAL).</span><span class="sxs-lookup"><span data-stu-id="8b222-131">Finds contacts in the default Contacts folder and/or the Global Address List (GAL).</span></span> <span data-ttu-id="8b222-132">Неоднозначное имя — это строковое значение, указывает расположение поиска папку Контакты и/или глобального списка адресов и логическое значение, которое указывает, нужно ли возвращать полное контактные данные.</span><span class="sxs-lookup"><span data-stu-id="8b222-132">The string value is the ambiguous name, the search location specifies the Contacts folder and/or the GAL, and the Boolean value indicates whether to return the full contact information.</span></span>  <br/> |
|[<span data-ttu-id="8b222-133">ResolveName (строка, ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="8b222-133">ResolveName(String, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/en-us/library/hh532803%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8b222-134">Поиск контактов в папке контактов по умолчанию и/или глобального списка адресов (GAL).</span><span class="sxs-lookup"><span data-stu-id="8b222-134">Finds contacts in the default Contacts folder and/or Global Address List (GAL).</span></span> <span data-ttu-id="8b222-135">Этот метод позволяет задать свойства, которые возвращаются.</span><span class="sxs-lookup"><span data-stu-id="8b222-135">This method enables you to set the properties that are returned.</span></span>  <br/> |
|[<span data-ttu-id="8b222-136">ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span><span class="sxs-lookup"><span data-stu-id="8b222-136">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean)</span></span>](http://msdn.microsoft.com/en-us/library/dd636014%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8b222-137">Поиск контактов в указанных папках контактов и/или глобального списка адресов (GAL).</span><span class="sxs-lookup"><span data-stu-id="8b222-137">Finds contacts in specified contact folders and/or the Global Address List (GAL).</span></span> <span data-ttu-id="8b222-138">Этот метод можно использовать для передачи коллекции папок для поиска.</span><span class="sxs-lookup"><span data-stu-id="8b222-138">You can use this method to pass a collection of folders to search.</span></span> <span data-ttu-id="8b222-139">Это позволяет искать в папки контактов, отличных от папки Контакты по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="8b222-139">This enables you to look in contact folders other than the default Contacts folder.</span></span>  <br/> |
|[<span data-ttu-id="8b222-140">ResolveName (String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span><span class="sxs-lookup"><span data-stu-id="8b222-140">ResolveName(String, IEnumerable\<FolderId\>, ResolveNameSearchLocation, Boolean, PropertySet)</span></span>](http://msdn.microsoft.com/en-us/library/hh532581%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8b222-141">Находит контакты в глобальном списке адресов (GAL) и/или в указанных папках контактов.</span><span class="sxs-lookup"><span data-stu-id="8b222-141">Finds contacts in the Global Address List (GAL) and/or in specific contact folders.</span></span> <span data-ttu-id="8b222-142">Этот метод позволяет задать свойства, которые возвращаются.</span><span class="sxs-lookup"><span data-stu-id="8b222-142">This method enables you to set the properties that are returned.</span></span>  <br/> |
   
<span data-ttu-id="8b222-143">Начнем с простого примера.</span><span class="sxs-lookup"><span data-stu-id="8b222-143">Let's start with a simple example.</span></span> <span data-ttu-id="8b222-144">Приведенный ниже показано, как устранить текстовая строка «Дэн» и вывода имя и адрес электронной почты каждого кандидата найден.</span><span class="sxs-lookup"><span data-stu-id="8b222-144">The following example shows how to resolve the text string "dan" and output the name and email address of each candidate found.</span></span> <span data-ttu-id="8b222-145">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="8b222-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="8b222-146">Ответ возвращается не более 100 кандидатов, несмотря на то, что может быть больше 100 потенциальных кандидатов.</span><span class="sxs-lookup"><span data-stu-id="8b222-146">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates.</span></span> <span data-ttu-id="8b222-147">Чтобы определить, возвращаются ли только первые 100 кандидатов большее число кандидатов, проверьте значение [IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) в объекте [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8b222-147">To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of [IncludesAllResolutions](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.includesallresolutions%28v=exchg.80%29.aspx) in the [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) object.</span></span> <span data-ttu-id="8b222-148">Если значение равно true, существует заканчивается возможных кандидатов; Если значение равно false, метод возвращается только первые 100 большего количества потенциальных кандидатов.</span><span class="sxs-lookup"><span data-stu-id="8b222-148">If the value is true, there are no more possible candidates; if the value is false, the method only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="8b222-149">При работе в крупной организации, скорее всего, что имя, например «Дэн» возвращает максимальное число 100 кандидатов.</span><span class="sxs-lookup"><span data-stu-id="8b222-149">If you work in a large organization, it's likely that a name like "dan" will return the maximum number of 100 candidates.</span></span> <span data-ttu-id="8b222-150">Чтобы уменьшить количество возвращаемых кандидатов, ограничение, где проводится поиск.</span><span class="sxs-lookup"><span data-stu-id="8b222-150">To reduce the number of candidates returned, limit where you search.</span></span> <span data-ttu-id="8b222-151">В следующем примере используется перечисление [ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) , чтобы указать, где поиска для разрешения неоднозначное имя.</span><span class="sxs-lookup"><span data-stu-id="8b222-151">The next example uses the [ResolveNameSearchLocation](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.resolvenamesearchlocation%28v=exchg.80%29.aspx) enumeration to specify where to search to resolve the ambiguous name.</span></span> 
  
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

<span data-ttu-id="8b222-152">Если сохранить контакты в папке, отличной от известных контакты, используйте одну из перегруженных методов чтобы указать, где следует искать кандидатов.</span><span class="sxs-lookup"><span data-stu-id="8b222-152">If you store your contacts in a folder other than the well-known Contacts folder, use one of the overloaded methods to specify where to look for candidates.</span></span> <span data-ttu-id="8b222-153">В следующем примере создается список папок для метода **ResolveName** на основании папки.</span><span class="sxs-lookup"><span data-stu-id="8b222-153">The following example creates a folder list for the **ResolveName** method based on the folder ID.</span></span> <span data-ttu-id="8b222-154">**FolderId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="8b222-154">The **FolderId** has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="8b222-155">Если нет кандидатов возвращаются и применение фильтров, [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) будет содержать ноль записей.</span><span class="sxs-lookup"><span data-stu-id="8b222-155">If you apply filters and no candidates are returned, the [NameResolutionCollection](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection%28v=exchg.80%29.aspx) will contain zero entries.</span></span> <span data-ttu-id="8b222-156">Вы можете проверить, посмотрев свойства [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) коллекции.</span><span class="sxs-lookup"><span data-stu-id="8b222-156">You can verify this by looking at the [Count](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.nameresolutioncollection.count%28v=exchg.80%29.aspx) property of the collection.</span></span> 
  
## <a name="resolve-ambiguous-names-by-using-ews"></a><span data-ttu-id="8b222-157">Разрешения неоднозначных имен с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8b222-157">Resolve ambiguous names by using EWS</span></span>
<span data-ttu-id="8b222-158"><a name="bk_EWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="8b222-158"></span></span>

<span data-ttu-id="8b222-159">Можно использовать операцию [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) веб-служб Exchange для определения возможных кандидатов для разрешения неоднозначных псевдонимов.</span><span class="sxs-lookup"><span data-stu-id="8b222-159">You can use the [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) EWS operation to identify possible candidates for an ambiguous name.</span></span> <span data-ttu-id="8b222-160">Элемент [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) содержит неоднозначное имя, которое требуется разрешить.</span><span class="sxs-lookup"><span data-stu-id="8b222-160">The [UnresolvedEntry](http://msdn.microsoft.com/library/5ac6116a-3b24-40f8-a877-dbe9a6935919%28Office.15%29.aspx) element contains the ambiguous name you want to resolve.</span></span> <span data-ttu-id="8b222-161">В следующем примере показано, как для разрешения имени Sadie.</span><span class="sxs-lookup"><span data-stu-id="8b222-161">The following example shows how to resolve the name Sadie.</span></span> <span data-ttu-id="8b222-162">Это также запроса XML, управляемый API EWS при можно [использовать метод ResolveName](#bk_EWSMA), за исключением того, он использует имя допустимого вывода примеры.</span><span class="sxs-lookup"><span data-stu-id="8b222-162">This is also the XML request that the EWS Managed API uses when you [use the ResolveName method](#bk_EWSMA), except that it uses a different name for valid output examples.</span></span>
  
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

<span data-ttu-id="8b222-163">Ответ возвращается не более 100 кандидатов, несмотря на то, что может быть больше 100 потенциальных кандидатов для определения, возвращаются ли только первые 100 кандидатов большее число кандидатов, проверьте значение [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) атрибут [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) элемента.</span><span class="sxs-lookup"><span data-stu-id="8b222-163">The response returns a maximum of 100 candidates, although there might be more than 100 potential candidates To determine whether only the first 100 candidates of a larger number of candidates were returned, check the value of the [IncludesLastItemInRange](http://msdn.microsoft.com/library/e7d6c7d3-548e-48b0-a313-bfef81e4832a%28Office.15%29.aspx) attribute of the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="8b222-164">Если значение равно true, существует заканчивается возможных кандидатов; Если значение равно false, операция возвращается только первые 100 большего количества потенциальных кандидатов.</span><span class="sxs-lookup"><span data-stu-id="8b222-164">If the value is true, there are no more possible candidates; if the value is false, the operation only returned the first 100 of a larger number of potential candidates.</span></span> 
  
<span data-ttu-id="8b222-165">В следующем примере показано XML-ответ при обнаружении одного кандидата.</span><span class="sxs-lookup"><span data-stu-id="8b222-165">The following example shows the XML response when one candidate is found.</span></span> <span data-ttu-id="8b222-166">Помните, что [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) может содержать до 100 кандидатов, каждый из которых представлена элемент [решение](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) и его дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="8b222-166">Remember, the [ResolutionSet](http://msdn.microsoft.com/library/43d5b876-0e87-4414-9b1d-bff1c1ec825c%28Office.15%29.aspx) can contain up to 100 candidates, each one represented by the [Resolution](http://msdn.microsoft.com/library/573bed4b-d7b1-4baf-b16f-0795cdebf1a7%28Office.15%29.aspx) element and its child elements.</span></span> 
  
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

<span data-ttu-id="8b222-167">Не всегда вы собираетесь обеспечиваемые кандидатов для неоднозначное имя.</span><span class="sxs-lookup"><span data-stu-id="8b222-167">You're not always going to come up with candidates for your ambiguous name.</span></span> <span data-ttu-id="8b222-168">В следующем примере показано XML-ответ, как ошибка, при обнаружении кандидатов.</span><span class="sxs-lookup"><span data-stu-id="8b222-168">The following example shows the XML response, as an error, when no candidates are found.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="8b222-169">См. также</span><span class="sxs-lookup"><span data-stu-id="8b222-169">See also</span></span>


- [<span data-ttu-id="8b222-170">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="8b222-170">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
    
- [<span data-ttu-id="8b222-171">Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="8b222-171">Expand distribution groups by using EWS in Exchange 2013</span></span>](how-to-expand-distribution-groups-by-using-ews-in-exchange-2013.md)
    

