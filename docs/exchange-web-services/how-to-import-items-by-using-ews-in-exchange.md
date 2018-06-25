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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761068"
---
# <a name="import-items-by-using-ews-in-exchange"></a>Импорт элементов с помощью веб-служб Exchange в Exchange

Узнайте, как импортировать встречи, сообщения электронной почты, контакты, задачи и других элементов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Многие системы содержат встреч, сообщения электронной почты, контакты и задачи, и можно импортировать эти элементы в Exchange в несколько способов. Импорт элементов в Exchange при простой связи почтового ящика не сохраняются на этих элементов. Можно использовать метод управляемый API EWS [Item.Save](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) или операции EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания элементов в почтовый ящик Exchange. Простой подход не поддерживает все сценарии Например: 
  
- Не может обеспечить согласованность между организаторов и участники при импорте встреч человек (собрания). Это означает, что организатор собрания могут потребоваться для повторной отправки приглашения на собрания участникам, чтобы восстановить связь между организатора и участников. Если Встреча была импортирована в календаре участника, встречи не связаны с организатором встречи. Участники, необходимо принять повторно отправленная приглашение из картинок для возобновления отношения Организатор attendee.
    
- Сведения о назначенных не сохраняются при импорте назначенных задач.
    
Все параметры импорта можно использовать для пакетного импорта элементов в Exchange.
  
## <a name="use-ews-managed-api-or-ews-item-types-to-import-an-item"></a>Управляемый API EWS использования или веб-служб Exchange типов для импорта элемента элементов
<a name="bk_importproperties"> </a>

Управляемый API EWS или веб-служб Exchange можно использовать для импорта сообщения электронной почты, контакты, встречи или задачи из других систем. Снова задайте [Свойства](properties-and-extended-properties-in-ews-in-exchange.md) из исходный формат на любой из следующих объектов в зависимости от того, что импорт. 
  
**В таблице 1. Управляемый API EWS объекты и элементы веб-служб Exchange**

|**Управляемый API EWS объектов**|**Элемент веб-служб Exchange**|
|:-----|:-----|
|[EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) <br/> |[Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) <br/> |
|[Контакт](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) <br/> |[Контакт](http://msdn.microsoft.com/library/66bfff50-7a91-4d81-b6a0-610b9962f677%28Office.15%29.aspx) <br/> |
|[Встреча](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) <br/> |[Элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) <br/> |
|[Задача](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.task%28v=exchg.80%29.aspx) <br/> |[Задача](http://msdn.microsoft.com/library/7c84927e-db28-4c5d-b0b5-cbcc2b88d869%28Office.15%29.aspx) <br/> |
   
Используйте метод управляемый API EWS [Item.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) или [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) операции веб-служб Exchange для выполнения импорта элементов. Такой подход рекомендуется при импорте элементов из других систем потому, что у вас есть элемент управления, через который импортируется свойства. Дополнительные сведения о том, как задать свойства элементов, а затем сохраните элемент можно [Создать элемент с помощью управляемого интерфейса API веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createewsma) или [Создать элемент с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_createews).
  
## <a name="import-items-with-full-fidelity"></a>Импорт элементов с корректном
<a name="bk_importproperties"> </a>

Отправка элемента как поток данных можно использовать операцию EWS [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) . Представление потока данных этот элемент должен поступают из результаты вызова операции [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) . Так как управляемый API EWS не реализует операцию **UploadItems** при использовании управляемого интерфейса API веб-служб Exchange, необходимые для написания процедуры для отправки веб-запросов. 
  
Это самый простой способ импорта элементов, которые были экспортированы из другой сервер Exchange.
  
В следующем примере содержимое элемента **данных** и идентификаторы сокращаются для удобства чтения. 
  
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

Сервер отвечает на запрос **UploadItems** с элементом [UploadItemsResponse](http://msdn.microsoft.com/library/93044d39-4489-456a-8cce-b6d69873348f%28Office.15%29.aspx) , что, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что элемент был отправлен успешно. Ответ также включает в себя идентификатор элемента загруженного элемента. 
  
## <a name="use-the-mime-stream-to-import-from-common-file-formats"></a>Использовать MIME-поток для импорта из распространенные форматы файлов
<a name="bk_importproperties"> </a>

Веб-служб Exchange можно импортировать файлы iCal (.ics) и EML (файл). Может потребоваться для проверки содержимого MIME для просмотра как средство синтаксического анализа Exchange MIME обрабатывает содержимого MIME-поток. Хотя использование MIME-поток удобен, обычно лучше [типов для импорта элемента элементов управляемый API EWS использования или веб-служб Exchange](#bk_importproperties). Ниже приведен пример того, как для [импорта визитной карточки](http://code.msdn.microsoft.com/How-to-Import-vCard-Files-ffa0ff50).
  
### <a name="use-the-ews-managed-api-to-import-an-email-from-an-eml-file-by-using-the-mime-stream"></a>Использовать управляемый API EWS для импорта на адрес электронной почты из EML-файла с помощью потока MIME

Следующем примере показано, как задать свойство [MimeContent](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) с содержимым EML-файла, а затем импортировать сообщение электронной почты в почтовый ящик. В этом примере также показано, как задать [PidTagMessageFlags (0x0E07)](http://msdn.microsoft.com/en-us/library/office/cc839733%28v=office.15%29.aspx) расширенные свойства на импортированных электронной почты, чтобы он не отображается в почтовом ящике как черновик элемента. В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и пользователь может выполнять проверку подлинности для Exchange server. 
  
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

### <a name="use-the-ews-managed-api-to-import-an-appointment-from-an-ical-file-by-using-the-mime-stream"></a>Использовать управляемый API EWS для импорта встречу из iCal файла с помощью потока MIME

Простой встречи в формате iCalendar файлы можно импортировать с помощью MIME-поток. Нельзя импортировать собраний, которые являются встреч человек, так как связь между организаторам собрания и участников должно быть задано как часть рабочего процесса, [Ведение календаря Exchange](calendars-and-ews-in-exchange.md) . Участники не могут записаны в MIME-поток. 
  
В следующем примере кода показано, как для импорта простой ICS-файл в почтовом ящике пользователя.
  
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

### <a name="use-ews-to-import-an-item-by-using-the-mime-stream"></a>Использование веб-служб Exchange для импорта элемента с помощью потока MIME

Можно использовать операцию EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) Импорт EML и iCal элементов с помощью своих MIME-поток. 
  
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

## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_importproperties"> </a>

После импорта элементов в почтовом ящике, может потребоваться [создать настраиваемые папки для хранения импортированных элементов](how-to-work-with-folders-by-using-ews-in-exchange.md)или [синхронизировать элементы вашего клиента и почтового ящика](mailbox-synchronization-and-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также


- [Экспорт и импорт элементов с помощью веб-служб Exchange в Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md)
    
- [Экспорт элементов с помощью веб-служб Exchange в Exchange](how-to-export-items-by-using-ews-in-exchange.md)
    
- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)
    
- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

