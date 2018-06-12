---
title: Работа с элементами почтового ящика Exchange с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Узнайте, как создавать, получать, редактировать и удалять элементы с помощью управляемого API EWS или служб EWS в Exchange.
ms.openlocfilehash: e70ac499da57faa60b4bcb6082648b23d1a7e791
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761140"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a><span data-ttu-id="23ed1-103">Работа с элементами почтового ящика Exchange с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="23ed1-103">Work with Exchange mailbox items by using EWS in Exchange</span></span>

<span data-ttu-id="23ed1-104">Узнайте, как создавать, получать, редактировать и удалять элементы с помощью управляемого API EWS или служб EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="23ed1-104">Learn how to create, get, update, and delete items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="23ed1-105">Для работы с элементами в почтовом ящике, можно использовать управляемый API EWS или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="23ed1-105">You can use the EWS Managed API or EWS to work with items in a mailbox.</span></span> <span data-ttu-id="23ed1-106">Можно использовать универсальный элементов — управляемый API EWS [элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) объектов или типов веб-служб Exchange [элемента](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) — для выполнения некоторых операций (начало элемента или удаление элемента с помощью идентификатора элемента); Тем не менее в большинстве случаев, необходимо будет использовать [строго типизированных элемента](folders-and-items-in-ews-in-exchange.md#bk_item) для get и операцию обновления, поскольку он потребуется доступ к свойствам, которые относятся к строго типизированный элемент.</span><span class="sxs-lookup"><span data-stu-id="23ed1-106">You can use generic items — EWS Managed API [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) objects or EWS [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) types — to perform some operations (getting an item or deleting an item by using the item's identifier); however, most of the time you'll have to use a [strongly typed item](folders-and-items-in-ews-in-exchange.md#bk_item) to perform a get or update operation because you'll need access to the properties that are specific to the strongly typed item.</span></span> 

<span data-ttu-id="23ed1-107">Например универсальный элемент нельзя использовать для получения элемента, который содержит начать и Дата окончания — нужно объект управляемый API EWS [встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) тип для этого.</span><span class="sxs-lookup"><span data-stu-id="23ed1-107">For example, you can't use a generic item to retrieve an item that contains a start and end date - you need an EWS Managed API [Appointment](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object or an EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) type to do that.</span></span> <span data-ttu-id="23ed1-108">И, если вы используете управляемый API веб-служб Exchange, всегда необходимо создать строго типизированные элементы, поскольку универсальный класс **элемента** не имеет конструктора.</span><span class="sxs-lookup"><span data-stu-id="23ed1-108">And if you're using the EWS Managed API, you always have to create strongly typed items, because the generic **Item** class does not have a constructor.</span></span> <span data-ttu-id="23ed1-109">При работе с элементом, который не является строго типизированным, всегда можно использовать базовый класс **элемента** для работы с элементом.</span><span class="sxs-lookup"><span data-stu-id="23ed1-109">If you're working with an item that is not strongly typed, you can always use the base **Item** class to work with the item.</span></span> 
  
<span data-ttu-id="23ed1-110">**В таблице 1. Управляемый API EWS методы и операций веб-служб Exchange для работы с элементами**</span><span class="sxs-lookup"><span data-stu-id="23ed1-110">**Table 1. EWS Managed API methods and EWS operations for working with items**</span></span>

|<span data-ttu-id="23ed1-111">**Чтобы...**</span><span class="sxs-lookup"><span data-stu-id="23ed1-111">**In order to…**</span></span>|<span data-ttu-id="23ed1-112">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="23ed1-112">**EWS Managed API method**</span></span>|<span data-ttu-id="23ed1-113">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="23ed1-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="23ed1-114">Создание универсального элемента</span><span class="sxs-lookup"><span data-stu-id="23ed1-114">Create a generic item</span></span>  <br/> |<span data-ttu-id="23ed1-p103">Нет. С помощью управляемого API EWS можно создавать только элементы определенных типов. Создавать универсальные элементы невозможно.</span><span class="sxs-lookup"><span data-stu-id="23ed1-p103">None. You can only create specific item types by using the EWS Managed API; you cannot create generic items.</span></span>  <br/> |[<span data-ttu-id="23ed1-117">CreateItem</span><span class="sxs-lookup"><span data-stu-id="23ed1-117">CreateItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="23ed1-118">Получение элемента</span><span class="sxs-lookup"><span data-stu-id="23ed1-118">Get an item</span></span>  <br/> |[<span data-ttu-id="23ed1-119">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="23ed1-119">Item.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="23ed1-120">GetItem</span><span class="sxs-lookup"><span data-stu-id="23ed1-120">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="23ed1-121">Изменение элемента</span><span class="sxs-lookup"><span data-stu-id="23ed1-121">Update an item</span></span>  <br/> |[<span data-ttu-id="23ed1-122">Item.Update</span><span class="sxs-lookup"><span data-stu-id="23ed1-122">Item.Update</span></span>](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="23ed1-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="23ed1-123">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="23ed1-124">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="23ed1-124">Delete an item</span></span>  <br/> |[<span data-ttu-id="23ed1-125">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="23ed1-125">Item.Delete</span></span>](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="23ed1-126">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="23ed1-126">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="23ed1-127">В этой статье вы узнаете, при использовании универсального базового класса и когда следует использовать строго типизированный элемент выполнение задачи.</span><span class="sxs-lookup"><span data-stu-id="23ed1-127">In this article, you'll learn when you can use the generic base class and when you need to use a strongly typed item to complete your task.</span></span> <span data-ttu-id="23ed1-128">В примере кода показано использование базового класса и что делать при базового класса или он не соответствии со своими потребностями.</span><span class="sxs-lookup"><span data-stu-id="23ed1-128">The code examples will show you how to use the base class, and what to do when you can't use the base class or it doesn't fit your needs.</span></span>
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="23ed1-129">Создание элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="23ed1-129">Create an item by using the EWS Managed API</span></span>
<span data-ttu-id="23ed1-130"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-130"></span></span>

<span data-ttu-id="23ed1-131">Управляемый API EWS не имеет общедоступным конструктора для класса [элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , необходимо использовать конструктор для типа определенного элемента, который требуется создать, чтобы создать элемент.</span><span class="sxs-lookup"><span data-stu-id="23ed1-131">The EWS Managed API does not have a publicly available constructor for the [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) class, so you must use the constructor for the specific item type you want to create in order to create an item.</span></span> <span data-ttu-id="23ed1-132">Например используйте [конструктор класса EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) для создания нового сообщения электронной почты и [контактов конструктор класса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) для создания нового контакта.</span><span class="sxs-lookup"><span data-stu-id="23ed1-132">For example, use the [EmailMessage class constructor](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) to create a new email message, and the [Contact class constructor](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) to create a new contact.</span></span> <span data-ttu-id="23ed1-133">Аналогичным образом сервер никогда не возвращает универсальный объекты **элементов** в ответы; все элементы универсальный возвращаются в виде объектов **EmailMessage** .</span><span class="sxs-lookup"><span data-stu-id="23ed1-133">Likewise, the server never returns generic **Item** objects in responses; all generic items are returned as **EmailMessage** objects.</span></span> 
  
<span data-ttu-id="23ed1-p106">Если вы знаете тип создаваемого элемента, выполнить задачу можно всего за несколько этапов. Действия одинаковы для всех типов элементов:</span><span class="sxs-lookup"><span data-stu-id="23ed1-p106">When you know the type of item to create, you can complete the task in just a few steps. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="23ed1-136">Инициализация нового экземпляра одного из классов [элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) с помощью объекта [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) как параметр.</span><span class="sxs-lookup"><span data-stu-id="23ed1-136">Initialize a new instance of one of the [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) classes with the [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object as a parameter.</span></span> 
    
2. <span data-ttu-id="23ed1-p107">Задайте свойства элемента. Для всех типов элементов используются разные схемы, поэтому для разных элементов доступны разные свойства.</span><span class="sxs-lookup"><span data-stu-id="23ed1-p107">Set properties on the item. The schemas are different for each item type, so different properties are available for different items.</span></span>
    
3. <span data-ttu-id="23ed1-139">Сохраните элемент или сохраните и отправьте его.</span><span class="sxs-lookup"><span data-stu-id="23ed1-139">Save the item, or save and send the item.</span></span>
    
<span data-ttu-id="23ed1-140">К примеру можно создать объект [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) , Настройка параметров [Тема](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [текст](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)и [ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) и отправить его с помощью метода [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="23ed1-140">For example, you can create an [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object, set the [Subject](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx), and [ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) properties, and then send it by using the [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
```

<span data-ttu-id="23ed1-141">Чтобы научиться создавать собрания или встречи с помощью управляемого интерфейса API веб-служб Exchange, обратитесь к разделу [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-141">To learn how to create a meeting or appointment item by using the EWS Managed API, see [Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span>
  
## <a name="create-an-item-by-using-ews"></a><span data-ttu-id="23ed1-142">Создание элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="23ed1-142">Create an item by using EWS</span></span>
<span data-ttu-id="23ed1-143"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-143"></span></span>

<span data-ttu-id="23ed1-p108">С помощью веб-служб Exchange можно создать универсальный или строго типизированный элемент. Действия одинаковы для всех типов элементов:</span><span class="sxs-lookup"><span data-stu-id="23ed1-p108">You can create a generic item or a strongly typed item by using EWS. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="23ed1-146">С помощью операции [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) для создания элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="23ed1-146">Use the [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to create an item in the Exchange store.</span></span> 
    
2. <span data-ttu-id="23ed1-147">Используйте элемент [элементов](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) содержит один или несколько элементов для создания.</span><span class="sxs-lookup"><span data-stu-id="23ed1-147">Use the [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) element to contain one or more items to create.</span></span> 
    
3. <span data-ttu-id="23ed1-148">Задайте свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="23ed1-148">Set properties on the item.</span></span>
    
<span data-ttu-id="23ed1-149">Например можно создавать сообщения электронной почты и отправьте его с помощью кода в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="23ed1-149">For example, you can create an email message and send it by using the code in the following example.</span></span> <span data-ttu-id="23ed1-150">Это также запроса XML, то при вызове метода [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) отправляет управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="23ed1-150">This is also the XML request that the EWS Managed API sends when you call the [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="23ed1-151">Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что сообщение электронной почты был успешно создан, и [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) из вновь сообщение о создании.</span><span class="sxs-lookup"><span data-stu-id="23ed1-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="23ed1-152">Чтобы научиться создавать собрания или встречи с помощью веб-служб Exchange, обратитесь к разделу [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-152">To learn how to create a meeting or appointment item by using EWS, see [Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span></span>
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="23ed1-153">Получение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="23ed1-153">Get an item by using the EWS Managed API</span></span>
<span data-ttu-id="23ed1-154"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-154"></span></span>

<span data-ttu-id="23ed1-155">Чтобы использовать управляемый API EWS для получения элемента, если вы знаете [элемент.идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для извлечения, можно просто вызвать один из методов [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для элемента, а элемент извлекается.</span><span class="sxs-lookup"><span data-stu-id="23ed1-155">To use the EWS Managed API to get an item if you know the [Item.Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to retrieve, you simply call one of the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) methods on the item, and the item is retrieved.</span></span> <span data-ttu-id="23ed1-156">Рекомендуется рекомендуется ограничить возвращаемые только теми надстройками, которые необходимы свойства.</span><span class="sxs-lookup"><span data-stu-id="23ed1-156">As a best practice, we recommend that you limit the properties returned to only those that are required.</span></span> <span data-ttu-id="23ed1-157">В этом примере возвращаются свойства **Id** элемента и свойство **Subject** .</span><span class="sxs-lookup"><span data-stu-id="23ed1-157">This example returns the item **Id** property and the **Subject** property.</span></span> 
  
<span data-ttu-id="23ed1-158">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="23ed1-158">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="23ed1-159">Локальной переменной *itemId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для обновления.</span><span class="sxs-lookup"><span data-stu-id="23ed1-159">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

<span data-ttu-id="23ed1-160">Если вы ищете элемента, который соответствует определенному набору условий, выполните следующее:</span><span class="sxs-lookup"><span data-stu-id="23ed1-160">If you're searching for an item that meets specific criteria, do the following:</span></span>
  
1. <span data-ttu-id="23ed1-161">Выполните привязку к папке, содержащей получаемые элементы.</span><span class="sxs-lookup"><span data-stu-id="23ed1-161">Bind to the folder that contains the items to get.</span></span>
    
2. <span data-ttu-id="23ed1-162">Создайте экземпляр [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) или [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) для фильтрации элементов для возврата.</span><span class="sxs-lookup"><span data-stu-id="23ed1-162">Instantiate a [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) or a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to filter the items to return.</span></span> 
    
3. <span data-ttu-id="23ed1-163">Создайте экземпляр объекта [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) или [представления календаря](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) для определения количества элементов для возврата.</span><span class="sxs-lookup"><span data-stu-id="23ed1-163">Instantiate an [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object to specify the number of items to return.</span></span> 
    
4. <span data-ttu-id="23ed1-164">Вызовите метод [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="23ed1-164">Call the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="23ed1-165">Например если вы хотите получать сообщения непрочитанные сообщения электронной почты в папке "Входящие", используйте код в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="23ed1-165">For example, if you want to retrieve unread email messages in the Inbox, use the code in the following example.</span></span> <span data-ttu-id="23ed1-166">В этом примере использует **SearchFilterCollection** для ограничения результатов метод **FindItems** , непрочитанных сообщений и ограничения для **ItemView** , чтобы ограничить результаты одного элемента.</span><span class="sxs-lookup"><span data-stu-id="23ed1-166">This example uses a **SearchFilterCollection** to limit the results of the **FindItems** method to unread messages, and limits the **ItemView** to limit results to one item.</span></span> <span data-ttu-id="23ed1-167">Этот код конкретного работает только с [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) объекты [EmailMessageSchema.IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) значение является частью **SearchFilter**.</span><span class="sxs-lookup"><span data-stu-id="23ed1-167">This particular code only works on [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects because the [EmailMessageSchema.IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) value is part of the **SearchFilter**.</span></span> 
  
```cs
// Bind the Inbox folder to the service object.
Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
// The search filter to get unread email.
SearchFilter sf = new SearchFilter.SearchFilterCollection(LogicalOperator.And, new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false));
ItemView view = new ItemView(1);
// Fire the query for the unread items.
// This method call results in a FindItem call to EWS.
FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Inbox, sf, view);
```

<span data-ttu-id="23ed1-168">Кроме того можно использовать [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) , чтобы ограничить результаты поиска, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="23ed1-168">Alternatively, you can use a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) to limit the results of the search as shown in the following code example.</span></span> <span data-ttu-id="23ed1-169">В этом примере используется метод [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) для получения до пяти встреч, которые происходят в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="23ed1-169">This example uses the [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve up to five appointments that occur in the next 30 days.</span></span> <span data-ttu-id="23ed1-170">Этот код безусловно работает только с элементами календаря.</span><span class="sxs-lookup"><span data-stu-id="23ed1-170">This code of course only works on calendar items.</span></span> 
  
```cs
// Initialize values for the start and end times, and the number of appointments to retrieve.
DateTime startDate = DateTime.Now;
DateTime endDate = startDate.AddDays(30);
const int NUM_APPTS = 5;
// Bind the Calendar folder to the service object.
// This method call results in a GetFolder call to EWS.
CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
// Set the start and end time and number of appointments to retrieve.
CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
// Limit the properties returned to the appointment's subject, start time, and end time.
cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
// Retrieve a collection of appointments by using the calendar view.
// This method call results in a FindAppointments call to EWS.
FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
```

<span data-ttu-id="23ed1-171">Обратите внимание, что в ответ **привязать** метод возвращает сведения о сервере, отличается от сведений, сервер возвращает метод отклика **FindItem** или **FindAppointment** .</span><span class="sxs-lookup"><span data-stu-id="23ed1-171">Note that the information the server returns in the **Bind** method response is different than the information that the server returns for a **FindItem** or **FindAppointment** method response.</span></span> <span data-ttu-id="23ed1-172">Метод **Bind** можно вернуть Схематизированный свойства, тогда как методы **FindItem** и **FindAppointment** не возвращают Схематизированный свойства.</span><span class="sxs-lookup"><span data-stu-id="23ed1-172">The **Bind** method can return all the schematized properties, whereas the **FindItem** and **FindAppointment** methods do not return all the schematized properties.</span></span> <span data-ttu-id="23ed1-173">Поэтому если вам требуется полный доступ к элементу, вам придется использовать метод **привязки** .</span><span class="sxs-lookup"><span data-stu-id="23ed1-173">So if you need full access to the item, you'll have to use the **Bind** method.</span></span> <span data-ttu-id="23ed1-174">Если у элемента нет **идентификатор** элемента, вы хотите получать, использовать методы **FindItem** или **FindAppointment** для получения идентификатора и затем использовать метод **привязки** для извлечения свойств, необходимую.</span><span class="sxs-lookup"><span data-stu-id="23ed1-174">If you don't have the item **Id** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** methods to retrieve the Id, and then use the **Bind** method to retrieve the properties you need.</span></span> 
  
<span data-ttu-id="23ed1-175">Чтобы узнать, как получить собрания или встречи с помощью управляемого интерфейса API веб-служб Exchange, обратитесь к разделу [получить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-175">To learn how to get a meeting or appointment item by using the EWS Managed API, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="get-an-item-by-using-ews"></a><span data-ttu-id="23ed1-176">Получение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="23ed1-176">Get an item by using EWS</span></span>
<span data-ttu-id="23ed1-177"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-177"></span></span>

<span data-ttu-id="23ed1-178">Если вы знаете [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) элемента для извлечения, вы получаете элемента с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="23ed1-178">If you know the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the item to retrieve, you can get the item by using the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation.</span></span> 
  
<span data-ttu-id="23ed1-179">В следующем примере показано XML-запрос, чтобы получить [тему](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) элемента с определенным **ItemId**.</span><span class="sxs-lookup"><span data-stu-id="23ed1-179">The following example shows the XML request to get the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of an item with a specific **ItemId**.</span></span> <span data-ttu-id="23ed1-180">Это также запроса XML, управляемый API EWS отправляет при вызове метода [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) на **идентификатор элемента**.</span><span class="sxs-lookup"><span data-stu-id="23ed1-180">This is also the XML request that the EWS Managed API sends when calling the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method on an **ItemId**.</span></span> <span data-ttu-id="23ed1-181">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="23ed1-181">The values of some attributes and elements have been shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="GJc/NAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показано XML-ответ, что сервер возвращает после обработки операции **GetItem** . Ответ указывает, что элемент был успешно извлечен. <span data-ttu-id="23ed1-184">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="23ed1-184">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="GJc/NAAA=" ChangeKey="CQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAGJd9Z"/>
              <t:Subject>Company Soccer Team</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="23ed1-185">Если вы не знаете **ItemId** элемента, которую необходимо получить, можно с помощью операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) поиск элемента.</span><span class="sxs-lookup"><span data-stu-id="23ed1-185">If you do not know the **ItemId** of the item you want to retrieve, you can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find the item.</span></span> <span data-ttu-id="23ed1-186">Чтобы использовать операции **FindItem** , необходимо сначала определить к папке, где выполняется поиск.</span><span class="sxs-lookup"><span data-stu-id="23ed1-186">In order to use the **FindItem** operation, you must first identify the folder that you're searching.</span></span> <span data-ttu-id="23ed1-187">Можно определить папку с помощью его **DistinguinguishedFolderName** или с помощью [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="23ed1-187">You can identify the folder by using its **DistinguinguishedFolderName** or by using the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span></span> <span data-ttu-id="23ed1-188">Параметр [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) или [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) операции можно использовать для получения **FolderId** необходимые.</span><span class="sxs-lookup"><span data-stu-id="23ed1-188">You can use either the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) or [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operations to get the **FolderId** you need.</span></span> <span data-ttu-id="23ed1-189">Затем с помощью операции **FindItem** для поиска этой папки для результатов, которые соответствуют фильтру поиска.</span><span class="sxs-lookup"><span data-stu-id="23ed1-189">Then use the **FindItem** operation to search that folder for results that match the search filter.</span></span> <span data-ttu-id="23ed1-190">В отличие от управляемый API веб-служб Exchange веб-служб Exchange не поддерживает операцию отдельные поиска для встреч.</span><span class="sxs-lookup"><span data-stu-id="23ed1-190">Unlike the EWS Managed API, EWS does not provide a separate find operation for appointments.</span></span> <span data-ttu-id="23ed1-191">Операция **FindItem** извлекает элементы всех типов.</span><span class="sxs-lookup"><span data-stu-id="23ed1-191">The **FindItem** operation retrieves items of all types.</span></span> 
  
<span data-ttu-id="23ed1-192">В следующем примере показано XML **FindItem** операция запроса, который отправляется на сервер для поиска встреч в папке календаря, найденных в течение 30 дней.</span><span class="sxs-lookup"><span data-stu-id="23ed1-192">The following example shows the XML **FindItem** operation request that is sent to the server to find appointments in the Calendar folder that occur in the next 30 days.</span></span> <span data-ttu-id="23ed1-193">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="23ed1-193">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-10-16T17:04:28.722Z" EndDate="2013-11-15T18:04:28.722Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAAEOAAA=" ChangeKey="AgAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAAAA3" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="23ed1-194">Сервер отвечает на запрос **FindItem** [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что операция выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="23ed1-194">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the operation completed successfully.</span></span> <span data-ttu-id="23ed1-195">Если все элементы календаря не отвечает условий фильтрации, их необходимо включить в ответе.</span><span class="sxs-lookup"><span data-stu-id="23ed1-195">If any calendar items meet the filtering criteria, they are included in the response.</span></span>
  
<span data-ttu-id="23ed1-196">Обратите внимание, что возвращает сведения о сервере в ответ операции **GetItem** , отличается от сведения, которые сервер возвращает **FindItem** или **FindAppointment** операция ответа.</span><span class="sxs-lookup"><span data-stu-id="23ed1-196">Note that the information the server returns in the **GetItem** operation response is different than the information the server returns in a **FindItem** or **FindAppointment** operation response.</span></span> <span data-ttu-id="23ed1-197">Операции **GetItem** может вернуть Схематизированный свойства, тогда как операций **FindItem** и **FindAppointment** не возвращает все Схематизированный свойства.</span><span class="sxs-lookup"><span data-stu-id="23ed1-197">The **GetItem** operation can return all the schematized properties, whereas the **FindItem** and **FindAppointment** operations do not return all the schematized properties.</span></span> <span data-ttu-id="23ed1-198">Поэтому если вам требуется полный доступ к элементу, необходимо хранить с помощью операции **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="23ed1-198">So if you need full access to the item, you'll have to use the **GetItem** operation.</span></span> <span data-ttu-id="23ed1-199">Если у вас нет **ItemId** элемента требуется получать, операции **FindItem** или **FindAppointment** использовать для получения **ItemId**и затем с помощью операции **GetItem** элементы, которые необходимо получить.</span><span class="sxs-lookup"><span data-stu-id="23ed1-199">If you don't have the **ItemId** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** operations to retrieve the **ItemId**, and then use the **GetItem** operation to retrieve the elements you need.</span></span> 
  
<span data-ttu-id="23ed1-200">Чтобы узнать, как получить собрания или встречи с помощью веб-служб Exchange, обратитесь к разделу [получить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-200">To learn how to get a meeting or appointment item by using EWS, see [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="23ed1-201">Изменение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="23ed1-201">Update an item by using the EWS Managed API</span></span>
<span data-ttu-id="23ed1-202"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-202"></span></span>

<span data-ttu-id="23ed1-203">Действия для обновления элемента с помощью управляемого интерфейса API EWS аналогичны и для всех типов элементов; Тем не менее свойства элемента различны для каждого типа элемента и метод [Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) имеет много перегруженных методов, из которых можно выбрать.</span><span class="sxs-lookup"><span data-stu-id="23ed1-203">The steps to update an item by using the EWS Managed API are similar for all item types; however, the item properties are different for each item type, and the [Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) method has many overloaded methods to choose from.</span></span> <span data-ttu-id="23ed1-204">Чтобы обновить элемент:</span><span class="sxs-lookup"><span data-stu-id="23ed1-204">To update an item:</span></span> 
  
1. <span data-ttu-id="23ed1-205">Метод [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для получения последней версии элемента, если у вас уже есть его.</span><span class="sxs-lookup"><span data-stu-id="23ed1-205">Use the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get the latest version of the item, unless you already have it.</span></span> <span data-ttu-id="23ed1-206">Для обновления свойств, относящихся к элементу строго типизированные, необходимо хранить связана с этим типом элемента.</span><span class="sxs-lookup"><span data-stu-id="23ed1-206">To update properties specific to a strongly typed item, you'll have to bind to that item type.</span></span> <span data-ttu-id="23ed1-207">Обновляет свойства, доступные на тип универсального элемента, можно привязать к объекту [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="23ed1-207">To update properties available on the generic item type, you can bind to the [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object.</span></span> 
    
2. <span data-ttu-id="23ed1-208">Измените свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="23ed1-208">Update the properties on the item.</span></span>
    
3. <span data-ttu-id="23ed1-209">Вызовите метод **Update** .</span><span class="sxs-lookup"><span data-stu-id="23ed1-209">Call the **Update** method.</span></span> 
    
<span data-ttu-id="23ed1-210">Например, вы можете изменить тему сообщения с помощью универсального типа элемента, как показано в коде приведенного ниже примера.</span><span class="sxs-lookup"><span data-stu-id="23ed1-210">For example, you can update the subject of an email by using the generic item type, as shown in the code in the following example.</span></span>
  
<span data-ttu-id="23ed1-211">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="23ed1-211">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="23ed1-212">Локальной переменной *itemId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для обновления.</span><span class="sxs-lookup"><span data-stu-id="23ed1-212">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Update the Subject of the email.
item.Subject = "New subject";
// Save the updated email.
// This method call results in an UpdateItem call to EWS.
item.Update(ConflictResolutionMode.AlwaysOverwrite);
```

<span data-ttu-id="23ed1-213">Чтобы узнать, как обновить собрания или встречи с помощью управляемого интерфейса API веб-служб Exchange, обратитесь к разделу [Обновить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-213">To learn how to update a meeting or appointment item by using the EWS Managed API, see [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="update-an-item-by-using-ews"></a><span data-ttu-id="23ed1-214">Изменение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="23ed1-214">Update an item by using EWS</span></span>
<span data-ttu-id="23ed1-215"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-215"></span></span>

<span data-ttu-id="23ed1-216">Чтобы изменить элемент с помощью веб-служб Exchange, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="23ed1-216">To update an item by using EWS, do the following:</span></span>
  
1. <span data-ttu-id="23ed1-217">Если у вас уже есть его с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для получения последней версии элемента.</span><span class="sxs-lookup"><span data-stu-id="23ed1-217">Use the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation to get the latest version of the item, unless you already have it.</span></span> 
    
2. <span data-ttu-id="23ed1-218">Используйте операцию [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) для определения полей для обновления и назначить новые значения к этим полям.</span><span class="sxs-lookup"><span data-stu-id="23ed1-218">Use the [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) operation to specify fields to update and assign new values to those fields.</span></span> 
    
<span data-ttu-id="23ed1-219">В следующем примере показано XML **UpdateItem** операция запроса, который отправляется на сервер для обновления значение [темы](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="23ed1-219">The following example shows the XML **UpdateItem** operation request that is sent to the server to update the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) value of the email message.</span></span> <span data-ttu-id="23ed1-220">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="23ed1-220">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAPdgr" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>New subject</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="23ed1-221">Сервер отвечает на запрос **UpdateItem** [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что элемент обновление выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="23ed1-221">The server responds to the **UpdateItem** request with a [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item update was successful.</span></span>
  
<span data-ttu-id="23ed1-222">Чтобы узнать, как обновить собрания или встречи с помощью веб-служб Exchange, обратитесь к разделу [Обновить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-222">To learn how to update a meeting or appointment item by using EWS, see [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="23ed1-223">Удаление элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="23ed1-223">Delete an item by using the EWS Managed API</span></span>
<span data-ttu-id="23ed1-224"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-224"></span></span>

<span data-ttu-id="23ed1-225">Можно удалять элементы при перемещении их для папки «Удаленные» или в корзину.</span><span class="sxs-lookup"><span data-stu-id="23ed1-225">You can delete items by moving them to the Deleted Items folder or to the dumpster.</span></span> <span data-ttu-id="23ed1-226">Если вы знаете [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для удаления, просто вызовите метод [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) для элемента.</span><span class="sxs-lookup"><span data-stu-id="23ed1-226">If you know the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to delete, just call the [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) method on the item.</span></span> 
  
<span data-ttu-id="23ed1-227">Если перед удалением элемента необходимо его найти, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="23ed1-227">If you need to find the item before deleting it, do the following:</span></span>
  
1. <span data-ttu-id="23ed1-228">Вызовите метод [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) , чтобы найти элемент, чтобы удалить.</span><span class="sxs-lookup"><span data-stu-id="23ed1-228">Call the [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to find the item to delete.</span></span> 
    
1. <span data-ttu-id="23ed1-229">Создайте экземпляр [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) и ограничить возвращаемых свойств или использование [SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) для поиска конкретных элементов.</span><span class="sxs-lookup"><span data-stu-id="23ed1-229">Instantiate a [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) and limit it to the properties to return, or use a [SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) to find specific items.</span></span> 
    
2. <span data-ttu-id="23ed1-230">Создайте экземпляр [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) или [представления календаря](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) для указания числа элементов для возврата.</span><span class="sxs-lookup"><span data-stu-id="23ed1-230">Instantiate an [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) to specify the number of items to return.</span></span> 
    
2. <span data-ttu-id="23ed1-231">Вызовите метод [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="23ed1-231">Call the [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="23ed1-232">Например, в представленном ниже коде показано, как переместить электронное сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="23ed1-232">For example, the following code shows how to move an email message to the Deleted Items folder.</span></span>
  
<span data-ttu-id="23ed1-233">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="23ed1-233">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="23ed1-234">Локальной переменной *itemId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для обновления.</span><span class="sxs-lookup"><span data-stu-id="23ed1-234">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

<span data-ttu-id="23ed1-235">Для получения дополнительных сведений об удалении элементов видеть [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-235">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="23ed1-236">Чтобы узнать, как удалить собрания или встречи с помощью управляемого интерфейса API веб-служб Exchange, обратитесь к разделу [удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-236">To learn how to delete a meeting or appointment item by using the EWS Managed API, see [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="delete-an-item-by-using-ews"></a><span data-ttu-id="23ed1-237">Удаление элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="23ed1-237">Delete an item by using EWS</span></span>
<span data-ttu-id="23ed1-238"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-238"></span></span>

<span data-ttu-id="23ed1-239">Элемент можно удалить с помощью операции [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="23ed1-239">You can delete an item by using the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) operation.</span></span> 
  
<span data-ttu-id="23ed1-p128">В приведенном ниже примере кода показан XML-запрос, отправляемый на сервер для перемещения электронного сообщения в папку "Удаленные". Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="23ed1-p128">The following example shows the XML request that is sent to the server to move the email message to the Deleted Items folder. The values of some attributes and elements have been shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems">
      <m:ItemIds>
        <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAANIFzC" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="23ed1-242">Сервер отвечает на запрос **DeleteItem** [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что удаления элемента прошла успешно.</span><span class="sxs-lookup"><span data-stu-id="23ed1-242">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes the a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item deletion was successful.</span></span>
  
<span data-ttu-id="23ed1-243">Для получения дополнительных сведений об удалении элементов видеть [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-243">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="23ed1-244">Чтобы узнать, как удалить собрания или встречи с помощью веб-служб Exchange, обратитесь к разделу [удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-244">To learn how to delete a meeting or appointment item by using EWS, see [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span></span>
  
## <a name="move-or-copy-items-to-another-mailbox"></a><span data-ttu-id="23ed1-245">Перемещение или копирование элементов в другой почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="23ed1-245">Move or copy items to another mailbox</span></span>
<span data-ttu-id="23ed1-246"><a name="bk_movecopybtnmailboxes"> </a></span><span class="sxs-lookup"><span data-stu-id="23ed1-246"></span></span>

<span data-ttu-id="23ed1-247">Можно переместить или скопировать элементы между почтовыми ящиками с помощью операции [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) и [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="23ed1-247">You can move or copy items between mailboxes by using the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) and [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) operations.</span></span> <span data-ttu-id="23ed1-248">Чтобы получить дополнительные сведения, обратитесь к разделу [Экспорт и импорт элементов с помощью веб-служб Exchange в Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="23ed1-248">To learn more, see [Exporting and importing items by using EWS in Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="23ed1-249">См. также</span><span class="sxs-lookup"><span data-stu-id="23ed1-249">See also</span></span>

- [<span data-ttu-id="23ed1-250">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="23ed1-250">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)    
- [<span data-ttu-id="23ed1-251">Работа с папками с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="23ed1-251">Work with folders by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="23ed1-252">Удаление элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="23ed1-252">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)
    

