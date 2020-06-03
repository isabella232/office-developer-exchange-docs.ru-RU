---
title: Получение фотографий пользователей с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: f86d1099-1f57-47dc-abf2-4d5ae4e900a9
description: Узнайте, как получить фотографии пользователей, связанные с почтовым ящиком или контактом, с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 14f2bc6bef1ce3c3529f03e213e3ada7c45a5a71
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455788"
---
# <a name="get-user-photos-by-using-ews-in-exchange"></a>Получение фотографий пользователей с помощью EWS в Exchange

Узнайте, как получить фотографии пользователей, связанные с почтовым ящиком или контактом, с помощью управляемого API EWS или EWS в Exchange.
  
Удобно добавлять лицо в имя. Если пользователям требуется добавлять имена в грани, приложение может запросить изображение, как правило, фотографию, из Exchange, который представляет учетную запись электронной почты. Вы можете получить фотографию пользователя, сохраненную на сервере Exchange Server для почтового ящика, или получить фотографию контакта из контактов, хранящихся в почтовом ящике.
  
Вы можете использовать несколько различных технологий для получения фотографий из почтовых ящиков или доменных служб Active Directory (AD DS). Лучший способ получить фотографию зависит от типа контакта, с которого вы хотите получить фотографию. 
  
**Таблица 1. Технологии, используемые для получения фотографий пользователей на основе типа контакта**

|**Тип контакта**|**Используемые технологии**|
|:-----|:-----|
|Фотография пользователя почтового ящика  <br/> |[Получение фотографии пользователя почтового ящика с помощью REST](#bk_REST)<br/><br/> [Получение фотографии пользователя с помощью EWS](#bk_EWS) <br/> |
|Фотография пользователя контакта  <br/> |[Получение фотографии пользователя контакта с помощью управляемого API EWS](#bk_EWSMA)<br/><br/> [Получение фотографии пользователя с помощью EWS](#bk_EWS) <br/> |

<a name="bk_REST"> </a>

## <a name="get-a-mailbox-user-photo-by-using-rest"></a>Получение фотографии пользователя почтового ящика с помощью REST

Вы можете запросить фотографии пользователей с сервера Exchange, используя стандартный запрос **Get** HTTPS. В запросе укажите адрес учетной записи электронной почты и код размера для изображения, как показано в следующем примере. 
  
```HTML
https://Exchange Server/ews/Exchange.asmx/s/GetUserPhoto?email=email address&amp;size=size code
```

Используйте операцию [GetUserSettings](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) службы автообнаружения для получения параметра **екстерналевсурл** , который содержит URL-адрес конечной точки веб-служб Exchange (EWS), и расположение обработчика HTTP- **сообщений Exchange. asmx** , который возвращает фотографии пользователей. 
  
Каждый код размера указывает высоту и ширину изображения в пикселях. Например, код размера **HR48x48** возвращает изображение размером 48 пикселей в высоту, равное 48 x ширина. Возможные значения параметра кода размера совпадают с возможными значениями для элемента [сизерекуестед](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) . Если запрос указывает недоступный размер, будет возвращена самая большая доступная фотография. Если на сервере Exchange не хранится фотография, будет возвращено эскизное изображение, хранящееся в доменных СЛУЖБах Active Directory для учетной записи. 
  
> [!NOTE]
> Код размера **HR48x48** всегда возвращает изображение ЭСКИЗА AD DS, если оно доступно. 
  
В приведенном ниже примере показано, как можно использовать запрос GET для получения фотографии пользователя для Ольга и сохранения его на локальном компьютере.
  
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

Запрос возвратит HTTP-ответ. 
  
**Таблица 2. Коды отклика для запроса GetUserPhoto**

|**Response code** (Код ответа)|**Описание**|
|:-----|:-----|
|200  <br/> |Для указанной учетной записи электронной почты доступен образ, а в ответе присутствует двоичный образ.  <br/> |
|304  <br/> |Изображение не изменилось со времени последнего возврата **ETag** в приложение.  <br/> |
|404  <br/> |Нет доступных изображений для указанной учетной записи электронной почты.  <br/> |

<a name="bk_REST"> </a>

## <a name="cache-user-photos"></a>Кэширование фотографий пользователей

Exchange возвращает данные с типом контента Image/JPEG, а также коллекцию значений заголовков. Заголовок **ETag** похож на ключ изменения. Значение — это строка, представляющая время последнего обновления фотографии. **Тег eTag** остается таким же для фотографии пользователя, пока не будет изменена фотография. Это значение **ETag** можно отправить на сервер в запросе HTTPS **Get** в заголовке **If – None – ПОИСКПОЗ** . Если с момента последнего запроса фотография не изменилась, сервер ответит ответ HTTP 304, который показывает, что это так. Это означает, что вы можете использовать фотографию пользователя, которую вы запросили и сохранили, вместо обработки новой. 

<a name="bk_EWSMA"> </a>

## <a name="get-a-contact-user-photo-by-using-ews-managed-api"></a>Получение фотографии пользователя контакта с помощью управляемого API EWS

Приложение может использовать управляемый API EWS для получения фотографий для контактов, если контакт хранится в папке контактов в почтовом ящике пользователя. Для этого сначала найдите идентификатор **элемента для контакта, который необходимо** использовать. Затем после привязывания к этому контакту загрузите его в коллекцию вложений. Если у контакта есть фотография, фотография будет одним из вложений. Пройдите по коллекции вложений, проверив значение свойства **исконтактфото** . Когда вы найдете фотографию контакта, вы можете сохранить ее на локальном компьютере, и приложение сможет получить к нему доступ. 
  
Этот процесс показан в приведенном ниже примере. В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
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

## <a name="get-a-user-photo-by-using-ews"></a>Получение фотографии пользователя с помощью EWS

Если вы получаете фотографию пользователя из доменных служб Active Directory, вы можете использовать операцию [GetUserPhoto](https://msdn.microsoft.com/library/f6e8143d-4235-428e-8f9c-ab6e9b1cfa6e%28Office.15%29.aspx) (если вы знаете адрес электронной почты) или операцию [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) (если вы не знаете адрес электронной почты). Если вы получаете фотографию пользователя из папки "Контакты" в почтовом ящике, используйте операцию [GetItem](https://msdn.microsoft.com/library/6b96dace-1260-4b83-869a-7c31c5583daa%28Office.15%29.aspx) , а затем операцию [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) . В обоих случаях фотография возвращается в виде строки в виде строки с кодировкой base64 в ответе XML. 
  
### <a name="get-a-mailbox-user-photo-by-using-the-getuserphoto-operation"></a>Получение фотографии пользователя почтового ящика с помощью операции GetUserPhoto

Использование операции **GetUserPhoto** является простым. В XML-запросе укажите адрес электронной почты пользователя и размер возвращаемой [фотографии](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) (в элементе [сизерекуестед](https://msdn.microsoft.com/library/e86f98b6-83b5-4530-80eb-dc5df42e2c62%28Office.15%29.aspx) ). В приведенном ниже примере XML-запроса показано, как получить фотографию для Ольга Даниелс шириной 360 пикселя на 360 пикселя высотой. 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Ниже приведен XML-ответ. Фотография в кодировке Base64 хранится в элементе [PictureData](https://msdn.microsoft.com/library/1124eac3-ebf2-4b81-96d3-96838c840433%28Office.15%29.aspx) (содержимое было сокращено для удобочитаемости). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetUserPhotoResponse ResponseClass="Success" 
         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <HasChanged>true</HasChanged>
      <PictureData>/9j/4AAQSkZJRgABAQEAYABgAAD/2wBDAAg... wATRRRSuB//2Q==</PictureData>
    </GetUserPhotoResponse>
  </s:Body>
</s:Envelope>

```

### <a name="get-a-mailbox-user-photo-by-using-the-resolvenames-operation"></a>Получение фотографии пользователя почтового ящика с помощью операции ResolveNames

Если вы не знаете адрес электронной почты пользователя, для которого вы получаете фотографию, вы можете [использовать операцию ResolveNames](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md) , чтобы получить кандидатов для возможных сопоставлений. Если для атрибута **контактдаташапе** элемента [ResolveNames](https://msdn.microsoft.com/library/c85207e1-1315-443b-94ec-2b58f405076b%28Office.15%29.aspx) задано значение "аллпропертиес", для каждого кандидата будет возвращено множество данных, включая фотографии пользователя. В следующем примере показан XML-запрос для разрешения имени "Ольга" и возврата всех свойств для каждого кандидата. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

В ответе будет возвращено множество данных. В приведенном ниже примере показаны только те данные, которые относятся к фотографии пользователя. Элемент **Photo** содержит фотографию пользователя с кодировкой base64 (содержимое было сокращено для удобочитаемости). 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="get-a-contact-user-photo-by-using-the-getattachment-operation"></a>Получение фотографии пользователя контакта с помощью операции GetAttachment

С помощью EWS вы можете получать фотографии из контактов, хранящихся в почтовом ящике. Для начала используйте операцию **GetItem** , чтобы возвратить все свойства, чтобы можно было искать фотографии. В следующем примере показан XML-запрос для получения элемента контакта. Идентификатор элемента был сокращен для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
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

Найдите элемент [хаспиктуре](https://msdn.microsoft.com/library/922a43fe-01bd-49f2-9261-e00e4699b8da%28Office.15%29.aspx) , чтобы убедиться, что контакт имеет связанную фотографию. Затем просмотрите коллекцию вложений, для которой для элемента [исконтактфото](https://msdn.microsoft.com/library/ae36b5f9-a787-4863-9dbc-258ad724801d%28Office.15%29.aspx) задано значение true. В приведенном ниже примере ответа показаны только нужные данные. Значения ИДЕНТИФИКАТОРов сокращаются для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Затем используйте операцию **GetAttachment** с **AttachmentId** , чтобы запросить вложение, имеющее фотографию контакта. В следующем примере показан XML-запрос для получения вложения. Идентификатор сокращен для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
         <t:AttachmentId Id="1LGlhgpgoA="/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показан XML-ответ со сведениями о запрошенном вложении. Элемент [Content](https://msdn.microsoft.com/library/24f8c54a-505f-4fc0-b7e7-93ad50b97070%28Office.15%29.aspx) содержит строку в кодировке Base64 для фотографии пользователя, что в этом примере сокращается для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="decode-a-base64-encoded-string"></a>Декодирование строки в кодировке Base64

Независимо от того, какую операцию вы используете для получения фотографии пользователя, вам потребуется декодировать эту строку, чтобы ее можно было использовать в приложении. В приведенном ниже примере показано, как декодировать строку, а затем сохранить ее на локальном компьютере, чтобы приложение могло получить к нему доступ позже.
  
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
- [Устранение неоднозначности имен с помощью EWS в Exchange 2013](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)    
- [Пакетная обработка контактов с помощью EWS в Exchange](how-to-process-contacts-in-batches-by-using-ews-in-exchange.md)
    

