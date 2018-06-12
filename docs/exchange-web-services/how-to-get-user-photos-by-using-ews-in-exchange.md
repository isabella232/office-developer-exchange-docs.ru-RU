---
title: Получение фотографий с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Узнайте, как получить пользовательские фотографии, которые связаны с почтовым ящиком или контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: f0f5cddd41fc563fb9ed38e75b505830a3992411
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761045"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a>Получение фотографий с помощью веб-служб Exchange в Exchange

Узнайте, как получить пользовательские фотографии, которые связаны с почтовым ящиком или контактов с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Приятно поместить фрагмент с именем. Если для помещения имен граней пользователей, приложение может запрашивать изображения, обычно фотографии, Exchange, который представляет учетную запись электронной почты. Можно получить фото пользователя, хранящиеся на сервере Exchange server для почтовых ящиков, либо вы можете получить фотографий контактов на контакты, хранятся в почтовом ящике пользователя.
  
Несколько новых технологий можно использовать для получения фотографии из почтовых ящиков или доменных служб Active Directory (AD DS). Лучший способ получить фотографию зависит от типа контакта, которого требуется получать фотографию с. 
  
**В таблице 1. Технологии использовать для получения фотографии пользователя на основе типа контакта**

|**Тип контакта**|**Технологии использовать**|
|:-----|:-----|
|Фото пользователя почтового ящика  <br/> |[Получение фото пользователя почтового ящика с помощью REST](#bk_REST)<br/><br/> [Получение фото пользователя с помощью веб-служб Exchange](#bk_EWS) <br/> |
|Фотографии контактов пользователя  <br/> |[Получение фотографий контактов пользователя с помощью управляемого интерфейса API веб-служб Exchange](#bk_EWSMA)<br/><br/> [Получение фото пользователя с помощью веб-служб Exchange](#bk_EWS) <br/> |

<a name="bk_REST"> </a>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a>Получение фото пользователя почтового ящика с помощью REST

Можно запросить фотографии пользователя с сервера Exchange с помощью стандартного запроса HTTPS, **Получение** . В запросе укажите адрес электронной почты учетной записи и кода размер изображения, как показано в следующем примере. 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

Используйте операцию [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) службы автообнаружения для получения параметр **ExternalEwsUrl** , который содержит URL-адрес конечной точки веб-служб Exchange (EWS) и расположение обработчик **Exchange.asmx** HTTP, который возвращает фотографии пользователя. 
  
Код каждого размер указывает высоту и ширину изображения в пикселях. Например код размер **HR48x48** возвращает изображение, которое является 48 пикселов в высоту и 48 пикселей в высоту. Возможные значения для параметра кода размер совпадают с возможными значениями для элемента [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) . Если запрос указывает размер, который не поддерживается, будут возвращены наибольшее доступных фотографий. Если нет фотографий хранится на сервере Exchange, будут возвращены эскизное изображение, хранящиеся в AD DS для учетной записи. 
  
> [!NOTE]
> Код размера **HR48x48** всегда возвращает эскизное изображение Доменные службы Active Directory, если он доступен. 
  
В следующем примере показано, как использовать запрос GET для извлечения фото пользователя для Sadie и сохраните его на локальный компьютер.
  
```cs
// Create the web request with the REST URL.
HttpWebRequest request = 
   WebRequest.Create("https://www.contoso.com/ews/exchange.asmx/s/GetUserPhoto?email=sadie@contoso.com&amp;size=HR240x240") 
   as HttpWebRequest;
// Submit the request.
using (HttpWebResponse resp = request.GetResponse() as HttpWebResponse)
{
   // Take the response and save it as an image.
   Bitmap image = new Bitmap(resp.GetResponseStream());
   image.Save("Sadie.jpg");
}

```

Запрос возвращает HTTP-ответа. 
  
**В таблице 2. Коды ответа на запрос GetUserPhoto**

|**Код ответа**|**Описание**|
|:-----|:-----|
|200  <br/> |Изображение доступен для учетной записи электронной почты указанного и двоичные изображение находится в ответе.  <br/> |
|304  <br/> |Изображение не был изменен с момента последнего **ETag** был возвращен в приложение.  <br/> |
|404  <br/> |Изображение не доступна для учетной записи электронной почты указанного.  <br/> |

<a name="bk_REST"> </a>

## <a name="cache-user-photos"></a>Фотографии пользователя кэша

Exchange возвращает данные с типом контента изображение/jpeg, а также коллекцию значений заголовка. Заголовок **ETag** аналогична изменить ключ. Значение — это строка, представляющая время последнего обновления фотографии. **ETag** остаются неизменными для фото пользователя, пока не будет изменено фотографии. Это значение **ETag** можно отправлять на сервер в запросе на **Получение** HTTPS в заголовок **If-None-Match** . Если фотографии не изменилось с момента последнего запроса, сервер отправляет ответ HTTP 304, которое указывает, таким образом. Это означает, что можно использовать фото пользователя, который ранее был запрошен и сохранения вместо обработки новый. 

<a name="bk_EWSMA"> </a>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a>Получение фотографий контактов пользователя с помощью управляемого интерфейса API веб-служб Exchange

Приложение может использовать управляемый API EWS для получения фотографии контактов, если контакт хранится в папке контактов в почтовом ящике пользователя. Для этого сначала найдите **идентификатор элемента** для контакта требуется использовать. Затем после привязки к этому контакту, загрузите его в коллекцию вложений. Если у контакта фотографии, фотография будет вложений. Просмотрите коллекцию вложений, проверки значения свойства **IsContactPhoto** . Найдя фотографий контактов, можно сохранить его на локальный компьютер и приложение может получить доступ к. 
  
В следующем примере показано выполнение этого процесса. В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
private static void GetContactPhoto(ExchangeService service, string ItemId)
{
   // Bind to an existing contact by using the ItemId passed into this function.
   Contact contact = Contact.Bind(service, ItemId);
   // Load the contact to get access to the collection of attachments.
   contact.Load(new PropertySet(ContactSchema.Attachments));
   // Loop through the attachments looking for a contact photo.
   foreach (Attachment attachment in contact.Attachments)
   {
      if ((attachment as FileAttachment).IsContactPhoto)
      {
         // Load the attachment to access the content.
         attachment.Load();
      }
   }
   FileAttachment photo = contact.GetContactPictureAttachment();
   // Create a file stream and save the contact photo to your computer.
   using (FileStream file = new FileStream(photo.Name, FileMode.Create, System.IO.FileAccess.Write))
   {
      photo.Load(file);
   }
}

```

<a name="bk_EWS"> </a>

## <a name="get-a-user-photo-by-using-ews"></a>Получение фото пользователя с помощью веб-служб Exchange

Они будут фото пользователя из Доменные службы Active Directory, можно использовать операцию [GetUserPhoto](http://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (Если вы знаете адрес электронной почты) или операции [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (Если вы не знаете адрес электронной почты). Если они будут фото пользователя из папки "Контакты" в почтовом ящике, с помощью операции [GetItem](http://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) , следуют операции [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) . В любом случае фотографии возвращается как строка в кодировке Base64 в ответе XML. 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a>Получение фото пользователя почтового ящика с помощью операции GetUserPhoto

С помощью операции **GetUserPhoto** не вызывает затруднений. В XML-запрос укажите адрес электронной почты пользователя и [размер фотографии](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) для возврата (в элементе [SizeRequested](http://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ). В следующем примере запрос XML показано, как получить фотографию для Sadie Daniels, который является 360 пикселов 360 пикселей. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013 "/>
   </soap:Header>
   <soap:Body>
      <m:GetUserPhoto>
         <m:Email>sadie@contoso.com</m:Email>
         <m:SizeRequested>HR360x360</m:SizeRequested>
      </m:GetUserPhoto>
   </soap:Body>
</soap:Envelope>

```

Ниже приведен XML-ответ. Photo кодировки Base64 содержится в элементе [Свойства](http://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (содержимое URL были сокращены для удобства чтения). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a>Получение фото пользователя почтового ящика с помощью операции ResolveNames

Если вы не знаете адрес электронной почты пользователя, для которого вы получаете фотографию, можно [использовать операцию ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) , чтобы получить кандидатов для возможно соответствие. При указании «AllProperties» для атрибута **ContactDataShape** элемента [ResolveNames](http://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) большого объема данных, включая пользовательские фотографии, будут возвращены для каждого кандидата. В следующем примере показано XML-запрос для разрешения имени «Sadie» и получить все свойства для каждого кандидата. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>  
<soap:Body>
  <m:ResolveNames ReturnFullContactData="true" ContactDataShape="AllProperties">
      <m:UnresolvedEntry>sadie</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

В ответе будут возвращены большого объема данных. В следующем примере показано только данные, относящиеся к фото пользователя. Элемент **фотографий** содержит кодировки Base64 фото пользователя (содержимое URL были сокращены для удобства чтения). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ResolutionSet TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>Sadie Daniels</t:Name>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Mailbox</t:MailboxType>
              </t:Mailbox>
              <t:Contact>
                <t:DisplayName>Sadie Daniels</t:DisplayName>
                <t:GivenName>Sadie</t:GivenName>
                <t:Initials/>
                <t:CompanyName>CONTOSO</t:CompanyName>
......
                <t:Photo>/9j/4AAQSkZJRgABAQE...qKKKAP/2Q==</t:Photo>
......
              </t:Contact>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a>Получение фотографий контактов пользователя с помощью операции GetAttachment

Можно использовать веб-служб Exchange для получения фотографии с контактами, хранятся в почтовом ящике пользователя. Во-первых используйте операции **GetItem** для возврата всех свойств, поэтому можно искать фотографии. В следующем примере показано XML-запрос для получения элемента контакта. Идентификатор элемента был усечен для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='http://schemas.microsoft.com/exchange/services/2006/messages'>
      <ItemShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>

```

Найдите элемент [HasPicture](http://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) чтобы убедиться, что контакт находится связанных фотографий. Найдите через коллекцию вложений, которая имеет значение true для элемента [IsContactPhoto](http://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) . В следующем примере ответа показано только нужные данные. Значения Идентификаторов сокращаются для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAAGECXAAA=" ChangeKey="EQAAABYAAAD2WuN+TpqwSrNP9JCCMKC0AABLzXRv"/>
              <t:ParentFolderId Id="nIxIAAA=" ChangeKey="AQAAAA=="/>
              <t:ItemClass>IPM.Contact</t:ItemClass>
              <t:Subject>Hope Gross</t:Subject>
              <t:Sensitivity>Normal</t:Sensitivity>
......
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="1LGlhgpgoA="/>
                  <t:Name>ContactPicture.jpg</t:Name>
                  <t:Size>6260</t:Size>
                  <t:LastModifiedTime>2011-03-09T16:55:55</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>true</t:IsContactPhoto>
                </t:FileAttachment>
              </t:Attachments>
......
              <t:HasPicture>true</t:HasPicture>
            </t:Contact>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

Затем используйте операции **GetAttachment** с помощью **идентификатора вложения AttachmentId** для запроса вложения с фотографий контактов. В следующем примере показано запроса XML для получения вложения. Идентификатор сокращение для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показано XML-ответ со сведениями о вложении запрошенного. Элемент [содержимого](http://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) содержит строку в кодировке Base64 для фото пользователя, сокращение в этом примере для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="+KsDBEr1LGlhgpgoA="/>
              <t:Name>ContactPicture.jpg</t:Name>
              <t:Content>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg...D//2Q==</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>

```

<a name="bk_EWS"> </a>

## <a name="decode-a-base64-encoded-string"></a>Декодирования строка в кодировке Base64

Независимо от того, операция, которую можно использовать для получения фото пользователя вам потребуются для декодирования эту строку, чтобы можно было использовать в приложении. Следующем примере показано, как декодировать строки, а затем сохраните на локальный компьютер, поэтому приложения могут обращаться к ней позже.
  
```cs
// Convert the encoded string into a byte array.
byte[] data = System.Convert.FromBase64String(Photo);
// Create a memory stream to read the data.
MemoryStream ms = new MemoryStream(data);
// Save the data on your local computer as a JPG image.
using (FileStream file = new FileStream(ContactName + ".jpg", FileMode.Create, System.IO.FileAccess.Write))
{
   byte[] bytes = new byte[ms.Length];
   ms.Read(bytes, 0, (int)ms.Length);
   file.Write(bytes, 0, bytes.Length);
   ms.Close();
}

```

## <a name="see-also"></a>См. также

- [Пользователи и контакты в EWS для Exchange](people-and-contacts-in-ews-in-exchange.md)    
- [Разрешения неоднозначных имен с помощью веб-служб Exchange в Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [Процесс контакты партиями с помощью веб-служб Exchange в Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

