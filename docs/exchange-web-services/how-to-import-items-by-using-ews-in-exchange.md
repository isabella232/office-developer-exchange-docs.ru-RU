---
title: Импорт элементов с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: dd3d3221-c98e-4fa0-81f0-77f733d2f432
description: Узнайте, как импортировать встречи, сообщения электронной почты, контакты, задачи и другие элементы с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: bc874c667c31beb4e59a305626247488cb1a1781
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527987"
---
# <a name="import-items-by-using-ews-in-exchange"></a>Импорт элементов с помощью EWS в Exchange

Узнайте, как импортировать встречи, сообщения электронной почты, контакты, задачи и другие элементы с помощью управляемого API EWS или EWS в Exchange.
  
Многие системы содержат встречи, сообщения электронной почты, контакты и задачи, а также могут импортировать эти элементы в Exchange несколькими различными способами. Импорт элементов в Exchange выполняется просто, если для этих элементов не поддерживаются отношения почтовых ящиков. Для создания элементов в почтовом ящике Exchange можно использовать метод [Item. Save](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) управляемый API EWS или операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS. Простой подход не поддерживает все сценарии, однако. Например: 
  
- Вы не можете поддерживать связь между организаторов и участниками при импорте встреч с участниками (собраниями). Это означает, что организатору собрания потребуется повторить отправку приглашений на собрания для участников, чтобы установить связь между организатором и участниками. Если встреча была импортирована в календарь участника, встреча не будет связана с встречей организатора собрания. Участникам необходимо принять приглашение на собрание, отправленное из организатора, чтобы восстановить связь с организатором.
    
- Сведения о уполномоченные не сохраняются при импорте назначенных задач.
    
Все параметры импорта можно использовать для пакетного импорта элементов в Exchange.
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a>Использование управляемого API EWS или типов элементов EWS для импорта элемента
<a name="bk_importproperties"> </a>

Вы можете использовать управляемый API EWS или EWS для импорта электронных сообщений, контактов, встреч или задач из других систем. Просто присвойте [свойствам](properties-and-extended-properties-in-ews-in-exchange.md) исходного формата любой из следующих объектов в зависимости от того, что вы импортируете. 
  
**Таблица 1. Объекты управляемого API EWS и элементы EWS**

|**Объект управляемого API EWS**|**Элемент EWS**|
|:-----|:-----|
|[EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Сообщение](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[контакт](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx); <br/> |[контакт](https://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx); <br/> |
|[Встреча](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[календаритем](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Task](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Task](https://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Используйте метод [Item. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) Managed API или операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS для выполнения импорта элементов. Этот подход рекомендуется при импорте элементов из других систем, так как вы контролируете, какие свойства будут импортированы. Дополнительные сведения о том, как задать свойства элементов и затем сохранить элемент, можно узнать в статье [Создание элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) или [Создание элемента с помощью EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).
  
## <a name="import-items-with-full-fidelity"></a>Импорт элементов с полными качествами
<a name="bk_importproperties"> </a>

Вы можете использовать операцию [UploadItems](https://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) EWS для отправки элемента в качестве потока данных. Это представление потока данных элемента должно поступать из результатов вызова операции [ExportItems](https://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) . Так как управляемый API EWS не реализует операцию **UploadItems** , если вы используете управляемый API EWS, вам потребуется написать процедуру для отправки веб-запросов. 
  
Это самый простой способ импортировать элементы, экспортированные с другого сервера Exchange Server.
  
В следующем примере идентификаторы и содержимое элемента **данных** сокращаются для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
      xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Сервер отвечает на запрос **UploadItems** с помощью элемента [уплоадитемсреспонсе](https://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) , который содержит значение элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) с **ошибкой**, что указывает на то, что элемент был успешно отправлен. Ответ также включает идентификатор элемента отправленного элемента. 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a>Использование потока MIME для импорта из распространенных форматов файлов
<a name="bk_importproperties"> </a>

В веб-службах EWS можно импортировать файлы EML (EML) и iCal (ICS). Вы хотите протестировать содержимое MIME, чтобы увидеть, как средство синтаксического анализа MIME Exchange обрабатывает содержимое потока MIME. Хотя использование потока MIME удобно, [для импорта элемента лучше использовать управляемый API EWS или типы элементов EWS](#bk_importproperties). Ниже приведен пример [импорта визитной карточки](https://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a>Использование управляемого API EWS для импорта электронной почты из EML-файла с помощью потока MIME

В приведенном ниже примере показано, как задать свойство [сохранитьmimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) с содержимым файла EML и затем импортировать его в почтовый ящик. В этом примере также показано, как задать расширенное свойство [PidTagMessageFlags (0x0E07)](https://msdn.microsoft.com/library/office/cc839733%28v=office.15%29.aspx) для импортированного электронного сообщения, чтобы оно не отображалось в почтовом ящике как элемент черновика. В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь может пройти проверку подлинности на сервере Exchange. 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a>Использование управляемого API EWS для импорта встречи из файла iCal с помощью потока MIME

Вы можете импортировать простые встречи в виде файлов iCalendar с помощью потока MIME. Вы не можете импортировать собрания, которые являются встречами с участниками, так как отношение между собраниями организаторов и участниками должно быть задано в составе рабочего процесса [календаря Exchange](calendars-and-ews-in-exchange.md) . Участники не могут быть захвачены в потоке MIME. 
  
В приведенном ниже примере кода показано, как импортировать простой файл ICS в почтовый ящик пользователя.
  
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

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a>Использование EWS для импорта элемента с помощью потока MIME

Вы можете использовать операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) EWS для импорта элементов EML и iCal с помощью потока MIME. 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_importproperties"> </a>

После импорта элементов в почтовый ящик может потребоваться [создать настраиваемую папку для хранения импортируемых элементов](how-to-work-with-folders-by-using-ews-in-exchange.md)или [синхронизировать элементы клиента и почтового ящика](mailbox-synchronization-and-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также


- [Экспорт и импорт элементов с помощью EWS в Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Экспорт элементов с помощью EWS в Exchange](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

