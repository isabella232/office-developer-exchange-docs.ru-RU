---
title: Доступ к контактам как представителю с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Узнайте, как получить доступ к контактам как представителю с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 06faf7dd7459b14792abbea21761e909c8eb9fb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455347"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="75578-103">Доступ к контактам как представителю с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="75578-103">Access contacts as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="75578-104">Узнайте, как получить доступ к контактам как представителю с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="75578-104">Learn how to access contacts as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="75578-105">С помощью управляемого API EWS или EWS вы можете предоставить пользователю доступ к папке контактов владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-105">You can use the EWS Managed API or EWS to give a user access to a mailbox owner's Contacts folder.</span></span> <span data-ttu-id="75578-106">После этого делегат может создавать контакты от имени владельца почтового ящика, а также получать, обновлять и удалять контакты из папки "Контакты" владельца почтового ящика в зависимости от их разрешений.</span><span class="sxs-lookup"><span data-stu-id="75578-106">The delegate can then create contacts on behalf of the mailbox owner, and retrieve, update, and delete contacts from the mailbox owner's Contacts folder, depending on their permissions.</span></span>
  
<span data-ttu-id="75578-107">В качестве представителя вы можете использовать те же методы и операции для доступа к папке контактов владельца почтового ящика, которая используется для доступа к собственной папке контактов.</span><span class="sxs-lookup"><span data-stu-id="75578-107">As a delegate, you use the same methods and operations to access a mailbox owner's Contacts folder that you use to access your own Contacts folder.</span></span> <span data-ttu-id="75578-108">Основное отличие заключается в том, что для поиска или создания элемента контакта необходимо использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) , а затем после определения идентификатора элемента можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновления или удаления элемента.</span><span class="sxs-lookup"><span data-stu-id="75578-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a contact item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="75578-109">**Таблица 1. Методы управляемого API EWS и операции EWS для доступа к контакту в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="75578-109">**Table 1. EWS Managed API methods and EWS operations for accessing a contact as a delegate**</span></span>

|<span data-ttu-id="75578-110">**Задача**</span><span class="sxs-lookup"><span data-stu-id="75578-110">**If you want to…**</span></span>|<span data-ttu-id="75578-111">**Используйте этот метод управляемого API EWS...**</span><span class="sxs-lookup"><span data-stu-id="75578-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="75578-112">**Используйте эту операцию EWS...**</span><span class="sxs-lookup"><span data-stu-id="75578-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="75578-113">Создание контакта в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="75578-113">Create a contact as a delegate</span></span>  <br/> |<span data-ttu-id="75578-114">[Item. Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) , где параметр [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке контактов владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="75578-114">[Item.Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="75578-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="75578-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="75578-116">Создание нескольких контактов в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="75578-116">Create multiple contacts as a delegate</span></span>  <br/> |<span data-ttu-id="75578-117">[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке контактов владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="75578-117">[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="75578-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="75578-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="75578-119">Разрешение контакта в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="75578-119">Resolve a contact as a delegate</span></span>  <br/> |<span data-ttu-id="75578-120">[ExchangeService. ресолвенаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) , где параметр [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке контактов владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="75578-120">[ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="75578-121">[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) , где элемент [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="75578-121">[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="75578-122">Поиск и поиск контакта в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="75578-122">Search for or find a contact as a delegate</span></span>  <br/> |<span data-ttu-id="75578-123">[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке контактов владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="75578-123">[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="75578-124">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="75578-124">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="75578-125">Получение контакта в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="75578-125">Get a contact as a delegate</span></span>  <br/> |[<span data-ttu-id="75578-126">Contact. Bind</span><span class="sxs-lookup"><span data-stu-id="75578-126">Contact.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="75578-127">GetItem</span><span class="sxs-lookup"><span data-stu-id="75578-127">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="75578-128">Обновление контакта представителем</span><span class="sxs-lookup"><span data-stu-id="75578-128">Update a contact as a delegate</span></span>  <br/> |<span data-ttu-id="75578-129">[Contact. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) , за которым следует [Contact. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="75578-129">[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="75578-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="75578-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="75578-131">Удаление контакта в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="75578-131">Delete a contact as a delegate</span></span>  <br/> |<span data-ttu-id="75578-132">[Contact. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) , за которым следует [Contact. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="75578-132">[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="75578-133">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75578-133">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="75578-134">В примерах кода, приведенных в этой статье, primary@contoso.com является владельцем почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-134">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 

<span data-ttu-id="75578-135"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="75578-135"><a name="bk_prereq"> </a></span></span>

## <a name="prerequisite-tasks"></a><span data-ttu-id="75578-136">Предварительные задачи</span><span class="sxs-lookup"><span data-stu-id="75578-136">Prerequisite tasks</span></span>

<span data-ttu-id="75578-137">Прежде чем пользователь сможет получить доступ к папке контактов владельца почтового ящика в качестве представителя, пользователь должен быть [добавлен в качестве представителя с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для папки "Контакты" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-137">Before a user can access the mailbox owner's Contacts folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Contacts folder.</span></span> 

<span data-ttu-id="75578-138"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="75578-138"><a name="bk_createewsma"> </a></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="75578-139">Создание контакта в качестве делегата с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="75578-139">Create a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="75578-140">Управляемый API EWS позволяет использовать объект Service для делегированного пользователя, чтобы создавать контакты для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-140">The EWS Managed API enables you to use the service object for the delegate user to create contacts for the mailbox owner.</span></span> <span data-ttu-id="75578-141">В этом примере показано, как использовать метод [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) для создания собрания и отправки приглашений на собрание участникам.</span><span class="sxs-lookup"><span data-stu-id="75578-141">This example shows how to use the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="75578-142">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для делегата, а представителю предоставлены соответствующие разрешения для папки "Контакты" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-142">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="75578-143">Обратите внимание, что при сохранении элемента вызов метода [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) должен определить папку контактов владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-143">Note that when you save the item, the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="75578-144">Если папка "Контакты" владельца почтового ящика не указана, приглашение на собрание сохраняется в папке "Контакты" представителя, а не в папке "Контакты" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-144">If the mailbox owner's Contacts folder is not specified, the meeting request gets saved to the delegate's Contacts folder and not the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="75578-145">Вы можете включить папку контактов владельца почтового ящика в вызов метода **Save** двумя способами.</span><span class="sxs-lookup"><span data-stu-id="75578-145">You can include the mailbox owner's Contacts folder in the **Save** method call in two way.</span></span> <span data-ttu-id="75578-146">Мы рекомендуем создать экземпляр нового экземпляра объекта [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) с помощью [веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-146">We recommend that you instantiate a new instance of the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

<span data-ttu-id="75578-147">Однако сначала можно [выполнить привязывание](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) к папке Contacts, а затем использовать идентификатор папки в вызове метода **Save** .</span><span class="sxs-lookup"><span data-stu-id="75578-147">However, you can also [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Contacts folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="75578-148">Однако имейте в виду, что при этом создается дополнительный вызов EWS.</span><span class="sxs-lookup"><span data-stu-id="75578-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<span data-ttu-id="75578-149"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="75578-149"><a name="bk_createews"> </a></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="75578-150">Создание контакта в качестве представителя с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="75578-150">Create a contact as a delegate by using EWS</span></span>

<span data-ttu-id="75578-151">Служба EWS позволяет использовать объект Service для делегированного пользователя, чтобы создавать элементы контактов для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-151">EWS enables you to use the service object for the delegate user to create contact items for the mailbox owner.</span></span> <span data-ttu-id="75578-152">В этом примере показано, как использовать операцию [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания контакта.</span><span class="sxs-lookup"><span data-stu-id="75578-152">This example shows how to use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a contact.</span></span> 
  
<span data-ttu-id="75578-153">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **Save** для [создания контакта](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="75578-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a contact](#bk_createewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="75578-154">Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что контакт был создан успешно.</span><span class="sxs-lookup"><span data-stu-id="75578-154">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the contact was created successfully.</span></span> <span data-ttu-id="75578-155">Ответ также содержит идентификатор элемента нового контакта.</span><span class="sxs-lookup"><span data-stu-id="75578-155">The response also contains the item ID of the newly created contact.</span></span>

<span data-ttu-id="75578-156"><a name="bk_resolveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="75578-156"><a name="bk_resolveewsma"> </a></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="75578-157">Разрешение контакта в качестве делегата с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="75578-157">Resolve a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="75578-158">Чтобы найти контакт на основе потенциально неоднозначного имени или термина, необходимо использовать один из методов [ExchangeService. ресолвенаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) , включающий параметр [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , чтобы можно было указать папку контактов владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-158">To find a contact based on a possibly ambiguous name or term, you must use one of the [ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) methods that includes a [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="75578-159">После того как вызов метода **ResolveNames** возвращает ответ с идентификатором, вы можете [получить, обновить или удалить контакт](#bk_getewsma) с помощью идентификатора и [неявного доступа](delegate-access-and-ews-in-exchange.md#bk_implicit) &mdash; , а также не указывать SMTP-адрес владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-159">After the **ResolveNames** method call returns a response with an ID, you can [get, update or delete the contact](#bk_getewsma) using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="75578-160"><a name="bk_resolveews"> </a></span><span class="sxs-lookup"><span data-stu-id="75578-160"><a name="bk_resolveews"> </a></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="75578-161">Разрешение контакта в качестве делегата с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="75578-161">Resolve a contact as a delegate by using EWS</span></span>

<span data-ttu-id="75578-162">Служба EWS позволяет использовать объект Service для делегированного пользователя для разрешения частичных имен в папке "Контакты" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-162">EWS enables you to use the service object for the delegate user to resolve partial names in the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="75578-163">В этом примере показано, как использовать операцию [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) для поиска собраний в папке "Контакты" владельца почтового ящика, содержащей слово "Johnson".</span><span class="sxs-lookup"><span data-stu-id="75578-163">This example shows how to use the [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Contacts folder that contain the word "johnson".</span></span> 
  
<span data-ttu-id="75578-164">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **ресолвенаме** для [разрешения контакта](#bk_resolveewsma).</span><span class="sxs-lookup"><span data-stu-id="75578-164">This is also the XML request that the EWS Managed API sends when you use the **ResolveName** method to [resolve a contact](#bk_resolveewsma).</span></span>
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="75578-165">Сервер отвечает на запрос **ResolveNames** с сообщением [ресолвенамесреспонсе](https://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает на то, что операция выполнена успешно и обнаружила только один результат, или **еррорнамересолутионмултиплересултс** , если найдено несколько результатов (то есть в третьем примере кода, основанном на контакте [Создание контакта в качестве делегата с помощью управляемого API EWS](#bk_createewsma)).</span><span class="sxs-lookup"><span data-stu-id="75578-165">The server responds to the **ResolveNames** request with a [ResolveNamesResponse](https://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the operation completed successfully and found only one result, or **ErrorNameResolutionMultipleResults** if multiple results were found - which is what's shown in third code example based on the contact [Create a contact as a delegate by using the EWS Managed API](#bk_createewsma).</span></span> <span data-ttu-id="75578-166">Ответ также содержит идентификатор [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) каждого результата.</span><span class="sxs-lookup"><span data-stu-id="75578-166">The response also contains the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of each result.</span></span> 
  
<span data-ttu-id="75578-167">Значение элемента **ItemId** было сокращено для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="75578-167">The value of the **ItemId** element has been shortened for readability.</span></span> 
  
```XML
 <?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="75578-168">Теперь, когда у вас есть идентификатор **ItemId** для контактов, которые совпадают с неоднозначным именем, вы можете [получать, обновлять и удалять элементы контакта в качестве делегата с помощью EWS](#bk_getews) , используя идентификатор **ItemId** и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) &mdash; , и вам не нужно указывать SMTP-адрес владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-168">Now that you have the **ItemId** for the contacts that match the ambiguous name, you can [Get, update, or delete contact items as a delegate by using EWS](#bk_getews) by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="75578-169"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="75578-169"><a name="bk_getewsma"> </a></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="75578-170">Получение, обновление и удаление элементов контактов в качестве делегата с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="75578-170">Get, update, or delete contact items as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="75578-171">Вы можете использовать управляемый API EWS для получения, обновления или удаления контакта аналогично выполнению этих действий, если вы не используете делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="75578-171">You can use the EWS Managed API to get, update, or delete a contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="75578-172">Единственное отличие заключается в том, что объект службы предназначен для делегированного пользователя.</span><span class="sxs-lookup"><span data-stu-id="75578-172">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="75578-173">Идентификатор элемента, включенный в вызов метода **BIND** , уникальным образом определяет элемент в хранилище почтовых ящиков в папке "Контакты" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-173">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="75578-174">**Таблица 2. Методы управляемого API EWS, работающие с контактом в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="75578-174">**Table 2. EWS Managed API methods working with a contact as a delegate**</span></span>

|<span data-ttu-id="75578-175">**Задача**</span><span class="sxs-lookup"><span data-stu-id="75578-175">**Task**</span></span>|<span data-ttu-id="75578-176">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="75578-176">**EWS Managed API method**</span></span>|<span data-ttu-id="75578-177">**Пример кода**</span><span class="sxs-lookup"><span data-stu-id="75578-177">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="75578-178">Получение контакта.</span><span class="sxs-lookup"><span data-stu-id="75578-178">Get a contact</span></span>  <br/> |[<span data-ttu-id="75578-179">Базу</span><span class="sxs-lookup"><span data-stu-id="75578-179">Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="75578-180">Получение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="75578-180">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="75578-181">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="75578-181">Update a contact</span></span>  <br/> |<span data-ttu-id="75578-182">[Привязка](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которой следует [Обновление](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="75578-182">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="75578-183">Изменение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="75578-183">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="75578-184">Удалить контакт</span><span class="sxs-lookup"><span data-stu-id="75578-184">Delete a contact</span></span>  <br/> |<span data-ttu-id="75578-185">[Привязка](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которой следует [Удаление](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="75578-185">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="75578-186">Удаление элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="75578-186">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<span data-ttu-id="75578-187"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="75578-187"><a name="bk_getews"> </a></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="75578-188">Получение, обновление и удаление элементов контактов в качестве делегата с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="75578-188">Get, update, or delete contact items as a delegate by using EWS</span></span>

<span data-ttu-id="75578-189">С помощью EWS вы можете получать, обновлять и удалять контакты собрания или встречи так же, как и при использовании делегированного доступа.</span><span class="sxs-lookup"><span data-stu-id="75578-189">You can use EWS to get, update, or delete a meeting or appointment contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="75578-190">Единственное отличие заключается в том, что объект службы предназначен для делегированного пользователя.</span><span class="sxs-lookup"><span data-stu-id="75578-190">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="75578-191">Идентификатор элемента, включенный в запрос [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , однозначно определяет элемент в хранилище почтовых ящиков в папке "Контакты" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="75578-191">The item ID included in the [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) request uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="75578-192">**Таблица 3. Операции EWS для работы с контактом в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="75578-192">**Table 3. EWS operations for working with a contact as a delegate**</span></span>

|<span data-ttu-id="75578-193">**Task**</span><span class="sxs-lookup"><span data-stu-id="75578-193">**Task**</span></span>|<span data-ttu-id="75578-194">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="75578-194">**EWS operation**</span></span>|<span data-ttu-id="75578-195">**Пример**</span><span class="sxs-lookup"><span data-stu-id="75578-195">**Sample**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="75578-196">Получение контакта.</span><span class="sxs-lookup"><span data-stu-id="75578-196">Get a contact</span></span>  <br/> |[<span data-ttu-id="75578-197">GetItem</span><span class="sxs-lookup"><span data-stu-id="75578-197">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="75578-198">Получение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="75578-198">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="75578-199">Обновление контакта</span><span class="sxs-lookup"><span data-stu-id="75578-199">Update a contact</span></span>  <br/> |<span data-ttu-id="75578-200">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="75578-200">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="75578-201">Изменение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="75578-201">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="75578-202">Удалить контакт</span><span class="sxs-lookup"><span data-stu-id="75578-202">Delete a contact</span></span>  <br/> |<span data-ttu-id="75578-203">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="75578-203">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[<span data-ttu-id="75578-204">Удаление элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="75578-204">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75578-205">См. также</span><span class="sxs-lookup"><span data-stu-id="75578-205">See also</span></span>

- [<span data-ttu-id="75578-206">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="75578-206">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="75578-207">Добавление и удаление делегатов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="75578-207">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="75578-208">Задание разрешений для папки другого пользователя с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="75578-208">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [<span data-ttu-id="75578-209">Пользователи и контакты в EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="75578-209">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
- [<span data-ttu-id="75578-210">Устранение неоднозначности имен с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75578-210">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

