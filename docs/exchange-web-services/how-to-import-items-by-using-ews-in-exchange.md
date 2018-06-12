---
title: Импорт элементов с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Узнайте, как импортировать встречи, сообщения электронной почты, контакты, задачи и других элементов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: c09c96eff455b7584b084e71b937853abfde731d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761068"
---
# <a name="import-items-by-using-ews-in-exchange"></a><span data-ttu-id="39f54-103">Импорт элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="39f54-103">Import items by using EWS in Exchange</span></span>

<span data-ttu-id="39f54-104">Узнайте, как импортировать встречи, сообщения электронной почты, контакты, задачи и других элементов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="39f54-104">Learn how to import appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="39f54-105">Многие системы содержат встреч, сообщения электронной почты, контакты и задачи, и можно импортировать эти элементы в Exchange в несколько способов.</span><span class="sxs-lookup"><span data-stu-id="39f54-105">Many systems contain appointments, emails, contacts, and tasks, and you can import those items into Exchange in a number of different ways.</span></span> <span data-ttu-id="39f54-106">Импорт элементов в Exchange при простой связи почтового ящика не сохраняются на этих элементов.</span><span class="sxs-lookup"><span data-stu-id="39f54-106">Importing items into Exchange is simple when mailbox relationships aren't maintained on those items.</span></span> <span data-ttu-id="39f54-107">Можно использовать метод управляемый API EWS [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) или операции EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания элементов в почтовый ящик Exchange.</span><span class="sxs-lookup"><span data-stu-id="39f54-107">You can use the [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to create the items in an Exchange mailbox.</span></span> <span data-ttu-id="39f54-108">Простой подход не поддерживает все сценарии Например:</span><span class="sxs-lookup"><span data-stu-id="39f54-108">The simple approach does not support all scenarios, however; for example:</span></span> 
  
- <span data-ttu-id="39f54-109">Не может обеспечить согласованность между организаторов и участники при импорте встреч человек (собрания).</span><span class="sxs-lookup"><span data-stu-id="39f54-109">You cannot maintain the relationship between organizers and attendees when importing appointments with attendees (meetings).</span></span> <span data-ttu-id="39f54-110">Это означает, что организатор собрания могут потребоваться для повторной отправки приглашения на собрания участникам, чтобы восстановить связь между организатора и участников.</span><span class="sxs-lookup"><span data-stu-id="39f54-110">This means that the meeting organizer will need to resend meeting invites to attendees in order to reestablish the relationship between the organizer and attendees.</span></span> <span data-ttu-id="39f54-111">Если Встреча была импортирована в календаре участника, встречи не связаны с организатором встречи.</span><span class="sxs-lookup"><span data-stu-id="39f54-111">If the appointment was imported into an attendee's calendar, the appointment will not be related to the meeting organizer's appointment.</span></span> <span data-ttu-id="39f54-112">Участники, необходимо принять повторно отправленная приглашение из картинок для возобновления отношения Организатор attendee.</span><span class="sxs-lookup"><span data-stu-id="39f54-112">The attendees will need to accept the resent meeting invite from the organizer in order to reestablish the organizer-attendee relationship.</span></span>
    
- <span data-ttu-id="39f54-113">Сведения о назначенных не сохраняются при импорте назначенных задач.</span><span class="sxs-lookup"><span data-stu-id="39f54-113">Information about the assignees is not preserved when assigned tasks are imported.</span></span>
    
<span data-ttu-id="39f54-114">Все параметры импорта можно использовать для пакетного импорта элементов в Exchange.</span><span class="sxs-lookup"><span data-stu-id="39f54-114">All the import options can be used to batch import items into Exchange.</span></span>
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a><span data-ttu-id="39f54-115">Управляемый API EWS использования или веб-служб Exchange типов для импорта элемента элементов</span><span class="sxs-lookup"><span data-stu-id="39f54-115">Use EWS Managed API or EWS item types to import an item</span></span>
<span data-ttu-id="39f54-116"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="39f54-116"></span></span>

<span data-ttu-id="39f54-117">Управляемый API EWS или веб-служб Exchange можно использовать для импорта сообщения электронной почты, контакты, встречи или задачи из других систем.</span><span class="sxs-lookup"><span data-stu-id="39f54-117">You can use the EWS Managed API or EWS to import emails, contacts, appointments, or tasks from other systems.</span></span> <span data-ttu-id="39f54-118">Снова задайте [Свойства](properties-and-extended-properties-in-ews-in-exchange.md) из исходный формат на любой из следующих объектов в зависимости от того, что импорт.</span><span class="sxs-lookup"><span data-stu-id="39f54-118">Just set the [properties ](properties-and-extended-properties-in-ews-in-exchange.md) from your source format on any of the following objects, depending on what you're importing.</span></span> 
  
<span data-ttu-id="39f54-119">**В таблице 1. Управляемый API EWS объекты и элементы веб-служб Exchange**</span><span class="sxs-lookup"><span data-stu-id="39f54-119">**Table 1. EWS Managed API objects and EWS elements**</span></span>

|<span data-ttu-id="39f54-120">**Управляемый API EWS объектов**</span><span class="sxs-lookup"><span data-stu-id="39f54-120">**EWS Managed API object**</span></span>|<span data-ttu-id="39f54-121">**Элемент веб-служб Exchange**</span><span class="sxs-lookup"><span data-stu-id="39f54-121">**EWS element**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39f54-122">EmailMessage</span><span class="sxs-lookup"><span data-stu-id="39f54-122">EmailMessage</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="39f54-123">Message</span><span class="sxs-lookup"><span data-stu-id="39f54-123">Message</span></span>](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="39f54-124">Контакт</span><span class="sxs-lookup"><span data-stu-id="39f54-124">Contact</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="39f54-125">Контакт</span><span class="sxs-lookup"><span data-stu-id="39f54-125">Contact</span></span>](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="39f54-126">Встреча</span><span class="sxs-lookup"><span data-stu-id="39f54-126">Appointment</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="39f54-127">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="39f54-127">CalendarItem</span></span>](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[<span data-ttu-id="39f54-128">Задача</span><span class="sxs-lookup"><span data-stu-id="39f54-128">Task</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="39f54-129">Задача</span><span class="sxs-lookup"><span data-stu-id="39f54-129">Task</span></span>](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="39f54-130">Используйте метод управляемый API EWS [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) или [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) операции веб-служб Exchange для выполнения импорта элементов.</span><span class="sxs-lookup"><span data-stu-id="39f54-130">Use the [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to perform the import of items.</span></span> <span data-ttu-id="39f54-131">Такой подход рекомендуется при импорте элементов из других систем потому, что у вас есть элемент управления, через который импортируется свойства.</span><span class="sxs-lookup"><span data-stu-id="39f54-131">We recommend this approach when you're importing items from other systems because you have control over which properties get imported.</span></span> <span data-ttu-id="39f54-132">Дополнительные сведения о том, как задать свойства элементов, а затем сохраните элемент можно [Создать элемент с помощью управляемого интерфейса API веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) или [Создать элемент с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="39f54-132">For more information about how to set properties on items and then save the item, see [Create an item by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) or [Create an item by using EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).</span></span>
  
## <a name="import-items-with-full-fidelity"></a><span data-ttu-id="39f54-133">Импорт элементов с корректном</span><span class="sxs-lookup"><span data-stu-id="39f54-133">Import items with full fidelity</span></span>
<span data-ttu-id="39f54-134"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="39f54-134"></span></span>

<span data-ttu-id="39f54-135">Отправка элемента как поток данных можно использовать операцию EWS [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="39f54-135">You can use the [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS operation to upload an item as a data stream.</span></span> <span data-ttu-id="39f54-136">Представление потока данных этот элемент должен поступают из результаты вызова операции [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="39f54-136">This data stream representation of an item has to come from the results of an [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) operation call.</span></span> <span data-ttu-id="39f54-137">Так как управляемый API EWS не реализует операцию **UploadItems** при использовании управляемого интерфейса API веб-служб Exchange, необходимые для написания процедуры для отправки веб-запросов.</span><span class="sxs-lookup"><span data-stu-id="39f54-137">Because the EWS Managed API does not implement the **UploadItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> 
  
<span data-ttu-id="39f54-138">Это самый простой способ импорта элементов, которые были экспортированы из другой сервер Exchange.</span><span class="sxs-lookup"><span data-stu-id="39f54-138">This is the easiest way to import items that have been exported from another Exchange server.</span></span>
  
<span data-ttu-id="39f54-139">В следующем примере содержимое элемента **данных** и идентификаторы сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="39f54-139">In the following example, the identifiers and the **Data** element content are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId  Id="AAMkADEzOTE7kV0AAA=" ChangeKey="AQAAAA=="/>
          <t:Data>AQAAAAgAAAAAAQAAAAADABZADQASDkANABMO</t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **UploadItems** с элементом [UploadItemsResponse](http://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) , что, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что элемент был отправлен успешно. <span data-ttu-id="39f54-141">Ответ также включает в себя идентификатор элемента загруженного элемента.</span><span class="sxs-lookup"><span data-stu-id="39f54-141">The response also includes the item ID of the uploaded item.</span></span> 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a><span data-ttu-id="39f54-142">Использовать MIME-поток для импорта из распространенные форматы файлов</span><span class="sxs-lookup"><span data-stu-id="39f54-142">Use the MIME stream to import from common file formats</span></span>
<span data-ttu-id="39f54-143"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="39f54-143"></span></span>

<span data-ttu-id="39f54-144">Веб-служб Exchange можно импортировать файлы iCal (.ics) и EML (файл).</span><span class="sxs-lookup"><span data-stu-id="39f54-144">EWS can import EML (.eml) and iCal (.ics) files.</span></span> <span data-ttu-id="39f54-145">Может потребоваться для проверки содержимого MIME для просмотра как средство синтаксического анализа Exchange MIME обрабатывает содержимого MIME-поток.</span><span class="sxs-lookup"><span data-stu-id="39f54-145">You'll want to test your MIME content to see how the Exchange MIME parser handles the content of your MIME stream.</span></span> <span data-ttu-id="39f54-146">Хотя использование MIME-поток удобен, обычно лучше [типов для импорта элемента элементов управляемый API EWS использования или веб-служб Exchange](#bk_importproperties).</span><span class="sxs-lookup"><span data-stu-id="39f54-146">Although using the MIME stream is convenient, it is typically better to [Use EWS Managed API or EWS item types to import an item](#bk_importproperties).</span></span> <span data-ttu-id="39f54-147">Ниже приведен пример того, как для [импорта визитной карточки](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span><span class="sxs-lookup"><span data-stu-id="39f54-147">Here's an example of how to [import a vCard](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).</span></span>
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a><span data-ttu-id="39f54-148">Использовать управляемый API EWS для импорта на адрес электронной почты из EML-файла с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="39f54-148">Use the EWS Managed API to import an email from an EML file by using the MIME stream</span></span>

<span data-ttu-id="39f54-149">Следующем примере показано, как задать свойство [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) с содержимым EML-файла, а затем импортировать сообщение электронной почты в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="39f54-149">The following example shows how to set the [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property with the contents of an EML file and then import the email into a mailbox.</span></span> <span data-ttu-id="39f54-150">В этом примере также показано, как задать [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) расширенные свойства на импортированных электронной почты, чтобы он не отображается в почтовом ящике как черновик элемента.</span><span class="sxs-lookup"><span data-stu-id="39f54-150">This example also shows how to set the [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) extended property on an imported email so that it doesn't appear in the mailbox as a draft item.</span></span> <span data-ttu-id="39f54-151">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и пользователь может выполнять проверку подлинности для Exchange server.</span><span class="sxs-lookup"><span data-stu-id="39f54-151">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void UploadMIMEEmail(ExchangeService service)
{
    EmailMessage email = new EmailMessage(service);
    
    string emlFileName = @"C:\import\email.eml";
    using (FileStream fs = new FileStream(emlFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .eml file to the MimeContent property.
        email.MimeContent = new MimeContent("UTF-8", bytes);
    }
    
    // Indicate that this email is not a draft. Otherwise, the email will appear as a 
    // draft to clients.
    ExtendedPropertyDefinition PR_MESSAGE_FLAGS_msgflag_read = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
    email.SetExtendedProperty(PR_MESSAGE_FLAGS_msgflag_read, 1);
    // This results in a CreateItem call to EWS. The email will be saved in the Inbox folder.
    email.Save(WellKnownFolderName.Inbox);
}
```

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="39f54-152">Использовать управляемый API EWS для импорта встречу из iCal файла с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="39f54-152">Use the EWS Managed API to import an appointment from an iCal file by using the MIME stream</span></span>

<span data-ttu-id="39f54-153">Простой встречи в формате iCalendar файлы можно импортировать с помощью MIME-поток.</span><span class="sxs-lookup"><span data-stu-id="39f54-153">You can import simple appointments in the form of iCalendar files by using the MIME stream.</span></span> <span data-ttu-id="39f54-154">Нельзя импортировать собраний, которые являются встреч человек, так как связь между организаторам собрания и участников должно быть задано как часть рабочего процесса, [Ведение календаря Exchange](calendars-and-ews-in-exchange.md) .</span><span class="sxs-lookup"><span data-stu-id="39f54-154">You can't import meetings, which are appointments with attendees, because the relationship between meeting organizers and attendees has to be set as part of the [Exchange calendaring](calendars-and-ews-in-exchange.md) workflow.</span></span> <span data-ttu-id="39f54-155">Участники не могут записаны в MIME-поток.</span><span class="sxs-lookup"><span data-stu-id="39f54-155">Attendees cannot be captured in the MIME stream.</span></span> 
  
<span data-ttu-id="39f54-156">В следующем примере кода показано, как для импорта простой ICS-файл в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="39f54-156">The following code example shows you how to import a simple .ics file into a user's mailbox.</span></span>
  
```cs
private static void UploadMIMEAppointment(ExchangeService service)
{
    Appointment appointment = new Appointment(service);
    string iCalFileName = @"C:\import\appointment.ics";
    using (FileStream fs = new FileStream(iCalFileName, FileMode.Open, FileAccess.Read))
    {
        byte[] bytes = new byte[fs.Length];
        int numBytesToRead = (int)fs.Length;
        int numBytesRead = 0;
        while (numBytesToRead > 0)
        {
            int n = fs.Read(bytes, numBytesRead, numBytesToRead);
            if (n == 0)
                break;
            numBytesRead += n;
            numBytesToRead -= n;
        }
        // Set the contents of the .ics file to the MimeContent property.
        appointment.MimeContent = new MimeContent("UTF-8", bytes);
    }
    // This results in a CreateItem call to EWS. 
    appointment.Save(WellKnownFolderName.Calendar);
}
```

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a><span data-ttu-id="39f54-157">Использование веб-служб Exchange для импорта элемента с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="39f54-157">Use EWS to import an item by using the MIME stream</span></span>

<span data-ttu-id="39f54-158">Можно использовать операцию EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) Импорт EML и iCal элементов с помощью своих MIME-поток.</span><span class="sxs-lookup"><span data-stu-id="39f54-158">You can use the [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS operation to import EML and iCal items by using their MIME stream.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
    <t:MailboxCulture>en-US</t:MailboxCulture>
  </soap:Header>
  <soap:Body >
    <m:CreateItem>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </m:SavedItemFolderId> 
        <m:Items>
        <t:Message>
          <t:MimeContent CharacterSet="UTF-8">
            <!-- Insert MIME content here-->
          </t:MimeContent>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="39f54-159">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="39f54-159">Next steps</span></span>
<span data-ttu-id="39f54-160"><a name="bk_importproperties"> </a></span><span class="sxs-lookup"><span data-stu-id="39f54-160"></span></span>

<span data-ttu-id="39f54-161">После импорта элементов в почтовом ящике, может потребоваться [создать настраиваемые папки для хранения импортированных элементов](how-to-work-with-folders-by-using-ews-in-exchange.md)или [синхронизировать элементы вашего клиента и почтового ящика](mailbox-synchronization-and-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="39f54-161">After you import items into a mailbox, you might want to [create a custom folder to store your imported items](how-to-work-with-folders-by-using-ews-in-exchange.md), or [synchronize your client and mailbox items](mailbox-synchronization-and-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="39f54-162">См. также</span><span class="sxs-lookup"><span data-stu-id="39f54-162">See also</span></span>


- [<span data-ttu-id="39f54-163">Экспорт и импорт элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="39f54-163">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="39f54-164">Экспорт элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="39f54-164">Export items by using EWS in Exchange</span></span>](how-to-export-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="39f54-165">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="39f54-165">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="39f54-166">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="39f54-166">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

