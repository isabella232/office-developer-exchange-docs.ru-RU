---
title: Контакты доступа роли представителя с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Узнайте, как получить доступ к роли представителя контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 47540082f7e60645cae60fe2347e50e17cd226dd
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353723"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="acb00-103">Контакты доступа роли представителя с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-103">Access contacts as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="acb00-104">Узнайте, как получить доступ к роли представителя контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="acb00-104">Learn how to access contacts as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="acb00-105">Можно использовать управляемый API EWS или веб-служб Exchange для предоставления пользователю доступа к владельца почтового ящика папки «Контакты».</span><span class="sxs-lookup"><span data-stu-id="acb00-105">You can use the EWS Managed API or EWS to give a user access to a mailbox owner's Contacts folder.</span></span> <span data-ttu-id="acb00-106">Делегат может затем создание контактов от имени владельца почтового ящика и извлечения, обновление и удаление контактов из папки Контакты владельца почтового ящика, в зависимости от их разрешения.</span><span class="sxs-lookup"><span data-stu-id="acb00-106">The delegate can then create contacts on behalf of the mailbox owner, and retrieve, update, and delete contacts from the mailbox owner's Contacts folder, depending on their permissions.</span></span>
  
<span data-ttu-id="acb00-107">Роли представителя используйте ту же методов и операций для доступа владельца почтового ящика папки «Контакты», которая используется для доступа к папке контактов.</span><span class="sxs-lookup"><span data-stu-id="acb00-107">As a delegate, you use the same methods and operations to access a mailbox owner's Contacts folder that you use to access your own Contacts folder.</span></span> <span data-ttu-id="acb00-108">Основное различие —, что вам следует использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) для поиска или создание элемента контакта и затем после определения идентификатора элемента, можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновить или удалить элемент.</span><span class="sxs-lookup"><span data-stu-id="acb00-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a contact item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="acb00-109">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для доступа к контакту роли представителя**</span><span class="sxs-lookup"><span data-stu-id="acb00-109">**Table 1. EWS Managed API methods and EWS operations for accessing a contact as a delegate**</span></span>

|<span data-ttu-id="acb00-110">**Задача**</span><span class="sxs-lookup"><span data-stu-id="acb00-110">**If you want to…**</span></span>|<span data-ttu-id="acb00-111">**Используйте этот метод управляемый API EWS...**</span><span class="sxs-lookup"><span data-stu-id="acb00-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="acb00-112">**Используйте эту операцию EWS...**</span><span class="sxs-lookup"><span data-stu-id="acb00-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="acb00-113">Создание контакта в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="acb00-113">Create a contact as a delegate</span></span>  <br/> |<span data-ttu-id="acb00-114">[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке Контакты владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="acb00-114">[Item.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="acb00-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="acb00-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="acb00-116">Создание нескольких контактов в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="acb00-116">Create multiple contacts as a delegate</span></span>  <br/> |<span data-ttu-id="acb00-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке Контакты владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="acb00-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="acb00-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="acb00-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="acb00-119">Разрешить контакт роли представителя</span><span class="sxs-lookup"><span data-stu-id="acb00-119">Resolve a contact as a delegate</span></span>  <br/> |<span data-ttu-id="acb00-120">[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке Контакты владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="acb00-120">[ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="acb00-121">[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="acb00-121">[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="acb00-122">Поиск или найдите контакт роли представителя</span><span class="sxs-lookup"><span data-stu-id="acb00-122">Search for or find a contact as a delegate</span></span>  <br/> |<span data-ttu-id="acb00-123">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке Контакты владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="acb00-123">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="acb00-124">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="acb00-124">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="acb00-125">Получение контакт роли представителя</span><span class="sxs-lookup"><span data-stu-id="acb00-125">Get a contact as a delegate</span></span>  <br/> |[<span data-ttu-id="acb00-126">Contact.Bind</span><span class="sxs-lookup"><span data-stu-id="acb00-126">Contact.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="acb00-127">GetItem</span><span class="sxs-lookup"><span data-stu-id="acb00-127">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="acb00-128">Обновление контакт роли представителя</span><span class="sxs-lookup"><span data-stu-id="acb00-128">Update a contact as a delegate</span></span>  <br/> |<span data-ttu-id="acb00-129">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) , а затем [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="acb00-129">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="acb00-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="acb00-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="acb00-131">Удаление контакта в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="acb00-131">Delete a contact as a delegate</span></span>  <br/> |<span data-ttu-id="acb00-132">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) , а затем [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="acb00-132">[Contact.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="acb00-133">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="acb00-133">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="acb00-134">В примерах кода в этой статье primary@contoso.com — это владелец почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-134">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 

<span data-ttu-id="acb00-135"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="acb00-135"></span></span>

## <a name="prerequisite-tasks"></a><span data-ttu-id="acb00-136">Обязательные задачи</span><span class="sxs-lookup"><span data-stu-id="acb00-136">Prerequisite tasks</span></span>

<span data-ttu-id="acb00-137">Пользователь может получить доступ к папки контактов владельца почтового ящика для делегата, пользователь должен быть [добавлен в качестве делегата с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для папки «Контакты» владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-137">Before a user can access the mailbox owner's Contacts folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Contacts folder.</span></span> 

<span data-ttu-id="acb00-138"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="acb00-138"></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="acb00-139">Создание контактов как делегат с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-139">Create a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="acb00-140">Управляемый API EWS позволяет использовать объект службы для пользователя делегат для создания контактов для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-140">The EWS Managed API enables you to use the service object for the delegate user to create contacts for the mailbox owner.</span></span> <span data-ttu-id="acb00-141">В этом примере показано, как использовать метод [сохранения](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) для создания собрания и отправки приглашений на собрание участникам.</span><span class="sxs-lookup"><span data-stu-id="acb00-141">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="acb00-142">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) делегата и делегата предоставлены необходимые разрешения для папки «Контакты» владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-142">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Contacts folder.</span></span> 
  
```cs
 public static void DelegateAccessCreateContact(ExchangeService service)
{
    // Create the contact.
    Contact contact = new Contact(service);
    // Specify the name and how the contact should be filed.
    contact.GivenName = "Brian";
    contact.MiddleName = "David";
    contact.Surname = "Johnson";
    contact.FileAsMapping = FileAsMapping.SurnameCommaGivenName;
    // Specify the company name.
    contact.CompanyName = "Contoso";
    // Specify the business, home, and car phone numbers.
    contact.PhoneNumbers[PhoneNumberKey.BusinessPhone] = "425-555-0110";
    contact.PhoneNumbers[PhoneNumberKey.HomePhone] = "425-555-0120";
    contact.PhoneNumbers[PhoneNumberKey.CarPhone] = "425-555-0130";
    // Specify two email addresses.
    contact.EmailAddresses[EmailAddressKey.EmailAddress1] = 
        new EmailAddress("brian_1@contoso.com");
    contact.EmailAddresses[EmailAddressKey.EmailAddress2] = 
        new EmailAddress("brian_2@contoso.com");
    // Save the contact in the mailbox owner's Contacts folder.
    // This method call results in a CreateItem call to EWS. 
    // The contact identifier contains the context for the mailbox owner's 
    // Contact folder. Any additional actions take on this contact will 
    // be performed in the mailbox owner's mailbox. 
    contact.Save(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    // Verify that the contact was created.
    // This method call results in a GetItem call to EWS
    // to load the display name property on the contact. 
    contact.Load(new PropertySet (ContactSchema.DisplayName));
    Console.WriteLine("\nContact created: " + contact.DisplayName + "\n");
}
```

<span data-ttu-id="acb00-143">Обратите внимание, что при сохранении элемента вызова метода [Сохранить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) необходимо определить владельца почтового ящика папки «Контакты».</span><span class="sxs-lookup"><span data-stu-id="acb00-143">Note that when you save the item, the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="acb00-144">Если владелец почтового ящика папки «Контакты» не указан, запрос на собрание получает сохранены делегата папки «Контакты» и не владельца почтового ящика папки «Контакты».</span><span class="sxs-lookup"><span data-stu-id="acb00-144">If the mailbox owner's Contacts folder is not specified, the meeting request gets saved to the delegate's Contacts folder and not the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="acb00-145">В вызове метода **Сохранить** в двухстороннем может включать владельца почтового ящика папки «Контакты».</span><span class="sxs-lookup"><span data-stu-id="acb00-145">You can include the mailbox owner's Contacts folder in the **Save** method call in two way.</span></span> <span data-ttu-id="acb00-146">Рекомендуется создать новый экземпляр объекта [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) с помощью [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-146">We recommend that you instantiate a new instance of the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

<span data-ttu-id="acb00-147">Тем не менее, можно также [привязать](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) к папке контактов во-первых и затем используйте идентификатор папки в вызове метода **сохранения** .</span><span class="sxs-lookup"><span data-stu-id="acb00-147">However, you can also [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Contacts folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="acb00-148">Однако следует помнить, что при этом создается дополнительных вызовов веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="acb00-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<span data-ttu-id="acb00-149"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="acb00-149"></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="acb00-150">Создание контактов в качестве делегата с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-150">Create a contact as a delegate by using EWS</span></span>

<span data-ttu-id="acb00-151">Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для создания элементов контактов для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-151">EWS enables you to use the service object for the delegate user to create contact items for the mailbox owner.</span></span> <span data-ttu-id="acb00-152">В этом примере показано, как использовать операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания контакта.</span><span class="sxs-lookup"><span data-stu-id="acb00-152">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a contact.</span></span> 
  
<span data-ttu-id="acb00-153">Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **Сохранить** , чтобы [Создать контакт](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="acb00-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a contact](#bk_createewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Contact>
          <t:FileAsMapping>LastCommaFirst</t:FileAsMapping>
          <t:GivenName>Brian</t:GivenName>
          <t:MiddleName>David</t:MiddleName>
          <t:CompanyName>Contoso</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">brian_1@contoso.com</t:Entry>
            <t:Entry Key="EmailAddress2">brian_2@contoso.com</t:Entry>
          </t:EmailAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">425-555-0110</t:Entry>
            <t:Entry Key="HomePhone">425-555-0120</t:Entry>
            <t:Entry Key="CarPhone">425-555-0130</t:Entry>
          </t:PhoneNumbers>
          <t:Surname>Johnson</t:Surname>
        </t:Contact>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="acb00-154">Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что контакт был успешно создан.</span><span class="sxs-lookup"><span data-stu-id="acb00-154">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the contact was created successfully.</span></span> <span data-ttu-id="acb00-155">Ответ также содержит идентификатор только что созданный контакта.</span><span class="sxs-lookup"><span data-stu-id="acb00-155">The response also contains the item ID of the newly created contact.</span></span>

<span data-ttu-id="acb00-156"><a name="bk_resolveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="acb00-156"></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="acb00-157">Разрешить контакт роли представителя с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-157">Resolve a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="acb00-158">Поиск контакта на основе возможно неоднозначное имя или терминов, необходимо использовать один из методов [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) , включает параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , таким образом, можно указать папку Контакты владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-158">To find a contact based on a possibly ambiguous name or term, you must use one of the [ExchangeService.ResolveName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Contacts folder.</span></span> 
  
```cs
private static void DelegateAccessResolveContacts(ExchangeService service)
{
    // Create a list to store folders to search.
    List<FolderId> folders = new List<FolderId>();
   
    // Add the mailbox owner's folder to the list.
    folders.Add(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    
    // Resolve the ambiguous name "Johnson".
    // This method call results in a ResolveNames call to EWS.
    NameResolutionCollection resolvedNames = service.ResolveName(
        "johnson", folders, ResolveNameSearchLocation.ContactsOnly, true);
    // Output the list of candidate email addresses and contact names.
    foreach (NameResolution nameRes in resolvedNames)
    {
        Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
        Console.WriteLine("Contact ID: " + nameRes.Mailbox.Id);
    }
}
```

<span data-ttu-id="acb00-159">После вызова метода **ResolveNames** возвращает ответ с кодом, можно [получить, обновить или удалить контакт](#bk_getewsma) с помощью идентификатора и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;и необходимо указать SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-159">After the **ResolveNames** method call returns a response with an ID, you can [get, update or delete the contact](#bk_getewsma) using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="acb00-160"><a name="bk_resolveews"> </a></span><span class="sxs-lookup"><span data-stu-id="acb00-160"></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="acb00-161">Разрешения роли представителя контакта с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-161">Resolve a contact as a delegate by using EWS</span></span>

<span data-ttu-id="acb00-162">Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для разрешения имен частичное в папке контактов владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-162">EWS enables you to use the service object for the delegate user to resolve partial names in the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="acb00-163">В этом примере показано, как использовать операцию [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) Поиск собраний в владельца почтового ящика папки «Контакты», содержащие слово «johnson».</span><span class="sxs-lookup"><span data-stu-id="acb00-163">This example shows how to use the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Contacts folder that contain the word "johnson".</span></span> 
  
<span data-ttu-id="acb00-164">Это также запроса XML, управляемый API EWS отправляет при использовании **ResolveName** метод для [разрешения контакта](#bk_resolveewsma).</span><span class="sxs-lookup"><span data-stu-id="acb00-164">This is also the XML request that the EWS Managed API sends when you use the **ResolveName** method to [resolve a contact](#bk_resolveewsma).</span></span>
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ResolveNames ReturnFullContactData="true"
                    SearchScope="Contacts">
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
      <m:UnresolvedEntry>johnson</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="acb00-165">Сервер отвечает на запрос **ResolveNames** [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что операция успешно завершена и найти только один результат, или **ErrorNameResolutionMultipleResults** Если найдено несколько результатов - являющийся, отображаемые в третьем примере кода на основании контакт, [Создание контактов роли представителя с помощью управляемого интерфейса API веб-служб Exchange](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="acb00-165">The server responds to the **ResolveNames** request with a [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the operation completed successfully and found only one result, or **ErrorNameResolutionMultipleResults** if multiple results were found - which is what's shown in third code example based on the contact [Create a contact as a delegate by using the EWS Managed API](#bk_createewsma).</span></span> <span data-ttu-id="acb00-166">Ответ также содержит [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) каждого результата.</span><span class="sxs-lookup"><span data-stu-id="acb00-166">The response also contains the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of each result.</span></span> 
  
<span data-ttu-id="acb00-167">Значение элемента **ItemId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="acb00-167">The value of the **ItemId** element has been shortened for readability.</span></span> 
  
```XML
 <?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Warning">
          <m:MessageText>Multiple results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionMultipleResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:ResolutionSet TotalItemsInView="2"
                           IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_1@contoso.com</t:Name>
                <t:EmailAddress>brian_1@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_2@contoso.com</t:Name>
                <t:EmailAddress>brian_2@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="acb00-168">Теперь, когда у вас есть **идентификатор элемента** для контактов, которые соответствуют неоднозначное имя, можно [получить, обновить и удаление элементов контактов в качестве делегата с помощью веб-служб Exchange](#bk_getews) с помощью **ItemId** и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;и необходимо указать SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-168">Now that you have the **ItemId** for the contacts that match the ambiguous name, you can [Get, update, or delete contact items as a delegate by using EWS](#bk_getews) by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="acb00-169"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="acb00-169"></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="acb00-170">Получение, обновление и удаление элементов контактов роли представителя с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-170">Get, update, or delete contact items as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="acb00-171">Можно использовать управляемый API EWS для получения, обновить или удалить контакт так же, как выполнять эти действия, если вы не используете делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="acb00-171">You can use the EWS Managed API to get, update, or delete a contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="acb00-172">Единственное отличие — объект службы для делегата.</span><span class="sxs-lookup"><span data-stu-id="acb00-172">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="acb00-173">Идентификатор элемента, включенные в вызове метода **Привязка** уникальным образом определяет элемент в хранилище почтовых ящиков в папке контактов владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-173">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="acb00-174">**В таблице 2. Управляемый API EWS методы работы с контактом роли представителя**</span><span class="sxs-lookup"><span data-stu-id="acb00-174">**Table 2. EWS Managed API methods working with a contact as a delegate**</span></span>

|<span data-ttu-id="acb00-175">**Задача**</span><span class="sxs-lookup"><span data-stu-id="acb00-175">**Task**</span></span>|<span data-ttu-id="acb00-176">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="acb00-176">**EWS Managed API method**</span></span>|<span data-ttu-id="acb00-177">**Пример кода**</span><span class="sxs-lookup"><span data-stu-id="acb00-177">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="acb00-178">Получение контакта.</span><span class="sxs-lookup"><span data-stu-id="acb00-178">Get a contact</span></span>  <br/> |[<span data-ttu-id="acb00-179">Привязка</span><span class="sxs-lookup"><span data-stu-id="acb00-179">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="acb00-180">Получение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="acb00-180">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="acb00-181">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="acb00-181">Update a contact</span></span>  <br/> |<span data-ttu-id="acb00-182">[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) следуют [обновления](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="acb00-182">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="acb00-183">Изменение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="acb00-183">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="acb00-184">Удалить контакт</span><span class="sxs-lookup"><span data-stu-id="acb00-184">Delete a contact</span></span>  <br/> |<span data-ttu-id="acb00-185">[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , а затем [Удалить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="acb00-185">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="acb00-186">Удаление элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="acb00-186">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<span data-ttu-id="acb00-187"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="acb00-187"></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="acb00-188">Получение, обновление и удаление элементов контактов роли представителя с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-188">Get, update, or delete contact items as a delegate by using EWS</span></span>

<span data-ttu-id="acb00-189">Чтобы получить, обновить или удалить контакт собранием или встречей так же, как выполнять эти действия, если вы не используете делегированный доступ, можно использовать веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="acb00-189">You can use EWS to get, update, or delete a meeting or appointment contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="acb00-190">Единственное отличие — объект службы для делегата.</span><span class="sxs-lookup"><span data-stu-id="acb00-190">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="acb00-191">Идентификатор элемента, включенных в запрос [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) уникальным образом определяет элемент в хранилище почтовых ящиков в папке контактов владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="acb00-191">The item ID included in the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) request uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="acb00-192">**В таблице 3. Операции EWS для работы с контактом роли представителя**</span><span class="sxs-lookup"><span data-stu-id="acb00-192">**Table 3. EWS operations for working with a contact as a delegate**</span></span>

|<span data-ttu-id="acb00-193">**Задача**</span><span class="sxs-lookup"><span data-stu-id="acb00-193">**Task**</span></span>|<span data-ttu-id="acb00-194">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="acb00-194">**EWS operation**</span></span>|<span data-ttu-id="acb00-195">**Пример**</span><span class="sxs-lookup"><span data-stu-id="acb00-195">**Sample**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="acb00-196">Получение контакта.</span><span class="sxs-lookup"><span data-stu-id="acb00-196">Get a contact</span></span>  <br/> |[<span data-ttu-id="acb00-197">GetItem</span><span class="sxs-lookup"><span data-stu-id="acb00-197">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="acb00-198">Получение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-198">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="acb00-199">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="acb00-199">Update a contact</span></span>  <br/> |<span data-ttu-id="acb00-200">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="acb00-200">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="acb00-201">Изменение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-201">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="acb00-202">Удалить контакт</span><span class="sxs-lookup"><span data-stu-id="acb00-202">Delete a contact</span></span>  <br/> |<span data-ttu-id="acb00-203">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="acb00-203">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[<span data-ttu-id="acb00-204">Удаление элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-204">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="acb00-205">См. также</span><span class="sxs-lookup"><span data-stu-id="acb00-205">See also</span></span>

- [<span data-ttu-id="acb00-206">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-206">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="acb00-207">Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-207">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="acb00-208">Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-208">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [<span data-ttu-id="acb00-209">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="acb00-209">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
- [<span data-ttu-id="acb00-210">Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="acb00-210">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

