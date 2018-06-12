---
title: Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Узнайте, как с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange разверните группу рассылки.
ms.openlocfilehash: 0f9186fb71b3005c71a70e89aafb674ae15e4814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761000"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a><span data-ttu-id="fe262-103">Разверните узел группы рассылки с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="fe262-103">Expand distribution groups by using EWS in Exchange 2013</span></span>

<span data-ttu-id="fe262-104">Узнайте, как с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange разверните группу рассылки.</span><span class="sxs-lookup"><span data-stu-id="fe262-104">Learn how to expand a distribution group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="fe262-105">Можно использовать метод управляемый API EWS [ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) или операция [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) веб-служб Exchange разверните группу рассылки для идентификации всех получателей.</span><span class="sxs-lookup"><span data-stu-id="fe262-105">You can use the [ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS operation to expand a distribution group to identify all recipients.</span></span> 
  
<span data-ttu-id="fe262-106">Так как метод [ExpandGroup](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) перегружен, его можно вызвать несколькими способами:</span><span class="sxs-lookup"><span data-stu-id="fe262-106">Because the [ExpandGroup](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) method is overloaded, you can call it in several ways:</span></span> 
  
- <span data-ttu-id="fe262-107">[ExpandGroup(String)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx) - расширяет группу, определенную SMTP-адрес.</span><span class="sxs-lookup"><span data-stu-id="fe262-107">[ExpandGroup(String)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address.</span></span> 
    
- <span data-ttu-id="fe262-108">[ExpandGroup(EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) - расширяет группу, определенную с адресом электронной почты.</span><span class="sxs-lookup"><span data-stu-id="fe262-108">[ExpandGroup(EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) - Expands a group identified by an email address.</span></span> 
    
- <span data-ttu-id="fe262-109">[ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) - расширяет группу, определенную группу ID.</span><span class="sxs-lookup"><span data-stu-id="fe262-109">[ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) - Expands a group identified by a group ID.</span></span> 
    
- <span data-ttu-id="fe262-110">[ExpanGroup (строка, строка)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx) - расширяет группу, определенную SMTP-адреса и типа маршрутизации этот адрес.</span><span class="sxs-lookup"><span data-stu-id="fe262-110">[ExpanGroup(String, String)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address and the routing type of that address.</span></span> 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a><span data-ttu-id="fe262-111">Разверните узел универсальная группа рассылки или группу безопасности с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="fe262-111">Expand a universal distribution group or security group by using EWS Managed API</span></span>
<span data-ttu-id="fe262-112"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fe262-112"></span></span>

<span data-ttu-id="fe262-113">Следующий пример демонстрирует разверните универсальная группа рассылки или группу безопасности, используя адрес электронной почты, которая наиболее простой способ.</span><span class="sxs-lookup"><span data-stu-id="fe262-113">The following example shows how to expand a universal distribution group or security group by using an email address, which is the simplest approach.</span></span> <span data-ttu-id="fe262-114">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe262-114">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

<span data-ttu-id="fe262-115">Который не является большой объем кода, но они также довольно просто и может не предоставить требуется найти.</span><span class="sxs-lookup"><span data-stu-id="fe262-115">That's not a lot of code, but it's also pretty basic and might not give you what you are looking for.</span></span> <span data-ttu-id="fe262-116">Давайте сделать его шаг дальнейшей.</span><span class="sxs-lookup"><span data-stu-id="fe262-116">So let's take it a step further.</span></span> <span data-ttu-id="fe262-117">Группы рассылки также может содержать другие группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="fe262-117">Distribution groups can also contain other distribution groups.</span></span> <span data-ttu-id="fe262-118">Просто он был развернут вывода адрес электронной почты группы рассылки автономные но не раскрывать их.</span><span class="sxs-lookup"><span data-stu-id="fe262-118">Simply expanding it will output the email address of the contained distribution groups but not expand them.</span></span> <span data-ttu-id="fe262-119">Путем добавления еще на несколько строк кода, можно рекурсивно развернуть группы выводить все контакты.</span><span class="sxs-lookup"><span data-stu-id="fe262-119">By adding a few more lines of code, you can recursively expand the groups to output every contact.</span></span>
  
```cs
private static void ExpandDistributionLists(ExchangeService service, string Mailbox)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(Mailbox);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         // Check to see if the mailbox is a public group
         if (address.MailboxType == MailboxType.PublicGroup)
      {
         // Call the function again to expand the contained
         // distribution group.
         ExpandDistributionLists(service, address.Address);
      }
      else
      {
         // Output the address of the mailbox.
         Console.WriteLine("Email Address: {0}", address);
      }
   }
}

```

<span data-ttu-id="fe262-120">И теперь можно вызвать этой новой функции вашего кода и развернуть все группы рассылки общедоступных, содержащихся в первый.</span><span class="sxs-lookup"><span data-stu-id="fe262-120">And now you can call this new function in the your code and expand all the public distribution groups contained within the first one.</span></span>
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a><span data-ttu-id="fe262-121">Разверните группу контактов с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="fe262-121">Expand a contact group by using EWS Managed API</span></span>
<span data-ttu-id="fe262-122"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fe262-122"></span></span>

<span data-ttu-id="fe262-123">Так как группы контактов отсутствует адрес связанной электронной почты, вам нужно разверните группу на основании ItemId с помощью метода [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fe262-123">Because contact groups do not have an associated email address, you need to expand the group based on the ItemId by using the [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="fe262-124">Создание функции, как показано в предыдущем примере и измените второй тип параметра из строки на [идентификатор элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="fe262-124">You can create a function, as shown in the previous example, and change the second parameter type from a string to an [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span></span>
  
```cs
private static void ExpandContactGroup(ExchangeService service, ItemId groupID)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(groupID);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         if (address.MailboxType == MailboxType.PublicGroup)
         {
            ExpandDistributionLists(service, address.Address);
         }
         else
         {
            Console.WriteLine("Email Address: {0}", address);
         }
      }
}
```

<span data-ttu-id="fe262-125">Теперь можно вызвать эту функцию с помощью объекта службы Exchange и **ItemId** группы контактов.</span><span class="sxs-lookup"><span data-stu-id="fe262-125">Now you can call this function by using the Exchange service object and the **ItemId** of the contact group.</span></span> <span data-ttu-id="fe262-126">Обратите внимание на то, что **идентификатор элемента** в примере — это сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="fe262-126">Note that the **ItemId** in the example is shortened for readability.</span></span> 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a><span data-ttu-id="fe262-127">Разверните узел универсальная группа рассылки или группу безопасности с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="fe262-127">Expand a universal distribution group or security group by using EWS</span></span>
<span data-ttu-id="fe262-128"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fe262-128"></span></span>

<span data-ttu-id="fe262-129">В следующем примере показано сообщение запроса XML, передаче от клиента к серверу при использовании операции [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="fe262-129">The following example shows the XML request message that is sent from the client to the server when you use the [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="fe262-130">Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API веб-служб Exchange разверните [Универсальная группа рассылки](#bk_ExpandDGEWSMA).</span><span class="sxs-lookup"><span data-stu-id="fe262-130">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [expand a universal distribution group](#bk_ExpandDGEWSMA).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>employees@contoso.com</t:EmailAddress>
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="fe262-131">В следующем примере показано XML ответное сообщение, которое отправляется с сервера.</span><span class="sxs-lookup"><span data-stu-id="fe262-131">The following example shows the XML response message that is sent from the server to the client.</span></span> <span data-ttu-id="fe262-132">Обратите внимание на то, что возвращаются почтовых ящиков и универсальные группы рассылки.</span><span class="sxs-lookup"><span data-stu-id="fe262-132">Notice that both mailboxes and universal distribution groups are returned.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Support</Name>
          <EmailAddress>support@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
      </DLExpansion>
    </ExpandDLResponseMessage>
  </ResponseMessages>
</ExpandDLResponse>
</s:Body>
</s:Envelope>
```

<span data-ttu-id="fe262-133">В отличие от при использовании управляемый API веб-служб Exchange при использовании веб-служб Exchange разверните универсальная группа рассылки, вы не можете рекурсивно расширять группы рассылки, которые возвращаются.</span><span class="sxs-lookup"><span data-stu-id="fe262-133">Unlike when you use the EWS Managed API, when you use EWS to expand a universal distribution group, you can't recursively expand the distribution groups that are returned.</span></span> <span data-ttu-id="fe262-134">Необходимо будет отправить дополнительного запроса развернуть каждый из группы рассылки, включенных в ответ.</span><span class="sxs-lookup"><span data-stu-id="fe262-134">You will need to send an additional request to expand each of the distribution groups included in the response.</span></span>
  
## <a name="expand-a-contact-group-by-using-ews"></a><span data-ttu-id="fe262-135">Разверните группу контактов с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="fe262-135">Expand a contact group by using EWS</span></span>
<span data-ttu-id="fe262-136"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="fe262-136"></span></span>

<span data-ttu-id="fe262-137">В запросе XML, чтобы развернуть группу контактов похож на запрос, чтобы развернуть группу рассылки.</span><span class="sxs-lookup"><span data-stu-id="fe262-137">The XML request to expand a contact group is similar to a request to expand a distribution group.</span></span> <span data-ttu-id="fe262-138">Вместо адреса электронной почты используйте [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) группы контактов.</span><span class="sxs-lookup"><span data-stu-id="fe262-138">Instead of an email address, you use the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the contact group.</span></span> <span data-ttu-id="fe262-139">**Идентификатор элемента** в этом примере сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="fe262-139">The **ItemId** in this example is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="fe262-140">Структура XML-ответ на запрос, чтобы развернуть группу контактов — это то же, что ответ на запрос, чтобы развернуть универсальная группа рассылки.</span><span class="sxs-lookup"><span data-stu-id="fe262-140">The structure of the XML response to a request to expand a contact group is the same as the response to a request to expand a universal distribution group.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="fe262-141">См. также</span><span class="sxs-lookup"><span data-stu-id="fe262-141">See also</span></span>


- [<span data-ttu-id="fe262-142">Группы рассылки и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="fe262-142">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="fe262-143">Создание группы контактов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fe262-143">Create contact groups by using EWS in Exchange</span></span>](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

