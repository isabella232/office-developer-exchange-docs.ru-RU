---
title: Работа с элементами почтовых ящиков Exchange с помощью веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Узнайте, как создавать, получать, редактировать и удалять элементы с помощью управляемого API EWS или служб EWS в Exchange.
ms.openlocfilehash: a40cd7ae682c1fb0a8d2f9cfcb10d99d4ab08052
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353968"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a><span data-ttu-id="b463f-103">Работа с элементами почтовых ящиков Exchange с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="b463f-103">How to: Work with Exchange mailbox items by using EWS in Exchange</span></span>

<span data-ttu-id="b463f-104">Узнайте, как создавать, получать, редактировать и удалять элементы с помощью управляемого API EWS или служб EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b463f-104">Learn how to create, get, update, and delete items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b463f-105">Вы можете работать с элементами в почтовом ящике с помощью управляемого API EWS или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b463f-105">You can use the EWS Managed API or EWS to work with items in a mailbox.</span></span> <span data-ttu-id="b463f-106">Вы можете использовать универсальные [элементы — объекты ](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)или типы [элементов EWS ](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) для выполнения некоторых операций (получения или удаления элемента по его идентификатору). Однако для получения и обновления элементов чаще всего приходится использовать [строго типизированные элементы](folders-and-items-in-ews-in-exchange.md#bk_item), так как вам потребуется доступ к свойствам, относящимся к строго типизированному элементу.</span><span class="sxs-lookup"><span data-stu-id="b463f-106">You can use generic items — EWS Managed API [Item](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) objects or EWS [Item](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) types — to perform some operations (getting an item or deleting an item by using the item's identifier); however, most of the time you'll have to use a [strongly typed item](folders-and-items-in-ews-in-exchange.md#bk_item) to perform a get or update operation because you'll need access to the properties that are specific to the strongly typed item.</span></span> 

<span data-ttu-id="b463f-107">Например, с помощью универсального элемента невозможно получить элемент, содержащий даты начала и окончания — для этого потребуется объект управляемого API EWS [Appointment](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или тип [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-107">For example, you can't use a generic item to retrieve an item that contains a start and end date - you need an EWS Managed API [Appointment](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) object or an EWS [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) type to do that.</span></span> <span data-ttu-id="b463f-108">А если вы используете управляемый API EWS, то создавать строго типизированные элементы необходимо в любом случае, так как у класса универсального **элемента ** нет конструктора.</span><span class="sxs-lookup"><span data-stu-id="b463f-108">And if you're using the EWS Managed API, you always have to create strongly typed items, because the generic **Item** class does not have a constructor.</span></span> <span data-ttu-id="b463f-109">Для работы с элементом, не являющимся строго типизированным, всегда можно использовать класс базового **элемента**.</span><span class="sxs-lookup"><span data-stu-id="b463f-109">If you're working with an item that is not strongly typed, you can always use the base **Item** class to work with the item.</span></span> 
  
<span data-ttu-id="b463f-110">**Таблица 1. Методы управляемого API EWS и операции EWS для работы с элементами**</span><span class="sxs-lookup"><span data-stu-id="b463f-110">**Table 1.  EWS Managed API methods and EWS operations for working with items**</span></span>

|<span data-ttu-id="b463f-111">**Задача**</span><span class="sxs-lookup"><span data-stu-id="b463f-111">**In order to**</span></span>|<span data-ttu-id="b463f-112">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="b463f-112">**EWS Managed API method**</span></span>|<span data-ttu-id="b463f-113">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="b463f-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b463f-114">Создание универсального элемента</span><span class="sxs-lookup"><span data-stu-id="b463f-114">Create a generic item</span></span>  <br/> |<span data-ttu-id="b463f-p103">С помощью управляемого API EWS можно создавать только элементы определенных типов. Создавать универсальные элементы невозможно.</span><span class="sxs-lookup"><span data-stu-id="b463f-p103">None. You can only create specific item types by using the EWS Managed API; you cannot create generic items.</span></span>  <br/> |[<span data-ttu-id="b463f-117">CreateItem</span><span class="sxs-lookup"><span data-stu-id="b463f-117">CreateItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="b463f-118">Получение элемента</span><span class="sxs-lookup"><span data-stu-id="b463f-118">Get an item</span></span>  <br/> |[<span data-ttu-id="b463f-119">Item.Bind</span><span class="sxs-lookup"><span data-stu-id="b463f-119">Item.Bind</span></span>](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b463f-120">GetItem</span><span class="sxs-lookup"><span data-stu-id="b463f-120">GetItem</span></span>](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="b463f-121">Обновление элемента</span><span class="sxs-lookup"><span data-stu-id="b463f-121">Update an item</span></span>  <br/> |[<span data-ttu-id="b463f-122">Item.Update</span><span class="sxs-lookup"><span data-stu-id="b463f-122">Item.Update</span></span>](http://msdn.microsoft.com/ru-RU/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b463f-123">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="b463f-123">UpdateItem</span></span>](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="b463f-124">Удаление элемента</span><span class="sxs-lookup"><span data-stu-id="b463f-124">Delete an item</span></span>  <br/> |[<span data-ttu-id="b463f-125">Item.Delete</span><span class="sxs-lookup"><span data-stu-id="b463f-125">Item.Delete</span></span>](http://msdn.microsoft.com/ru-RU/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b463f-126">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="b463f-126">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |
   
<span data-ttu-id="b463f-127">Из этой статьи вы узнаете, когда для выполнения задачи можно использовать универсальный базовый класс, а в каких случаях необходимо применять строго типизированный элемент.</span><span class="sxs-lookup"><span data-stu-id="b463f-127">In this article, you’ll learn when you can use the generic base class and when you need to use a strongly typed item to complete your task. The code examples will show you how to use the base class, and what to do when you can’t use the base class or it doesn’t fit your needs.</span></span> <span data-ttu-id="b463f-128">В примерах кода показано, как использовать базовый класс и что делать, если использовать базовый класс невозможно или он не соответствует вашим потребностям.</span><span class="sxs-lookup"><span data-stu-id="b463f-128">In this article, you’ll learn when you can use the generic base class and when you need to use a strongly typed item to complete your task. The code examples will show you how to use the base class, and what to do when you can’t use the base class or it doesn’t fit your needs.</span></span>
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="b463f-129">Создание элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b463f-129">Create an item by using the EWS Managed API</span></span>
<span data-ttu-id="b463f-130"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-130"></span></span>

<span data-ttu-id="b463f-131">В управляемом API EWS нет общедоступного конструктора для класса [элемента](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx), поэтому потребуется использовать конструктор конкретного типа, который необходим для создания элемента.</span><span class="sxs-lookup"><span data-stu-id="b463f-131">The EWS Managed API does not have a publicly available constructor for the [Item](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) class, so you must use the constructor for the specific item type you want to create in order to create an item.</span></span> <span data-ttu-id="b463f-132">Например, с помощью [конструктора класса EmailMessage](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) можно создать новое сообщение электронной почты и с помощью [конструктора класса контактов Contact](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) можно создавать новые контакты.</span><span class="sxs-lookup"><span data-stu-id="b463f-132">For example, use the [EmailMessage class constructor](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) to create a new email message, and the [Contact class constructor](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) to create a new contact.</span></span> <span data-ttu-id="b463f-133">Аналогичным образом, сервер никогда не возвращает в ответах объекты универсального **элемента**. Все универсальные элементы возвращаются в виде объектов **EmailMessage**.</span><span class="sxs-lookup"><span data-stu-id="b463f-133">Likewise, the server never returns generic **Item** objects in responses; all generic items are returned as **EmailMessage** objects.</span></span> 
  
<span data-ttu-id="b463f-p106">Если вы знаете тип создаваемого элемента, выполнить задачу можно всего за несколько этапов. Действия одинаковы для всех типов элементов:</span><span class="sxs-lookup"><span data-stu-id="b463f-p106">When you know the type of item to create, you can complete the task in just a few steps. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="b463f-136">Инициализируйте новый экземпляр одного из классов [элемента](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) с объектом [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в качестве параметра.</span><span class="sxs-lookup"><span data-stu-id="b463f-136">Initialize a new instance of one of the [Item](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) classes with the [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object as a parameter.</span></span> 
    
2. <span data-ttu-id="b463f-p107">Задайте свойства элемента. Для всех типов элементов используются разные схемы, поэтому для разных элементов доступны разные свойства.</span><span class="sxs-lookup"><span data-stu-id="b463f-p107">Set properties on the item. The schemas are different for each item type, so different properties are available for different items.</span></span>
    
3. <span data-ttu-id="b463f-139">Сохраните элемент или сохраните и отправьте его.</span><span class="sxs-lookup"><span data-stu-id="b463f-139">Save the item, or save and send the item.</span></span>
    
<span data-ttu-id="b463f-140">Например, вы можете создать объект [EmailMessage](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) объекта, задавать свойства для [Subject](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) и [ToRecipients](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx), а затем отправлять его с помощью метода [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-140">For example, you can create an [EmailMessage](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object, set the [Subject](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx), and [ToRecipients](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) properties, and then send it by using the [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method.</span></span> 
  
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

<span data-ttu-id="b463f-141">Сведения о том, как создать элемент собрания или встречи с помощью управляемого API EWS, см. в статье [Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-141">To learn how to create a meeting or appointment item by using the EWS Managed API, see How to: Create appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="create-an-item-by-using-ews"></a><span data-ttu-id="b463f-142">Создание элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="b463f-142">Create an item by using EWS</span></span>
<span data-ttu-id="b463f-143"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-143"></span></span>

<span data-ttu-id="b463f-p108">С помощью EWS можно создать универсальный или строго типизированный элемент. Действия одинаковы для всех типов элементов.</span><span class="sxs-lookup"><span data-stu-id="b463f-p108">You can create a generic item or a strongly typed item by using EWS. The steps are similar for all item types:</span></span>
  
1. <span data-ttu-id="b463f-146">Создайте элемент в хранилище Exchange с помощью операции [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-146">Use the [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to create an item in the Exchange store.</span></span> 
    
2. <span data-ttu-id="b463f-147">Используйте элемент [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) в качестве контейнера для одного или нескольких создаваемых элементов.</span><span class="sxs-lookup"><span data-stu-id="b463f-147">Use the [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) element to contain one or more items to create.</span></span> 
    
3. <span data-ttu-id="b463f-148">Задайте свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="b463f-148">Set properties on the item.</span></span>
    
<span data-ttu-id="b463f-149">Например, вы можете создать электронное сообщение и отправить его с помощью кода из представленного ниже примера.</span><span class="sxs-lookup"><span data-stu-id="b463f-149">For example, you can create an email message and send it by using the code in the following example.</span></span> <span data-ttu-id="b463f-150">Управляемое API EWS также отправляет запрос XML при вызове метода [SendAndSaveCopy](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-150">This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [get all attachments from an email](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx).</span></span> 
  
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

<span data-ttu-id="b463f-151">В ответ на запрос **CreateItem** сервер отправляет сообщение [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError**, которое указывает, что сообщение было успешно создано, и свойство [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) созданного сообщения.</span><span class="sxs-lookup"><span data-stu-id="b463f-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="b463f-152">Сведения о том, как создать собрание или встречу с помощью EWS, см. в статье[Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-152">To learn how to create a meeting or appointment item by using EWS, see How to: Create appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="b463f-153">Получение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b463f-153">Get an item by using the EWS Managed API</span></span>
<span data-ttu-id="b463f-154"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-154"></span></span>

<span data-ttu-id="b463f-155">Чтобы использовать управляемое API EWS для получения элемента, если вы знаете свойство [Item.Id](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) получаемого элемента, необходимо просто вызвать один из методов [Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) в элементе, после чего элемент будет получен.</span><span class="sxs-lookup"><span data-stu-id="b463f-155">To use the EWS Managed API to get an item if you know the [Item.Id](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to retrieve, you simply call one of the [Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) methods on the item, and the item is retrieved.</span></span> <span data-ttu-id="b463f-156">Рекомендуем возвращать только обязательные свойства.</span><span class="sxs-lookup"><span data-stu-id="b463f-156">As a best practice, we recommend that you limit the properties returned to only those that are required.</span></span> <span data-ttu-id="b463f-157">В этом примере возвращаются свойства **Id** элемента и **Subject**.</span><span class="sxs-lookup"><span data-stu-id="b463f-157">This example returns the item **Id** property and the **Subject** property.</span></span> 
  
<span data-ttu-id="b463f-158">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="b463f-158">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that itemId is the ItemId of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="b463f-159">Локальная переменная *itemId* является [идентификатором](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) обновляемого элемента.</span><span class="sxs-lookup"><span data-stu-id="b463f-159">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

<span data-ttu-id="b463f-160">Чтобы найти элемент, отвечающий определенным условиям, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="b463f-160">If you’re searching for an item that meets specific criteria, do the following:</span></span>
  
1. <span data-ttu-id="b463f-161">Выполните привязку к папке, содержащей получаемые элементы.</span><span class="sxs-lookup"><span data-stu-id="b463f-161">Bind to the folder that contains the items to get.</span></span>
    
2. <span data-ttu-id="b463f-162">Создайте экземпляр [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) или [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) для фильтрации элементов на возврат.</span><span class="sxs-lookup"><span data-stu-id="b463f-162">Instantiate a [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) or a [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) to filter the items to return.</span></span> 
    
3. <span data-ttu-id="b463f-163">Создайте экземпляр объекта [ItemView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) или [CalendarView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx), чтобы указать количество элементов на возврат.</span><span class="sxs-lookup"><span data-stu-id="b463f-163">Instantiate an [ItemView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) object to specify the number of items to return.</span></span> 
    
4. <span data-ttu-id="b463f-164">Вызовите метод [ExchangeService.FindItems](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или [ExchangeService.FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-164">Call the [ExchangeService.FindItems](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [ExchangeService.FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="b463f-165">Например, чтобы получить непрочитанные электронные сообщения из папки "Входящие", используйте код из приведенного ниже примера.</span><span class="sxs-lookup"><span data-stu-id="b463f-165">For example, if you want to retrieve unread email messages in the Inbox, use the code in the following example.</span></span> <span data-ttu-id="b463f-166">В этом примере используется **SearchFilterCollection** для ограничения результатов метода **FindItems** до непрочитанных сообщений, а с помощью объекта **ItemView** результаты можно сократить до одного элемента.</span><span class="sxs-lookup"><span data-stu-id="b463f-166">This example uses a **SearchFilterCollection** to limit the results of the **FindItems** method to unread messages, and limits the **ItemView** to limit results to one item.</span></span> <span data-ttu-id="b463f-167">Этот конкретный код работает только в объектах [EmailMessage](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) объекты, поскольку значение [EmailMessageSchema.IsRead](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) является частью **SearchFilter**.</span><span class="sxs-lookup"><span data-stu-id="b463f-167">This particular code only works on [EmailMessage](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects because the [EmailMessageSchema.IsRead](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) value is part of the **SearchFilter**.</span></span> 
  
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

<span data-ttu-id="b463f-168">Кроме того, вы можете использовать [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) чтобы ограничить результаты поиска, как показано в приведенном ниже примере кода.</span><span class="sxs-lookup"><span data-stu-id="b463f-168">Alternatively, you can use a [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) to limit the results of the search as shown in the following code example.</span></span> <span data-ttu-id="b463f-169">В этом примере используется метод [FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) для получения до пяти встреч, которые произойдут в течение следующих 30 дней.</span><span class="sxs-lookup"><span data-stu-id="b463f-169">This example uses the [FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to retrieve up to five appointments that occur in the next 30 days.</span></span> <span data-ttu-id="b463f-170">Конечно, этот код работает только с элементами календаря.</span><span class="sxs-lookup"><span data-stu-id="b463f-170">This code of course only works on calendar items.</span></span> 
  
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

<span data-ttu-id="b463f-171">Обратите внимание, что данные, возвращаемые сервером в ответ на вызов метода **Bind**, отличаются от аналогичных данных, возвращаемых сервером в ответ на методы **FindItem** или **FindAppointment**.</span><span class="sxs-lookup"><span data-stu-id="b463f-171">Note that the information the server returns in the **Bind** method response is different than the information that the server returns for a **FindItem** or **FindAppointment** method response.</span></span> <span data-ttu-id="b463f-172">Метод **Bind** может возвращать все схематизированные свойства, в то время как методы **FindItem** и **FindAppointment** возвращают не все из этих свойств.</span><span class="sxs-lookup"><span data-stu-id="b463f-172">The **Bind** method can return all the schematized properties, whereas the **FindItem** and **FindAppointment** methods do not return all the schematized properties.</span></span> <span data-ttu-id="b463f-173">Следовательно, если вам нужен полный доступ к элементу, то необходимо использовать метод **Bind**.</span><span class="sxs-lookup"><span data-stu-id="b463f-173">So if you need full access to the item, you'll have to use the **Bind** method.</span></span> <span data-ttu-id="b463f-174">Если вам неизвестно значение свойства **Id** получаемого элемента, используйте методы **FindItem** или **FindAppointment**, чтобы получить свойство Id, а затем получите необходимые свойства с помощью метода **Bind**.</span><span class="sxs-lookup"><span data-stu-id="b463f-174">If you don't have the item **Id** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** methods to retrieve the Id, and then use the **Bind** method to retrieve the properties you need.</span></span> 
  
<span data-ttu-id="b463f-175">Сведения о том, как получить элемент собрания или встречи с помощью управляемого API EWS, см. в статье [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-175">To learn how to get a meeting or appointment item by using the EWS Managed API, see How to: Get appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="get-an-item-by-using-ews"></a><span data-ttu-id="b463f-176">Получение элемента с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="b463f-176">Get an item by using EWS</span></span>
<span data-ttu-id="b463f-177"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-177"></span></span>

<span data-ttu-id="b463f-178">Если вам известно значение свойства [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) получаемого элемента, то вы можете получить его с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-178">If you know the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the item to retrieve, you can get the item by using the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation.</span></span> 
  
<span data-ttu-id="b463f-179">В приведенном ниже примере показан XML-запрос на получение свойства [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) элемента с определенным значением свойства **ItemId**.</span><span class="sxs-lookup"><span data-stu-id="b463f-179">The following example shows the XML request to get the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of an item with a specific **ItemId**.</span></span> <span data-ttu-id="b463f-180">Управляемое API EWS также отправляет запрос XML при вызове метода [Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) на **ItemId**.</span><span class="sxs-lookup"><span data-stu-id="b463f-180">This is also the XML request that the EWS Managed API sends when calling the [Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method on an **ItemId**.</span></span> <span data-ttu-id="b463f-181">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="b463f-181">The values of some attributes and elements have been shortened for readability.</span></span>
  
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

<span data-ttu-id="b463f-p116">В приведенном ниже примере показан XML-ответ, возвращаемый сервером после обработки операции **GetItem**. Ответ указывает, что элемент был успешно получен. Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="b463f-p116">The following example shows the XML response that the server returns after it processes the **GetItem** operation. The response indicates the item was retrieved successfully. The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="b463f-185">Если вы не знаете значение свойства **ItemId** получаемого элемента, его можно найти с помощью операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-185">If you do not know the **ItemId** of the item you want to retrieve, you can use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find the item.</span></span> <span data-ttu-id="b463f-186">Для использования операции **FindItem** необходимо сначала определить папку для поиска.</span><span class="sxs-lookup"><span data-stu-id="b463f-186">In order to use the **FindItem** operation, you must first identify the folder that you're searching.</span></span> <span data-ttu-id="b463f-187">Это можно сделать с помощью свойства **DistinguinguishedFolderName** или [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-187">You can identify the folder by using its **DistinguinguishedFolderName** or by using the [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx).</span></span> <span data-ttu-id="b463f-188">Можно использовать операцию [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) или [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx), чтобы получить нужное свойство **FolderId**.</span><span class="sxs-lookup"><span data-stu-id="b463f-188">You can use either the [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) or [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) operations to get the **FolderId** you need.</span></span> <span data-ttu-id="b463f-189">Затем с помощью операции **FindItem** найдите в папке результаты, соответствующие фильтру поиска.</span><span class="sxs-lookup"><span data-stu-id="b463f-189">Then use the **FindItem** operation to search that folder for results that match the search filter.</span></span> <span data-ttu-id="b463f-190">В отличие от управляемого API EWS, в веб-службах Exchange нет отдельной операции поиска для встреч.</span><span class="sxs-lookup"><span data-stu-id="b463f-190">Unlike the EWS Managed API, EWS does not provide a separate find operation for appointments.</span></span> <span data-ttu-id="b463f-191">Операция **FindItem** получает элементы всех типов.</span><span class="sxs-lookup"><span data-stu-id="b463f-191">The **FindItem** operation retrieves items of all types.</span></span> 
  
<span data-ttu-id="b463f-p118">В приведенном ниже примере показан XML-запрос с операцией **FindItem**, отправляемый на сервер для поиска в папке Calendar встреч, назначенных на следующие 30 дней. Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="b463f-p118">The following example shows the XML **FindItem** operation request that is sent to the server to find appointments in the Calendar folder that occur in the next 30 days. The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="b463f-p119">В ответ на запрос **FindItem** сервер возвращает сообщение [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) со значением **NoError**, которое указывает, что операция успешно выполнена. Если какие-либо элементы календаря отвечают условиям фильтра, они включаются в ответ.</span><span class="sxs-lookup"><span data-stu-id="b463f-p119">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes the [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the operation completed successfully. If any calendar items meet the filtering criteria, they are included in the response.</span></span>
  
<span data-ttu-id="b463f-196">Обратите внимание, что данные, возвращаемые сервером в ответ на вызов операции **GetItem**, отличаются от аналогичных данных для операций **FindItem** или **FindAppointment**.</span><span class="sxs-lookup"><span data-stu-id="b463f-196">Note that the information the server returns in the **GetItem** operation response is different than the information the server returns in a **FindItem** or **FindAppointment** operation response.</span></span> <span data-ttu-id="b463f-197">Операция **GetItem** может возвращать все схематизированные свойства, в то время как операции **FindItem** и **FindAppointment** возвращают не все из этих свойств.</span><span class="sxs-lookup"><span data-stu-id="b463f-197">The **GetItem** operation can return all the schematized properties, whereas the **FindItem** and **FindAppointment** operations do not return all the schematized properties.</span></span> <span data-ttu-id="b463f-198">Следовательно, если вам нужен полный доступ к элементу, то необходимо использовать операцию **GetItem**.</span><span class="sxs-lookup"><span data-stu-id="b463f-198">So if you need full access to the item, you'll have to use the **GetItem** operation.</span></span> <span data-ttu-id="b463f-199">Если вам неизвестно значение свойства **ItemId** получаемого элемента, используйте операции **FindItem** или **FindAppointment**, чтобы получить свойство **ItemId**, а затем получите необходимые элементы с помощью операции **GetItem**.</span><span class="sxs-lookup"><span data-stu-id="b463f-199">If you don't have the **ItemId** of the item you'd like to retrieve, use the **FindItem** or **FindAppointment** operations to retrieve the **ItemId**, and then use the **GetItem** operation to retrieve the elements you need.</span></span> 
  
<span data-ttu-id="b463f-200">Сведения о том, как получить элемент собрания или встречи с помощью EWS, см. в статье [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-200">To learn how to get a meeting or appointment item by using EWS, see How to: Get appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="b463f-201">Изменение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b463f-201">Update an item by using the EWS Managed API</span></span>
<span data-ttu-id="b463f-202"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-202"></span></span>

<span data-ttu-id="b463f-203">Действия для изменения элемента с помощью управляемого API EWS одинаковы для всех типов элементов. Однако элементы разных типов содержат разные свойства, а для метода [Update](http://msdn.microsoft.com/ru-RU/library/office/dd635915%28v=exchg.80%29.aspx) доступно множество перегруженных методов.</span><span class="sxs-lookup"><span data-stu-id="b463f-203">The steps to update an item by using the EWS Managed API are similar for all item types; however, the item properties are different for each item type, and the [Updatehttp://msdn.microsoft.com/en-us/library/office/dd635915(v=exchg.80).aspx](http://msdn.microsoft.com/ru-RU/library/office/dd635915%28v=exchg.80%29.aspx) method has many overloaded methods to choose from. To update an item:</span></span> <span data-ttu-id="b463f-204">Чтобы обновить элемент, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="b463f-204">To update an item:</span></span> 
  
1. <span data-ttu-id="b463f-205">Получите последнюю версию элемента (если ее у вас еще нет) с помощью метода [Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-205">Use the [GetItem](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) operation to get the latest version of the item, unless you already have it.</span></span> <span data-ttu-id="b463f-206">Чтобы редактировать свойства, относящиеся к строго типизированному элементу, необходимо выполнить привязку к типу этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b463f-206">To update properties specific to a strongly typed item, you'll have to bind to that item type.</span></span> <span data-ttu-id="b463f-207">Чтобы изменить свойства, доступные для типа универсальный элемента, вы можете выполнить привязку к объекту [элемента](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-207">To update properties available on the generic item type, you can bind to the [Item](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) object.</span></span> 
    
2. <span data-ttu-id="b463f-208">Обновите свойства элемента.</span><span class="sxs-lookup"><span data-stu-id="b463f-208">Update the properties on the item.</span></span>
    
3. <span data-ttu-id="b463f-209">Вызовите метод **Update**.</span><span class="sxs-lookup"><span data-stu-id="b463f-209">Call the **Update** method.</span></span> 
    
<span data-ttu-id="b463f-210">Например, вы можете изменить тему сообщения с помощью универсального типа элемента, как показано в коде приведенного ниже примера.</span><span class="sxs-lookup"><span data-stu-id="b463f-210">For example, you can update the subject of an email by using the generic item type, as shown in the code in the following example.</span></span>
  
<span data-ttu-id="b463f-211">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="b463f-211">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that itemId is the ItemId of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="b463f-212">Локальная переменная *itemId* является [идентификатором](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) обновляемого элемента.</span><span class="sxs-lookup"><span data-stu-id="b463f-212">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
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

<span data-ttu-id="b463f-213">Сведения о том, как обновить элемент собрания или встречи с помощью управляемого API EWS, см. в статье [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-213">To learn how to update a meeting or appointment item by using the EWS Managed API, see How to: Update appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="update-an-item-by-using-ews"></a><span data-ttu-id="b463f-214">Обновление элемента с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="b463f-214">Update an item by using EWS</span></span>
<span data-ttu-id="b463f-215"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-215"></span></span>

<span data-ttu-id="b463f-216">Чтобы обновить элемент с помощью EWS, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="b463f-216">To update an item by using EWS, do the following:</span></span>
  
1. <span data-ttu-id="b463f-217">Получите последнюю версию элемента (если ее у вас еще нет) с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-217">Use the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) operation to get the latest version of the item, unless you already have it.</span></span> 
    
2. <span data-ttu-id="b463f-218">Укажите редактируемые поля и присвойте им новые значения с помощью операции [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-218">Use the [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) operation to specify fields to update and assign new values to those fields.</span></span> 
    
<span data-ttu-id="b463f-p124">В приведенном ниже примере показан XML-запрос с операцией **UpdateItem**, который отправляется на сервер для изменения свойства [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) электронного сообщения. Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="b463f-p124">The following example shows the XML **UpdateItem** operation request that is sent to the server to update the [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) value of the email message. The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="b463f-221">В ответ на запрос **UpdateItem** сервер отправляет сообщение [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError**, которое указывает, что элемент успешно обновлен.</span><span class="sxs-lookup"><span data-stu-id="b463f-221">The server responds to the **UpdateItem** request with a [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes the a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item update was successful.</span></span>
  
<span data-ttu-id="b463f-222">Сведения о том, как изменить элемент собрания или встречи с помощью веб-служб Exchange, см. в статье [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-222">To learn how to update a meeting or appointment item by using EWS, see How to: Update appointments and meetings by using EWS in Exchange 2013.</span></span>
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a><span data-ttu-id="b463f-223">Удаление элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="b463f-223">Delete an item by using the EWS Managed API</span></span>
<span data-ttu-id="b463f-224"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-224"></span></span>

<span data-ttu-id="b463f-225">Вы можете удалять элементы, перемещая их в папку "Удаленные" или в корзину.</span><span class="sxs-lookup"><span data-stu-id="b463f-225">You can delete items by moving them to the Deleted Items folder or to the dumpster.</span></span> <span data-ttu-id="b463f-226">Если вы знаете [ItemId](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) удаляемого элемента, то просто вызовите метод [Delete](http://msdn.microsoft.com/ru-RU/library/office/dd635072%28v=exchg.80%29.aspx) в элементе.</span><span class="sxs-lookup"><span data-stu-id="b463f-226">If you know the [ItemId](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to delete, just call the [Delete](http://msdn.microsoft.com/ru-RU/library/office/dd635072%28v=exchg.80%29.aspx) method on the item.</span></span> 
  
<span data-ttu-id="b463f-227">Если перед удалением элемента необходимо его найти, сделайте следующее:</span><span class="sxs-lookup"><span data-stu-id="b463f-227">If you need to find the item before deleting it, do the following:</span></span>
  
1. <span data-ttu-id="b463f-228">Вызовите метод [FindItems](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или [FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx), чтобы найти удаляемый элемент.</span><span class="sxs-lookup"><span data-stu-id="b463f-228">Call the [FindItems](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) or [FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) method to find the item to delete.</span></span> 
    
1. <span data-ttu-id="b463f-229">Создайте экземпляр [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) и ограничьте его до свойств для возврата или используйте [SearchFilterCollection](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) для поиска определенных элементов.</span><span class="sxs-lookup"><span data-stu-id="b463f-229">Instantiate a [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) and limit it to the properties to return, or use a [SearchFilterCollection](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) to find specific items.</span></span> 
    
2. <span data-ttu-id="b463f-230">Создайте экземпляр [ItemView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) или [CalendarView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx), чтобы указать количество элементов на возврат.</span><span class="sxs-lookup"><span data-stu-id="b463f-230">Instantiate an [ItemView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) or [CalendarView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) to specify the number of items to return.</span></span> 
    
2. <span data-ttu-id="b463f-231">Вызовите метод [Delete](http://msdn.microsoft.com/ru-RU/library/office/dd635072%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-231">Call the [Delete](http://msdn.microsoft.com/ru-RU/library/office/dd635072%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="b463f-232">Например, в представленном ниже коде показано, как переместить электронное сообщение в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="b463f-232">For example, the following code shows how to move an email message to the Deleted Items folder.</span></span>
  
<span data-ttu-id="b463f-233">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="b463f-233">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that itemId is the ItemId of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="b463f-234">Локальная переменная *itemId* является [идентификатором](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) обновляемого элемента.</span><span class="sxs-lookup"><span data-stu-id="b463f-234">The local variable  *itemId*  is the [Id](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to update.</span></span> 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

<span data-ttu-id="b463f-235">Дополнительные сведения об удалении элементов см. в статье [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-235">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="b463f-236">Сведения о том, как удалить элемент собрания или встречи с помощью управляемого API EWS, см. в статье [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-236">For more details about deleting items, see Deleting items by using EWS in Exchange. To learn how to delete a meeting or appointment item by using the EWS Managed API, see How to: Delete appointments and cancel meetings by using EWS in Exchange.</span></span>
  
## <a name="delete-an-item-by-using-ews"></a><span data-ttu-id="b463f-237">Удаление элемента с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="b463f-237">Delete an item by using EWS</span></span>
<span data-ttu-id="b463f-238"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-238"></span></span>

<span data-ttu-id="b463f-239">Вы можете удалить элемент с помощью операции [DeleteItem](../web-service-reference/deleteitem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-239">You can delete an item by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation.</span></span> 
  
<span data-ttu-id="b463f-p128">В приведенном ниже примере кода показан XML-запрос, отправляемый на сервер для перемещения электронного сообщения в папку "Удаленные". Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="b463f-p128">The following example shows the XML request that is sent to the server to move the email message to the Deleted Items folder. The values of some attributes and elements have been shortened for readability.</span></span>
  
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

<span data-ttu-id="b463f-242">В ответ на запрос **DeleteItem** сервер отправляет сообщение [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError**, которое указывает, что элемент успешно удален.</span><span class="sxs-lookup"><span data-stu-id="b463f-242">The server responds to the **DeleteItem** request with a [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes the a [ResponseCodehttp://msdn.microsoft.com/en-us/library/aa580757(v=exchg.150).aspx](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the item deletion was successful.</span></span>
  
<span data-ttu-id="b463f-243">Дополнительные сведения об удалении элементов см. в статье [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-243">For more details about deleting items, see [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md).</span></span> <span data-ttu-id="b463f-244">Сведения о том, как удалить элемент собрания или встречи с помощью EWS, см. в статье [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-244">For more details about deleting items, see Deleting items by using EWS in Exchange. To learn how to delete a meeting or appointment item by using EWS, see How to: Delete appointments and cancel meetings by using EWS in Exchange.</span></span>
  
## <a name="move-or-copy-items-to-another-mailbox"></a><span data-ttu-id="b463f-245">Перемещение или копирование элементов в другой почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="b463f-245">Move or copy items to another mailbox</span></span>
<span data-ttu-id="b463f-246"><a name="bk_movecopybtnmailboxes"> </a></span><span class="sxs-lookup"><span data-stu-id="b463f-246"></span></span>

<span data-ttu-id="b463f-247">Вы можете перемещать и копировать элементы между почтовыми ящиками с помощью операций [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) и [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="b463f-247">You can move or copy items between mailboxes by using the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) and [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) operations. To learn more, see Importing and exporting items by using EWS in Exchange.</span></span> <span data-ttu-id="b463f-248">Дополнительные сведения см. в статье [Exporting and importing items by using EWS in Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b463f-248">To learn more, see [Exporting and importing items by using EWS in Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b463f-249">См. также</span><span class="sxs-lookup"><span data-stu-id="b463f-249">See also</span></span>

- [<span data-ttu-id="b463f-250">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="b463f-250">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)    
- [<span data-ttu-id="b463f-251">Работа с папками с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b463f-251">How to: Work with Exchange mailbox items by using EWS in Exchange</span></span>](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="b463f-252">Удаление элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="b463f-252">Deleting items by using EWS in Exchange</span></span>](deleting-items-by-using-ews-in-exchange.md)
    

