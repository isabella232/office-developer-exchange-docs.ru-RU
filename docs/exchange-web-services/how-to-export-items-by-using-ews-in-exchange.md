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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761010"
---
# <a name="export-items-by-using-ews-in-exchange"></a>Экспорт элементов с помощью веб-служб Exchange в Exchange

Узнайте, как экспортировать встречи, сообщения электронной почты, контакты, задачи и других элементов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Элементы можно экспортировать из Exchange с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в несколько различных способов. Параметр, используемого зависит от:
  
- Тип элемента, который экспортируется.
    
- Степень качества, который будет поддерживаться между состоянием элемента в Exchange и экспортированный элемент.
    
- Формат экспортируемого элемента.
    
- Требования последующей обработки.
    
- Требуется ли импортировать элемент обратно в Exchange.
    
В этой статье показано, как использовать каждый из различных вариантов для экспорта элементов. Параметр можно использовать для экспорта элементов из него Exchange пакетной обработки.
  
## <a name="export-an-item-into-a-custom-format"></a>Экспорт элемента в пользовательском формате
<a name="bk_exportcustom"> </a>

Можно использовать результаты для вызова метода [Item.Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) управляемый API EWS или проанализировать результаты операции [Getitem](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) в формат, который работает с требований приложения. Используйте этот параметр при экспорте элементов для импорта их в базе данных, CSV-файл или другой формат или системы. Можно даже сохранения элемента в виде элемента XML веб-служб Exchange, которые могут быть полезны, потому что многие системы имеют возможность анализа XML. Мы рекомендуем использовать метод **Item.Bind** или операции **GetItem** (без свойства [Item.MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ), так как этот параметр позволяет управлять свойств, которые требуется экспортировать. 
  
## <a name="export-items-with-full-fidelity"></a>Экспорт элементов с корректном
<a name="bk_exportfullfidelity"> </a>

Если требуется для экспорта элементов с корректном, можно использовать операцию [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) веб-служб Exchange. Операция **ExportItems** экспортирует каждого элемента в виде потока данных. Этот поток данных не для синтаксического анализа, но можно использовать в качестве резервного копирования на уровне элементов, который можно импортировать обратно в почтовый ящик Exchange. Можно добавить много элементов каждого запроса **ExportItems** , хотя корпорация Майкрософт рекомендует включать не более 100 элементов в каждого вызова. Так как управляемый API EWS не реализует операцию **ExportItems** при использовании управляемого интерфейса API веб-служб Exchange, необходимые для написания процедуры для отправки веб-запросов. При необходимости можно использовать метод [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для получения метаданных о элементе, чтобы индексировать и хранить сведения о потоке данных. 
  
Рекомендуется использовать операцию **ExportItems** для экспорта элементов, которые планируется импортировать в почтовый ящик Exchange. 
  
Следующем примере показано, как использовать операцию **ExportItems** . В этом примере идентификатор элемента — это сокращение для удобства чтения. 
  
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

Сервер отвечает на запрос **ExportItems** с элементом [ExportItemsResponse](http://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) , который содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что элемент был успешно экспортированы. Ответ также включает в себя идентификатор элемента из экспортированного элемента и поток данных, содержащий экспортированное содержимое. В следующем примере показано body SOAP, содержащий экспортированный элемент.
  
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a>Использование MIME-поток для экспорта в стандартных форматах файлов
<a name="bk_exportfullfidelity"> </a>

Можно использовать метод управляемый API EWS [Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) или операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) веб-служб Exchange для получения представления MIME элемента. Так как Exchange не сохраняет содержимого MIME каждого элемента, имеет для преобразования представления базы данных для каждого элемента в MIME-поток. Так как это преобразование обходится дорого, не рекомендуется, чтобы запросить MIME-поток для элементов на большого масштаба. Также Обратите внимание на то, что поток MIME содержит ограниченный набор свойств. может потребоваться другие варианты, если набор свойств не содержит свойства, которые необходимо. 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a>Использовать управляемый API EWS для экспорта в файл EML с помощью проводника и .mht сообщения электронной почты с помощью MIME-поток
<a name="bk_exportemailmime"> </a>

Outlook и другие общие приложения электронной почты можно открыть в формате EML (файл). Следующий пример показывает, как можно экспортировать сообщение электронной почты с помощью потока MIME и используйте MIME-поток для создания EML и файл MIME HTML (MHT). Многие веб-браузеры поддерживают формат файлов MIME HTML. В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и пользователь может выполнять проверку подлинности для Exchange server. 
  
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

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a>Использование управляемого интерфейса API веб-служб Exchange для экспорта встречи в формате iCal-файл с помощью потока MIME
<a name="bk_exporticalmime"> </a>

Outlook и другие общие приложения календаря можно открыть в формате iCal (.ics). Следующем примере показано, как экспортировать встречи с помощью потока MIME и использовать MIME-поток для создания файла iCal. Обратите внимание, что многие свойства не экспортируются с MIME-поток, включая участников и свойства, связанные с вложением. Вы можете захватить другие свойства из веб-служб Exchange и сохранение их в файле iCal как закрытый расширения. Закрытый файлы с этим расширением начинаются с «x-». 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и пользователь может выполнять проверку подлинности для Exchange server. В этом примере также предполагается, что имеется встречи с темой «2015 финансовые проекции» в папке календаря. 
  
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

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a>Использовать управляемый API EWS для экспорта в файл визитной карточки контакта с помощью потока MIME
<a name="bk_exportvcardmime"> </a>

Outlook и другие общие приложения управления контактами можно открыть файл формата vCard (.vcf). Следующем примере показано, как экспортировать контакта с помощью потока MIME и использовать MIME-поток для создания визитной карточки. Вы можете захватить и сохранение их в другие свойства из веб-служб Exchange. vCard как закрытый расширения. Файлы с этим расширением начинаются с «x-». 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и пользователь может выполнять проверку подлинности для Exchange server. 
  
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
> С помощью свойства **MimeContent** нельзя импортировать файлы vCard. Контакты можно импортировать с помощью метода управляемый API EWS [Contact.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) или операции [CreateItem](http://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) веб-служб Exchange. 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a>Использование веб-служб Exchange для экспорта любого элемента с помощью потока MIME
<a name="bk_exportewsmime"> </a>

Чтобы получить MIME-поток элемента с помощью операции **GetItem** . Следующий запрос **GetItem** показано, как для запроса контента MIME элемента. 
  
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

В следующем примере показано ответ на запрос для получения MIME-поток. MIME-поток был усечен для удобства чтения.
  
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
<a name="bk_exportfullfidelity"> </a>

После экспорта элементов, можно [импортировать в Exchange](how-to-import-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также


- [Экспорт и импорт элементов с помощью веб-служб Exchange в Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Импорт элементов с помощью веб-служб Exchange в Exchange](how-to-import-items-by-using-ews-in-exchange.md)
    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

