---
title: Экспорт элементов с помощью EWS в Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.assetid: e93ee68c-e134-4469-9070-fba404d46cb4
description: Узнайте, как экспортировать встречи, сообщения электронной почты, контакты, задачи и другие элементы с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: a01c9487821958b06ec162f2aee27e2d2804eaaf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455886"
---
# <a name="export-items-by-using-ews-in-exchange"></a><span data-ttu-id="77b57-103">Экспорт элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="77b57-103">Export items by using EWS in Exchange</span></span>

<span data-ttu-id="77b57-104">Узнайте, как экспортировать встречи, сообщения электронной почты, контакты, задачи и другие элементы с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b57-104">Learn how to export appointments, emails, contacts, tasks, and other items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="77b57-105">Вы можете экспортировать элементы из Exchange с помощью управляемого API EWS или EWS несколькими различными способами.</span><span class="sxs-lookup"><span data-stu-id="77b57-105">You can export items from Exchange by using the EWS Managed API or EWS in a number of different ways.</span></span> <span data-ttu-id="77b57-106">Используемый вариант зависит от:</span><span class="sxs-lookup"><span data-stu-id="77b57-106">The option you use depends on:</span></span>
  
- <span data-ttu-id="77b57-107">Экспортируемый тип элемента.</span><span class="sxs-lookup"><span data-stu-id="77b57-107">The item type that is exported.</span></span>
    
- <span data-ttu-id="77b57-108">Степень точности, которую нужно поддерживать между состоянием элемента в Exchange и экспортированным элементом.</span><span class="sxs-lookup"><span data-stu-id="77b57-108">The degree of fidelity that you want maintained between the item state in Exchange and the exported item.</span></span>
    
- <span data-ttu-id="77b57-109">Формат экспортированного элемента.</span><span class="sxs-lookup"><span data-stu-id="77b57-109">The format of the exported item.</span></span>
    
- <span data-ttu-id="77b57-110">Требования к завершающей обработке.</span><span class="sxs-lookup"><span data-stu-id="77b57-110">Any post-processing requirements.</span></span>
    
- <span data-ttu-id="77b57-111">Нужно ли импортировать элемент обратно в Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b57-111">Whether you want to import the item back into Exchange.</span></span>
    
<span data-ttu-id="77b57-112">В этой статье показано, как использовать различные параметры для экспорта элементов.</span><span class="sxs-lookup"><span data-stu-id="77b57-112">This article shows you how to use each of the different options to export items.</span></span> <span data-ttu-id="77b57-113">Можно использовать любой параметр для пакетного экспорта элементов из Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b57-113">You can use any option to batch export items out of Exchange.</span></span>
  
## <a name="export-an-item-into-a-custom-format"></a><span data-ttu-id="77b57-114">Экспорт элемента в настраиваемый формат</span><span class="sxs-lookup"><span data-stu-id="77b57-114">Export an item into a custom format</span></span>
<span data-ttu-id="77b57-115"><a name="bk_exportcustom"> </a></span><span class="sxs-lookup"><span data-stu-id="77b57-115"><a name="bk_exportcustom"> </a></span></span>

<span data-ttu-id="77b57-116">Вы можете использовать результаты [элемента. Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) метод управляемого API EWS или анализ результатов [операции GetItem в](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) формате, который работает с требованиями приложения.</span><span class="sxs-lookup"><span data-stu-id="77b57-116">You can use the results of an [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) EWS Managed API method call or parse the results of a [GetItem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) EWS operation into a format that works with your application requirements.</span></span> <span data-ttu-id="77b57-117">Используйте этот параметр при экспорте элементов, чтобы импортировать их в базу данных, CSV-файл или другой формат или систему.</span><span class="sxs-lookup"><span data-stu-id="77b57-117">Use this option when you are exporting items in order to import them into a database, .csv file, or another format or system.</span></span> <span data-ttu-id="77b57-118">Вы также можете сохранить элемент в виде элемента XML EWS, который может быть полезен, так как многие системы имеют возможность синтаксического анализа XML.</span><span class="sxs-lookup"><span data-stu-id="77b57-118">You can even save the item in the form of the item EWS XML, which can be useful because many systems have XML parsing capability.</span></span> <span data-ttu-id="77b57-119">Рекомендуется использовать метод **Item. Bind** или операция **GetItem** (без свойства [Item. сохранитьmimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ), так как этот параметр позволяет контролировать экспортируемые свойства.</span><span class="sxs-lookup"><span data-stu-id="77b57-119">We recommend that you use the **Item.Bind** method or the **GetItem** operation (without the [Item.MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property) because this option gives you control over which properties are exported.</span></span> 
  
## <a name="export-items-with-full-fidelity"></a><span data-ttu-id="77b57-120">Экспорт элементов с использованием полной точности</span><span class="sxs-lookup"><span data-stu-id="77b57-120">Export items with full fidelity</span></span>
<span data-ttu-id="77b57-121"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="77b57-121"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="77b57-122">Если вы хотите экспортировать элементы с полным соответствием, вы можете использовать операцию [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="77b57-122">If you want to export items with full fidelity, you can use the [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="77b57-123">Операция **ExportItems** экспортирует каждый элемент в виде потока данных.</span><span class="sxs-lookup"><span data-stu-id="77b57-123">The **ExportItems** operation exports each item as a data stream.</span></span> <span data-ttu-id="77b57-124">Этот поток данных не предназначен для синтаксического анализа, но его можно использовать в качестве резервной копии на уровне элемента, которая может быть импортирована обратно в почтовый ящик Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b57-124">This data stream is not for parsing, but can be used as an item-level backup that can be imported back into an Exchange mailbox.</span></span> <span data-ttu-id="77b57-125">В каждый запрос **ExportItems** можно включить множество элементов, хотя при каждом вызове рекомендуется включать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="77b57-125">You can include many items in each **ExportItems** request, although we recommend that you include no more than 100 items in each call.</span></span> <span data-ttu-id="77b57-126">Так как управляемый API EWS не реализует операцию **ExportItems** , если вы используете управляемый API EWS, вам потребуется написать процедуру для отправки веб-запросов.</span><span class="sxs-lookup"><span data-stu-id="77b57-126">Because the EWS Managed API does not implement the **ExportItems** operation, if you use the EWS Managed API, you'll need to write a routine to send the web requests.</span></span> <span data-ttu-id="77b57-127">При необходимости можно использовать метод [Item. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для получения метаданных элемента, чтобы можно было индексировать и хранить сведения о потоке данных.</span><span class="sxs-lookup"><span data-stu-id="77b57-127">You can optionally use the [Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) method to get metadata about the item so that you can index and store information about the data stream.</span></span> 
  
<span data-ttu-id="77b57-128">Мы рекомендуем использовать операцию **ExportItems** для экспорта элементов, которые планируется импортировать в почтовый ящик Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b57-128">We recommend that you use the **ExportItems** operation to export items that you plan to import into an Exchange mailbox.</span></span> 
  
<span data-ttu-id="77b57-129">В приведенном ниже примере показано, как использовать операцию **ExportItems** .</span><span class="sxs-lookup"><span data-stu-id="77b57-129">The following example shows how to use the **ExportItems** operation.</span></span> <span data-ttu-id="77b57-130">В этом примере идентификатор элемента сокращается для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="77b57-130">In this example, the item identifier is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Сервер отвечает на запрос **ExportItems** с помощью элемента [експортитемсреспонсе](https://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) , который содержит значение элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) с **ошибкой**, что указывает на то, что элемент был успешно экспортирован. Ответ также включает идентификатор элемента экспортируемого элемента и поток данных, который содержит экспортированное содержимое. <span data-ttu-id="77b57-133">В следующем примере показан текст SOAP, который содержит экспортированный элемент.</span><span class="sxs-lookup"><span data-stu-id="77b57-133">The following example shows the SOAP body that contains the exported item.</span></span>
  
```XML
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
        xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <m:ExportItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a><span data-ttu-id="77b57-134">Использование потока MIME для экспорта в обычные форматы файлов</span><span class="sxs-lookup"><span data-stu-id="77b57-134">Use the MIME stream to export into common file formats</span></span>
<span data-ttu-id="77b57-135"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="77b57-135"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="77b57-136">Вы можете использовать метод [Item. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для управляемого API или операцию [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для получения представления элемента в формате MIME.</span><span class="sxs-lookup"><span data-stu-id="77b57-136">You can use the [Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) EWS Managed API method or the [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) EWS operation to get a MIME representation of an item.</span></span> <span data-ttu-id="77b57-137">Так как в Exchange не хранится MIME-содержимое каждого элемента, он должен преобразовать представление каждого элемента в поток MIME.</span><span class="sxs-lookup"><span data-stu-id="77b57-137">Because Exchange doesn't store the MIME content of each item, it has to convert the database representation of each item into the MIME stream.</span></span> <span data-ttu-id="77b57-138">Так как это преобразование является дорогостоящим, мы не рекомендуем запрашивать MIME-поток для элементов крупного масштаба.</span><span class="sxs-lookup"><span data-stu-id="77b57-138">Because this conversion is costly, we do not recommend that you request the MIME stream for items on a large scale.</span></span> <span data-ttu-id="77b57-139">Также обратите внимание на то, что поток MIME содержит ограниченный набор свойств; возможно, вам придется рассмотреть другие варианты, если набор свойств не содержит требуемые свойства.</span><span class="sxs-lookup"><span data-stu-id="77b57-139">Also note that the MIME stream contains a limited set of properties; you might have to consider other options if the property set doesn't contain the properties you need.</span></span> 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a><span data-ttu-id="77b57-140">Использование управляемого API EWS для экспорта электронной почты в EML-и MHT-файл с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="77b57-140">Use the EWS Managed API to export an email into an .eml and .mht file by using the MIME stream</span></span>
<span data-ttu-id="77b57-141"><a name="bk_exportemailmime"> </a></span><span class="sxs-lookup"><span data-stu-id="77b57-141"><a name="bk_exportemailmime"> </a></span></span>

<span data-ttu-id="77b57-142">Outlook и другие общие почтовые приложения могут открывать формат файлов EML (EML).</span><span class="sxs-lookup"><span data-stu-id="77b57-142">Outlook and other common email applications can open the EML (.eml) file format.</span></span> <span data-ttu-id="77b57-143">В приведенном ниже примере показано, как можно экспортировать электронную почту с помощью потока MIME и использовать поток MIME для создания файла EML и файла MIME HTML (MHT).</span><span class="sxs-lookup"><span data-stu-id="77b57-143">The following example shows you how you can export an email by using the MIME stream, and use the MIME stream to create an EML and a MIME HTML (.mht) file.</span></span> <span data-ttu-id="77b57-144">Многие веб-браузеры поддерживают формат HTML HTML-файлов.</span><span class="sxs-lookup"><span data-stu-id="77b57-144">Many web browsers support the MIME HTML file format.</span></span> <span data-ttu-id="77b57-145">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь может пройти проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b57-145">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a><span data-ttu-id="77b57-146">Использование управляемого API EWS для экспорта встречи в файл iCal с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="77b57-146">Use the EWS Managed API to export an appointment into an iCal file by using the MIME stream</span></span>
<span data-ttu-id="77b57-147"><a name="bk_exporticalmime"> </a></span><span class="sxs-lookup"><span data-stu-id="77b57-147"><a name="bk_exporticalmime"> </a></span></span>

<span data-ttu-id="77b57-148">Outlook и другие общие приложения календаря могут открывать формат файлов iCal (ICS).</span><span class="sxs-lookup"><span data-stu-id="77b57-148">Outlook and other common calendar applications can open the iCal (.ics) file format.</span></span> <span data-ttu-id="77b57-149">В приведенном ниже примере показано, как экспортировать встречу с помощью потока MIME и использовать поток MIME для создания файла в формате iCal.</span><span class="sxs-lookup"><span data-stu-id="77b57-149">The following example shows you how to export an appointment by using the MIME stream, and use the MIME stream to create an iCal file.</span></span> <span data-ttu-id="77b57-150">Обратите внимание, что многие свойства не экспортируются вместе с потоком MIME, включая участников и свойства, связанные с вложением.</span><span class="sxs-lookup"><span data-stu-id="77b57-150">Note that many properties are not exported with the MIME stream, including attendees and attachment-related properties.</span></span> <span data-ttu-id="77b57-151">Вы можете записать другие свойства из EWS, запросив их и сохранив в файле iCal в виде частных расширений.</span><span class="sxs-lookup"><span data-stu-id="77b57-151">You can capture other properties from EWS by requesting them and saving them in the iCal file as private extensions.</span></span> <span data-ttu-id="77b57-152">Для этих частных добавочных номеров используется префикс "x".</span><span class="sxs-lookup"><span data-stu-id="77b57-152">These private extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="77b57-153">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь может пройти проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b57-153">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> <span data-ttu-id="77b57-154">В этом примере также предполагается, что у вас есть встреча с темой "2015 финансовых проектов" в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="77b57-154">This example also assumes that you have an appointment with the subject "2015 Financial Projections" in the calendar folder.</span></span> 
  
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

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a><span data-ttu-id="77b57-155">Использование управляемого API EWS для экспорта контакта в файл vCard с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="77b57-155">Use the EWS Managed API to export a contact into a vCard file by using the MIME stream</span></span>
<span data-ttu-id="77b57-156"><a name="bk_exportvcardmime"> </a></span><span class="sxs-lookup"><span data-stu-id="77b57-156"><a name="bk_exportvcardmime"> </a></span></span>

<span data-ttu-id="77b57-157">Outlook и другие общие приложения управления контактами могут открыть формат файла vCard (VCF).</span><span class="sxs-lookup"><span data-stu-id="77b57-157">Outlook and other common contact management applications can open the vCard (.vcf) file format.</span></span> <span data-ttu-id="77b57-158">В приведенном ниже примере показано, как экспортировать контакт с помощью потока MIME и использовать поток MIME для создания визитной карточки.</span><span class="sxs-lookup"><span data-stu-id="77b57-158">The following example shows you how to export a contact by using the MIME stream, and use the MIME stream to create a vCard.</span></span> <span data-ttu-id="77b57-159">Вы можете записать другие свойства из EWS, запросив их и сохранив в файле.</span><span class="sxs-lookup"><span data-stu-id="77b57-159">You can capture other properties from EWS by requesting them and saving them in the .</span></span> <span data-ttu-id="77b57-160">vCard как личные расширения.</span><span class="sxs-lookup"><span data-stu-id="77b57-160">vCard as private extensions.</span></span> <span data-ttu-id="77b57-161">Эти расширения имеют префикс "x".</span><span class="sxs-lookup"><span data-stu-id="77b57-161">These extensions are prefixed with "x-".</span></span> 
  
<span data-ttu-id="77b57-162">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь может пройти проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="77b57-162">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that the user can authenticate to an Exchange server.</span></span> 
  
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
> <span data-ttu-id="77b57-163">Файлы vCard нельзя импортировать с помощью свойства **сохранитьmimecontent** .</span><span class="sxs-lookup"><span data-stu-id="77b57-163">You cannot import vCard files by using the **MimeContent** property.</span></span> <span data-ttu-id="77b57-164">Вы можете импортировать контакты с помощью [контакта. Сохраните](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) метод управляемого API EWS или операцию [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="77b57-164">You can import contacts by using the [Contact.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) EWS Managed API method or the [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS operation.</span></span> 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a><span data-ttu-id="77b57-165">Использование EWS для экспорта любого элемента с помощью потока MIME</span><span class="sxs-lookup"><span data-stu-id="77b57-165">Use EWS to export any item by using the MIME stream</span></span>
<span data-ttu-id="77b57-166"><a name="bk_exportewsmime"> </a></span><span class="sxs-lookup"><span data-stu-id="77b57-166"><a name="bk_exportewsmime"> </a></span></span>

<span data-ttu-id="77b57-167">Используйте операцию **GetItem** для получения MIME потока элемента.</span><span class="sxs-lookup"><span data-stu-id="77b57-167">Use the **GetItem** operation to get the MIME stream of an item.</span></span> <span data-ttu-id="77b57-168">Следующий запрос **GetItem** показывает, как запросить MIME содержимое элемента.</span><span class="sxs-lookup"><span data-stu-id="77b57-168">The following **GetItem** request shows how to request the MIME content of an item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="77b57-169">В следующем примере показан ответ на запрос на получение потока MIME.</span><span class="sxs-lookup"><span data-stu-id="77b57-169">The following example shows the response to a request to get the MIME stream.</span></span> <span data-ttu-id="77b57-170">Поток MIME был укорочен для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="77b57-170">The MIME stream has been shortened for readability.</span></span>
  
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
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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
<span data-ttu-id="77b57-171"><a name="bk_exportfullfidelity"> </a></span><span class="sxs-lookup"><span data-stu-id="77b57-171"><a name="bk_exportfullfidelity"> </a></span></span>

<span data-ttu-id="77b57-172">После экспорта элементов может потребоваться [импортировать их в Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="77b57-172">After exporting items, you might want to [import items into Exchange](how-to-import-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="77b57-173">См. также</span><span class="sxs-lookup"><span data-stu-id="77b57-173">See also</span></span>


- [<span data-ttu-id="77b57-174">Экспорт и импорт элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="77b57-174">Exporting and importing items by using EWS in Exchange</span></span>](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="77b57-175">Импорт элементов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="77b57-175">Import items by using EWS in Exchange</span></span>](how-to-import-items-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="77b57-176">Папки и элементы в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="77b57-176">Folders and items in EWS in Exchange</span></span>](folders-and-items-in-ews-in-exchange.md)
    
- [<span data-ttu-id="77b57-177">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="77b57-177">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

