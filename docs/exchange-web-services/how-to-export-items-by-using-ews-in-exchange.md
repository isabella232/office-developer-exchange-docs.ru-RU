---
title: Экспорт элементов с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e93ee68c-e134-4469-9070-fba404d46cb4
description: Узнайте, как экспортировать встречи, сообщения электронной почты, контакты, задачи и других элементов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 65b5b2ef1eba66877d5b6f6c3d4237a26a254196
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761010"
---
# <a name="export-items-by-using-ews-in-exchange"></a><span data-ttu-id="8a8b3-103">Экспорт элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a8b3-103">Export items by using EWS in Exchange</span></span>

<span data-ttu-id="8a8b3-104">Узнайте, как экспортировать встречи, сообщения электронной почты, контакты, задачи и других элементов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-104">Learn how to export appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="8a8b3-105">Элементы можно экспортировать из Exchange с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в несколько различных способов.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-105">You can export items from Exchange by using the EWS Managed API or EWS in a number of different ways.</span></span> <span data-ttu-id="8a8b3-106">Параметр, используемого зависит от:</span><span class="sxs-lookup"><span data-stu-id="8a8b3-106">The option you use depends on:</span></span>
  
- <span data-ttu-id="8a8b3-107">Тип элемента, который экспортируется.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-107">The item type that is exported.</span></span>
    
- <span data-ttu-id="8a8b3-108">Степень качества, который будет поддерживаться между состоянием элемента в Exchange и экспортированный элемент.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-108">The degree of fidelity that you want maintained between the item state in Exchange and the exported item.</span></span>
    
- <span data-ttu-id="8a8b3-109">Формат экспортируемого элемента.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-109">The format of the exported item.</span></span>
    
- <span data-ttu-id="8a8b3-110">Требования последующей обработки.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-110">Any post-processing requirements.</span></span>
    
- <span data-ttu-id="8a8b3-111">Требуется ли импортировать элемент обратно в Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-111">Whether you want to import the item back into Exchange.</span></span>
    
<span data-ttu-id="8a8b3-112">В этой статье показано, как использовать каждый из различных вариантов для экспорта элементов.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-112">This article shows you how to use each of the different options to export items.</span></span> <span data-ttu-id="8a8b3-113">Параметр можно использовать для экспорта элементов из него Exchange пакетной обработки.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-113">You can use any option to batch export items out of Exchange.</span></span>
  
## <a name="export-an-item-into-a-custom-format"></a><span data-ttu-id="8a8b3-114">Экспорт элемента в пользовательском формате</span><span class="sxs-lookup"><span data-stu-id="8a8b3-114">Export an item into a custom format</span></span>
<span data-ttu-id="8a8b3-115"><a name="bk_exportcustom"> </a></span><span class="sxs-lookup"><span data-stu-id="8a8b3-115"></span></span>

<span data-ttu-id="8a8b3-116">Можно использовать результаты для вызова метода [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) управляемый API EWS или проанализировать результаты операции [Getitem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) в формат, который работает с требований приложения.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-116">You can use the results of an [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) EWS Managed API method call or parse the results of a [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) EWS operation into a format that works with your application requirements.</span></span> <span data-ttu-id="8a8b3-117">Используйте этот параметр при экспорте элементов для импорта их в базе данных, CSV-файл или другой формат или системы.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-117">Use this option when you are exporting items in order to import them into a database, .csv file, or another format or system.</span></span> <span data-ttu-id="8a8b3-118">Можно даже сохранения элемента в виде элемента XML веб-служб Exchange, которые могут быть полезны, потому что многие системы имеют возможность анализа XML.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-118">You can even save the item in the form of the item EWS XML, which can be useful because many systems have XML parsing capability.</span></span> <span data-ttu-id="8a8b3-119">Мы рекомендуем использовать метод **Item.Bind** или операции **GetItem** (без свойства [Item.MimeContent](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ), так как этот параметр позволяет управлять свойств, которые требуется экспортировать.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-119">We recommend that you use the **Item.Bind** method or the **GetItem** operation (without the [Item.MimeContent](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property) because this option gives you control over which properties are exported.</span></span> 
  
## <a name="export-items-with-full-fidelity"></a><span data-ttu-id="8a8b3-120">Экспорт элементов с корректном</span><span class="sxs-lookup"><span data-stu-id="8a8b3-120">Export items with full fidelity</span></span>
<span data-ttu-id="8a8b3-121"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="8a8b3-121"></span></span>

<span data-ttu-id="8a8b3-122">Если требуется для экспорта элементов с корректном, можно использовать операцию [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-122">If you want to export items with full fidelity, you can use the [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="8a8b3-123">Операция **ExportItems** экспортирует каждого элемента в виде потока данных.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-123">The **ExportItems** operation exports each item as a data stream.</span></span> <span data-ttu-id="8a8b3-124">Этот поток данных не для синтаксического анализа, но можно использовать в качестве резервного копирования на уровне элементов, который можно импортировать обратно в почтовый ящик Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-124">This data stream is not for parsing, but can be used as an item-level backup that can be imported back into an Exchange mailbox.</span></span> <span data-ttu-id="8a8b3-125">Можно добавить много элементов каждого запроса **ExportItems** , хотя корпорация Майкрософт рекомендует включать не более 100 элементов в каждого вызова.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-125">You can include many items in each **ExportItems** request, although we recommend that you include no more than 100 items in each call.</span></span> <span data-ttu-id="8a8b3-126">Так как управляемый API EWS не реализует операцию **ExportItems** при использовании управляемого интерфейса API веб-служб Exchange, необходимые для написания процедуры для отправки веб-запросов.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-126">Because the EWS Managed API does not implement the **ExportItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> <span data-ttu-id="8a8b3-127">При необходимости можно использовать метод [Item.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для получения метаданных о элементе, чтобы индексировать и хранить сведения о потоке данных.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-127">You can optionally use the [Item.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get metadata about the item so that you can index and store information about the data stream.</span></span> 
  
<span data-ttu-id="8a8b3-128">Рекомендуется использовать операцию **ExportItems** для экспорта элементов, которые планируется импортировать в почтовый ящик Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-128">We recommend that you use the **ExportItems** operation to export items that you plan to import into an Exchange mailbox.</span></span> 
  
<span data-ttu-id="8a8b3-129">Следующем примере показано, как использовать операцию **ExportItems** .</span><span class="sxs-lookup"><span data-stu-id="8a8b3-129">The following example shows how to use the **ExportItems** operation.</span></span> <span data-ttu-id="8a8b3-130">В этом примере идентификатор элемента — это сокращение для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-130">In this example, the item identifier is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013"/>
  </soap:Header>
  <soap:Body>
    <m:ExportItems>
      <m:ItemIds>
        <t:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA="/>
      </m:ItemIds>
    </m:ExportItems>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **ExportItems** с элементом [ExportItemsResponse](http://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) , который содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что элемент был успешно экспортированы. Ответ также включает в себя идентификатор элемента из экспортированного элемента и поток данных, содержащий экспортированное содержимое. <span data-ttu-id="8a8b3-133">В следующем примере показано body SOAP, содержащий экспортированный элемент.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-133">The following example shows the SOAP body that contains the exported item.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:ExportItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
    <m:ResponseMessages>
      <m:ExportItemsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:ItemId Id="AAMkAGYzZjZmRiUsidkC+NAAAAY89GAAA=" ChangeKey="FwAAAA=="/>
        <m:Data>
          AQAAAAgAAAAAAAAALgBlAHgAdABlAHMAdAAuAG0AaQBjAHIAbwBzAG8AZgB0AC4A
          cgAyAEAAYQB1AGoAaQBuAGcALQBkAG8AbQAuAGUAeAB0AGUAcwB0AC4AbQBpAGMAcgBvAHMA
          bwBmAHQALgBjAG8AbQAAAAMAADkAAAAAAwD+DwYAAAADAARAAwACQAMADkA=
        </m:Data>
      </m:ExportItemsResponseMessage>
     </m:ResponseMessages>
  </m:ExportItemsResponse>
</s:Body>
```

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a><span data-ttu-id="8a8b3-134">Использование MIME-поток для экспорта в стандартных форматах файлов</span><span class="sxs-lookup"><span data-stu-id="8a8b3-134">Use the MIME stream to export into common file formats</span></span>
<span data-ttu-id="8a8b3-135"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="8a8b3-135"></span></span>

<span data-ttu-id="8a8b3-136">Можно использовать метод управляемый API EWS [Item.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) или операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) веб-служб Exchange для получения представления MIME элемента.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-136">You can use the [Item.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) EWS Managed API method or the [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get a MIME representation of an item.</span></span> <span data-ttu-id="8a8b3-137">Так как Exchange не сохраняет содержимого MIME каждого элемента, имеет для преобразования представления базы данных для каждого элемента в MIME-поток.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-137">Because Exchange doesn't store the MIME content of each item, it has to convert the database representation of each item into the MIME stream.</span></span> <span data-ttu-id="8a8b3-138">Так как это преобразование обходится дорого, не рекомендуется, чтобы запросить MIME-поток для элементов на большого масштаба.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-138">Because this conversion is costly, we do not recommend that you request the MIME stream for items on a large scale.</span></span> <span data-ttu-id="8a8b3-139">Также Обратите внимание на то, что поток MIME содержит ограниченный набор свойств. может потребоваться другие варианты, если набор свойств не содержит свойства, которые необходимо.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-139">Also note that the MIME stream contains a limited set of properties; you might have to consider other options if the property set doesn't contain the properties you need.</span></span> 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a><span data-ttu-id="8a8b3-140">Использовать управляемый API EWS для экспорта в файл EML с помощью проводника и .mht сообщения электронной почты с помощью MIME-поток</span><span class="sxs-lookup"><span data-stu-id="8a8b3-140">Use the EWS Managed API to export an email into an .eml and .mht file by using the MIME stream</span></span>
<span data-ttu-id="8a8b3-141"><a name="bk_exportemailmime"> </a></span><span class="sxs-lookup"><span data-stu-id="8a8b3-141"></span></span>

<span data-ttu-id="8a8b3-142">Outlook и другие общие приложения электронной почты можно открыть в формате EML (файл).</span><span class="sxs-lookup"><span data-stu-id="8a8b3-142">Outlook and other common email applications can open the EML (.eml) file format.</span></span> <span data-ttu-id="8a8b3-143">Следующий пример показывает, как можно экспортировать сообщение электронной почты с помощью потока MIME и используйте MIME-поток для создания EML и файл MIME HTML (MHT).</span><span class="sxs-lookup"><span data-stu-id="8a8b3-143">The following example shows you how you can export an email by using the MIME stream, and use the MIME stream to create an EML and a MIME HTML (.mht) file.</span></span> <span data-ttu-id="8a8b3-144">Многие веб-браузеры поддерживают формат файлов MIME HTML.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-144">Many web browsers support the MIME HTML file format.</span></span> <span data-ttu-id="8a8b3-145">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и пользователь может выполнять проверку подлинности для Exchange server.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void ExportMIMEEmail(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems(view);
    foreach (var item in results)
    { 
        PropertySet props = new PropertySet(EmailMessageSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = EmailMessage.Bind(service, item.Id, props);
                
        string emlFileName = @"C:\export\email.eml";
        string mhtFileName = @"C:\export\email.mht";
        // Save as .eml.
        using (FileStream fs = new FileStream(emlFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
        // Save as .mht.
        using (FileStream fs = new FileStream(mhtFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="8a8b3-146">Использование управляемого интерфейса API веб-служб Exchange для экспорта встречи в формате iCal-файл с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="8a8b3-146">Use the EWS Managed API to export an appointment into an iCal file by using the MIME stream</span></span>
<span data-ttu-id="8a8b3-147"><a name="bk_exporticalmime"> </a></span><span class="sxs-lookup"><span data-stu-id="8a8b3-147"></span></span>

<span data-ttu-id="8a8b3-148">Outlook и другие общие приложения календаря можно открыть в формате iCal (.ics).</span><span class="sxs-lookup"><span data-stu-id="8a8b3-148">Outlook and other common calendar applications can open the iCal (.ics) file format.</span></span> <span data-ttu-id="8a8b3-149">Следующем примере показано, как экспортировать встречи с помощью потока MIME и использовать MIME-поток для создания файла iCal.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-149">The following example shows you how to export an appointment by using the MIME stream, and use the MIME stream to create an iCal file.</span></span> <span data-ttu-id="8a8b3-150">Обратите внимание, что многие свойства не экспортируются с MIME-поток, включая участников и свойства, связанные с вложением.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-150">Note that many properties are not exported with the MIME stream, including attendees and attachment-related properties.</span></span> <span data-ttu-id="8a8b3-151">Вы можете захватить другие свойства из веб-служб Exchange и сохранение их в файле iCal как закрытый расширения.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-151">You can capture other properties from EWS by requesting them and saving them in the iCal file as private extensions.</span></span> <span data-ttu-id="8a8b3-152">Закрытый файлы с этим расширением начинаются с «x-».</span><span class="sxs-lookup"><span data-stu-id="8a8b3-152">These private extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="8a8b3-153">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и пользователь может выполнять проверку подлинности для Exchange server.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-153">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> <span data-ttu-id="8a8b3-154">В этом примере также предполагается, что имеется встречи с темой «2015 финансовые проекции» в папке календаря.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-154">This example also assumes that you have an appointment with the subject "2015 Financial Projections" in the calendar folder.</span></span> 
  
```cs
private static void ExportMIMEAppointment(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Calendar);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly); 
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems("subject:'2015 Financial Projections'", view);
    foreach (var item in results)
    {
        PropertySet props = new PropertySet(AppointmentSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = Appointment.Bind(service, item.Id, props);
        string iCalFileName = @"C:\export\appointment.ics";
        // Save as .ics.
        using (FileStream fs = new FileStream(iCalFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a><span data-ttu-id="8a8b3-155">Использовать управляемый API EWS для экспорта в файл визитной карточки контакта с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="8a8b3-155">Use the EWS Managed API to export a contact into a vCard file by using the MIME stream</span></span>
<span data-ttu-id="8a8b3-156"><a name="bk_exportvcardmime"> </a></span><span class="sxs-lookup"><span data-stu-id="8a8b3-156"></span></span>

<span data-ttu-id="8a8b3-157">Outlook и другие общие приложения управления контактами можно открыть файл формата vCard (.vcf).</span><span class="sxs-lookup"><span data-stu-id="8a8b3-157">Outlook and other common contact management applications can open the vCard (.vcf) file format.</span></span> <span data-ttu-id="8a8b3-158">Следующем примере показано, как экспортировать контакта с помощью потока MIME и использовать MIME-поток для создания визитной карточки.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-158">The following example shows you how to export a contact by using the MIME stream, and use the MIME stream to create a vCard.</span></span> <span data-ttu-id="8a8b3-159">Вы можете захватить и сохранение их в другие свойства из веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-159">You can capture other properties from EWS by requesting them and saving them in the .</span></span> <span data-ttu-id="8a8b3-160">vCard как закрытый расширения.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-160">vCard as private extensions.</span></span> <span data-ttu-id="8a8b3-161">Файлы с этим расширением начинаются с «x-».</span><span class="sxs-lookup"><span data-stu-id="8a8b3-161">These extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="8a8b3-162">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и пользователь может выполнять проверку подлинности для Exchange server.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-162">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
```cs
private static void ExportMIMEContact(ExchangeService service)
{
    Folder inbox = Folder.Bind(service, WellKnownFolderName.Contacts);
    ItemView view = new ItemView(1);
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly);
    // This results in a FindItem call to EWS.
    FindItemsResults<Item> results = inbox.FindItems(view);
    foreach (var item in results)
    {
        PropertySet props = new PropertySet(ContactSchema.MimeContent);
        // This results in a GetItem call to EWS.
        var email = Contact.Bind(service, item.Id, props);
        string vcfFileName = @"C:\export\contact.vcf";
        // Save as .vcf.
        using (FileStream fs = new FileStream(vcfFileName, FileMode.Create, FileAccess.Write))
        {
            fs.Write(email.MimeContent.Content, 0, email.MimeContent.Content.Length);
        }
    }
}
```

> [!NOTE]
> <span data-ttu-id="8a8b3-163">С помощью свойства **MimeContent** нельзя импортировать файлы vCard.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-163">You cannot import vCard files by using the **MimeContent** property.</span></span> <span data-ttu-id="8a8b3-164">Контакты можно импортировать с помощью метода управляемый API EWS [Contact.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) или операции [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-164">You can import contacts by using the [Contact.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS operation.</span></span> 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a><span data-ttu-id="8a8b3-165">Использование веб-служб Exchange для экспорта любого элемента с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="8a8b3-165">Use EWS to export any item by using the MIME stream</span></span>
<span data-ttu-id="8a8b3-166"><a name="bk_exportewsmime"> </a></span><span class="sxs-lookup"><span data-stu-id="8a8b3-166"></span></span>

<span data-ttu-id="8a8b3-167">Чтобы получить MIME-поток элемента с помощью операции **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="8a8b3-167">Use the **GetItem** operation to get the MIME stream of an item.</span></span> <span data-ttu-id="8a8b3-168">Следующий запрос **GetItem** показано, как для запроса контента MIME элемента.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-168">The following **GetItem** request shows how to request the MIME content of an item.</span></span> 
  
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
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADEzYjJkLTYxMwB8GqYicWAAA=" ChangeKey="CQAAABzXv"/>
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="8a8b3-169">В следующем примере показано ответ на запрос для получения MIME-поток.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-169">The following example shows the response to a request to get the MIME stream.</span></span> <span data-ttu-id="8a8b3-170">MIME-поток был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="8a8b3-170">The MIME stream has been shortened for readability.</span></span>
  
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
              <t:MimeContent CharacterSet="UTF-8">UmVjZ6IGZyb2b2suY29y5hMzgwZTA1YtDQo=</t:MimeContent>
              <t:ItemId Id="AAMkADEzYjJkLTYxMwB8GqYicWAAA=" ChangeKey="CQAAABzXv"/>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

## 
<span data-ttu-id="8a8b3-171"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="8a8b3-171"></span></span>

<span data-ttu-id="8a8b3-172">После экспорта элементов, можно [импортировать в Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="8a8b3-172">After exporting items, you might want to [import items into Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8a8b3-173">См. также</span><span class="sxs-lookup"><span data-stu-id="8a8b3-173">See also</span></span>


- [<span data-ttu-id="8a8b3-174">Экспорт и импорт элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a8b3-174">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="8a8b3-175">Импорт элементов с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8a8b3-175">Import items by using EWS in Exchange</span></span>](how-to-import-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="8a8b3-176">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="8a8b3-176">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="8a8b3-177">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="8a8b3-177">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

