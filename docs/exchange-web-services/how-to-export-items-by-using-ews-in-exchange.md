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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455886"
---
# <a name="export-items-by-using-ews-in-exchange"></a>Экспорт элементов с помощью EWS в Exchange

Узнайте, как экспортировать встречи, сообщения электронной почты, контакты, задачи и другие элементы с помощью управляемого API EWS или EWS в Exchange.
  
Вы можете экспортировать элементы из Exchange с помощью управляемого API EWS или EWS несколькими различными способами. Используемый вариант зависит от:
  
- Экспортируемый тип элемента.
    
- Степень точности, которую нужно поддерживать между состоянием элемента в Exchange и экспортированным элементом.
    
- Формат экспортированного элемента.
    
- Требования к завершающей обработке.
    
- Нужно ли импортировать элемент обратно в Exchange.
    
В этой статье показано, как использовать различные параметры для экспорта элементов. Можно использовать любой параметр для пакетного экспорта элементов из Exchange.
  
## <a name="export-an-item-into-a-custom-format"></a>Экспорт элемента в настраиваемый формат
<a name="bk_exportcustom"> </a>

Вы можете использовать результаты [элемента. Bind](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) метод управляемого API EWS или анализ результатов [операции GetItem в](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) формате, который работает с требованиями приложения. Используйте этот параметр при экспорте элементов, чтобы импортировать их в базу данных, CSV-файл или другой формат или систему. Вы также можете сохранить элемент в виде элемента XML EWS, который может быть полезен, так как многие системы имеют возможность синтаксического анализа XML. Рекомендуется использовать метод **Item. Bind** или операция **GetItem** (без свойства [Item. сохранитьmimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) ), так как этот параметр позволяет контролировать экспортируемые свойства. 
  
## <a name="export-items-with-full-fidelity"></a>Экспорт элементов с использованием полной точности
<a name="bk_exportfullfidelity"> </a>

Если вы хотите экспортировать элементы с полным соответствием, вы можете использовать операцию [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) EWS. Операция **ExportItems** экспортирует каждый элемент в виде потока данных. Этот поток данных не предназначен для синтаксического анализа, но его можно использовать в качестве резервной копии на уровне элемента, которая может быть импортирована обратно в почтовый ящик Exchange. В каждый запрос **ExportItems** можно включить множество элементов, хотя при каждом вызове рекомендуется включать не более 100 элементов. Так как управляемый API EWS не реализует операцию **ExportItems** , если вы используете управляемый API EWS, вам потребуется написать процедуру для отправки веб-запросов. При необходимости можно использовать метод [Item. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для получения метаданных элемента, чтобы можно было индексировать и хранить сведения о потоке данных. 
  
Мы рекомендуем использовать операцию **ExportItems** для экспорта элементов, которые планируется импортировать в почтовый ящик Exchange. 
  
В приведенном ниже примере показано, как использовать операцию **ExportItems** . В этом примере идентификатор элемента сокращается для удобочитаемости. 
  
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

Сервер отвечает на запрос **ExportItems** с помощью элемента [експортитемсреспонсе](https://msdn.microsoft.com/library/ef44354b-fbdb-4f7c-b6bd-b27f56a1d018%28Office.15%29.aspx) , который содержит значение элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) с **ошибкой**, что указывает на то, что элемент был успешно экспортирован. Ответ также включает идентификатор элемента экспортируемого элемента и поток данных, который содержит экспортированное содержимое. В следующем примере показан текст SOAP, который содержит экспортированный элемент.
  
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

## <a name="use-the-mime-stream-to-export-into-common-file-formats"></a>Использование потока MIME для экспорта в обычные форматы файлов
<a name="bk_exportfullfidelity"> </a>

Вы можете использовать метод [Item. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для управляемого API или операцию [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для получения представления элемента в формате MIME. Так как в Exchange не хранится MIME-содержимое каждого элемента, он должен преобразовать представление каждого элемента в поток MIME. Так как это преобразование является дорогостоящим, мы не рекомендуем запрашивать MIME-поток для элементов крупного масштаба. Также обратите внимание на то, что поток MIME содержит ограниченный набор свойств; возможно, вам придется рассмотреть другие варианты, если набор свойств не содержит требуемые свойства. 
  
### <a name="use-the-ews-managed-api-to-export-an-email-into-an-eml-and-mht-file-by-using-the-mime-stream"></a>Использование управляемого API EWS для экспорта электронной почты в EML-и MHT-файл с помощью потока MIME
<a name="bk_exportemailmime"> </a>

Outlook и другие общие почтовые приложения могут открывать формат файлов EML (EML). В приведенном ниже примере показано, как можно экспортировать электронную почту с помощью потока MIME и использовать поток MIME для создания файла EML и файла MIME HTML (MHT). Многие веб-браузеры поддерживают формат HTML HTML-файлов. В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь может пройти проверку подлинности на сервере Exchange. 
  
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

### <a name="use-the-ews-managed-api-to-export-an-appointment-into-an-ical-file-by-using-the-mime-stream"></a>Использование управляемого API EWS для экспорта встречи в файл iCal с помощью потока MIME
<a name="bk_exporticalmime"> </a>

Outlook и другие общие приложения календаря могут открывать формат файлов iCal (ICS). В приведенном ниже примере показано, как экспортировать встречу с помощью потока MIME и использовать поток MIME для создания файла в формате iCal. Обратите внимание, что многие свойства не экспортируются вместе с потоком MIME, включая участников и свойства, связанные с вложением. Вы можете записать другие свойства из EWS, запросив их и сохранив в файле iCal в виде частных расширений. Для этих частных добавочных номеров используется префикс "x". 
  
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь может пройти проверку подлинности на сервере Exchange. В этом примере также предполагается, что у вас есть встреча с темой "2015 финансовых проектов" в папке "Календарь". 
  
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

### <a name="use-the-ews-managed-api-to-export-a-contact-into-a-vcard-file-by-using-the-mime-stream"></a>Использование управляемого API EWS для экспорта контакта в файл vCard с помощью потока MIME
<a name="bk_exportvcardmime"> </a>

Outlook и другие общие приложения управления контактами могут открыть формат файла vCard (VCF). В приведенном ниже примере показано, как экспортировать контакт с помощью потока MIME и использовать поток MIME для создания визитной карточки. Вы можете записать другие свойства из EWS, запросив их и сохранив в файле. vCard как личные расширения. Эти расширения имеют префикс "x". 
  
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь может пройти проверку подлинности на сервере Exchange. 
  
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
> Файлы vCard нельзя импортировать с помощью свойства **сохранитьmimecontent** . Вы можете импортировать контакты с помощью [контакта. Сохраните](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.save%28v=exchg.80%29.aspx) метод управляемого API EWS или операцию [CreateItem](https://msdn.microsoft.com/library/417e994b-0a17-4c24-9527-04796b80b029%28Office.15%29.aspx) EWS. 
  
### <a name="use-ews-to-export-any-item-by-using-the-mime-stream"></a>Использование EWS для экспорта любого элемента с помощью потока MIME
<a name="bk_exportewsmime"> </a>

Используйте операцию **GetItem** для получения MIME потока элемента. Следующий запрос **GetItem** показывает, как запросить MIME содержимое элемента. 
  
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

В следующем примере показан ответ на запрос на получение потока MIME. Поток MIME был укорочен для удобочитаемости.
  
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
<a name="bk_exportfullfidelity"> </a>

После экспорта элементов может потребоваться [импортировать их в Exchange](how-to-import-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также


- [Экспорт и импорт элементов с помощью EWS в Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Импорт элементов с помощью EWS в Exchange](how-to-import-items-by-using-ews-in-exchange.md)
    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

