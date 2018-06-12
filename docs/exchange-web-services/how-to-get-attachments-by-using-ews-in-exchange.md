---
title: Получение вложений с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 12ce3cc0-a201-42e4-93e1-1f57961ff711
description: Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Узнайте, как получить вложения из элементов EWS с помощью управляемого API EWS или протокола EWS в Exchange.
ms.openlocfilehash: 2e1b3cfb346abd068695f66b01f9e34f1f5ff03f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761013"
---
# <a name="get-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="7dfaa-103">Получение вложений с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7dfaa-103">Get attachments by using EWS in Exchange</span></span>

<span data-ttu-id="7dfaa-104">Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Узнайте, как получить вложения из элементов EWS с помощью управляемого API EWS или протокола EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-104">Learn how to get attachments from EWS items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7dfaa-p101">Получить вложения из элемента можно с помощью управляемого API EWS или веб-служб EWS. Извлечение вложений всегда проходит в два этапа, поскольку исходный вызов для получения элемента содержит только метаданные о коллекции вложений элемента. Сперва необходимо извлечь объект, а затем  вложение.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-p101">You can get attachments from an item by using the EWS Managed API or EWS. Because the initial call to get an item only includes metadata about the attachment collection on the item, retrieving attachments is always a two-step process. First, retrieve the item. Next, retrieve the attachment.</span></span>
  
<span data-ttu-id="7dfaa-109">**Таблица 1. Методы управляемого API EWS и операции EWS для добавления вложений**</span><span class="sxs-lookup"><span data-stu-id="7dfaa-109">**Table 1. EWS Managed API methods and EWS operations for adding attachments**</span></span>

|<span data-ttu-id="7dfaa-110">**Задача**</span><span class="sxs-lookup"><span data-stu-id="7dfaa-110">**Task**</span></span>|<span data-ttu-id="7dfaa-111">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="7dfaa-111">**EWS Managed API method**</span></span>|<span data-ttu-id="7dfaa-112">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="7dfaa-112">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7dfaa-113">Получение вложений элемента</span><span class="sxs-lookup"><span data-stu-id="7dfaa-113">Get item attachments</span></span>  <br/> |<span data-ttu-id="7dfaa-114">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) и [ItemAttachment.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment.load%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7dfaa-114">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) followed by [ItemAttachment.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemattachment.load%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="7dfaa-115">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) и [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7dfaa-115">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) followed by [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="7dfaa-116">Получение файловых вложений</span><span class="sxs-lookup"><span data-stu-id="7dfaa-116">Get file attachments</span></span>  <br/> |<span data-ttu-id="7dfaa-117">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) и [FileAttachment.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment.load%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7dfaa-117">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) followed by [FileAttachment.Load](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.fileattachment.load%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="7dfaa-118">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) и [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="7dfaa-118">[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) followed by [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx)</span></span> <br/> |
   
## <a name="get-attachments-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="7dfaa-119">Извлечение вложений из электронного письма с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="7dfaa-119">Get attachments from an email by using the EWS Managed API</span></span>
<span data-ttu-id="7dfaa-120"><a name="bk_getattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7dfaa-120"></span></span>

<span data-ttu-id="7dfaa-121">В следующем примере кода показано, как для получения объекта [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) с помощью метода **привязки** , а затем выполните итерацию по коллекции вложений и вызовите метод **FileAttachment.Load** или **ItemAttachment.Load** на каждом вложение соответствующим образом.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-121">The following code example shows how to get an [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object by using the **Bind** method, then iterate through the attachment collection and call the **FileAttachment.Load** or **ItemAttachment.Load** method on each attachment as appropriate.</span></span> <span data-ttu-id="7dfaa-122">Каждый вложенный файл сохраняется в папку C:\temp\ и каждого вложения элемента загружается в память.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-122">Each file attachment is saved to the C:\temp\ folder, and each item attachment is loaded into memory.</span></span> <span data-ttu-id="7dfaa-123">Сведения о том, как сохранить вложение элемента в разделе [Сохранить вложенные по электронной почте с помощью управляемого интерфейса API веб-служб Exchange](#bk_saveitemattach).</span><span class="sxs-lookup"><span data-stu-id="7dfaa-123">For information about how to save an item attachment, see [Save an attached email by using the EWS Managed API](#bk_saveitemattach).</span></span>
  
<span data-ttu-id="7dfaa-124">В этом примере предполагается, что **service** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), что **itemId** является классом [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) сообщения, из которого будут извлекаться вложения, а также что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-124">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, that **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which attachments will be retrieved, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void GetAttachmentsFromEmail(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message item and retrieve the attachments collection.
    // This method results in an GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Iterate through the attachments collection and load each attachment.
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment is FileAttachment)
        {
            FileAttachment fileAttachment = attachment as FileAttachment;
            // Load the attachment into a file.
            // This call results in a GetAttachment call to EWS.
            fileAttachment.Load("C:\\temp\\" + fileAttachment.Name);
           
            Console.WriteLine("File attachment name: " + fileAttachment.Name);
        }
        else // Attachment is an item attachment.
        {
            ItemAttachment itemAttachment = attachment as ItemAttachment;
            // Load attachment into memory and write out the subject.
            // This does not save the file like it does with a file attachment.
            // This call results in a GetAttachment call to EWS.
            itemAttachment.Load();
            Console.WriteLine("Item attachment name: " + itemAttachment.Name);
        }
    }
}
```

## <a name="get-an-attachment-from-an-email-by-using-ews"></a><span data-ttu-id="7dfaa-125">Извлечение вложения из электронного письма с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="7dfaa-125">Get an attachment from an email by using EWS</span></span>
<span data-ttu-id="7dfaa-126"><a name="bk_getattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7dfaa-126"></span></span>

<span data-ttu-id="7dfaa-p103">Для извлечения вложения с помощью EWS сперва нужно извлечь сообщение и коллекцию вложений, чтобы получить элемент [Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) вложения, которое необходимо извлечь. Получив одно или несколько значений **AttachmentId** для извлечения, вызовите операцию [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx), чтобы загрузить все свойства вложения.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-p103">To get attachments by using EWS, you first need to retrieve the message and the attachment collection to get the [AttachmentId (GetAttachment and DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) of the attachment to retrieve. After you have one or more **AttachmentId** values to retrieve, call the [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) operation to load all the properties for the attachment.</span></span> 
  
<span data-ttu-id="7dfaa-p104">В следующем примере кода показано, как использовать операцию [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения сообщения электронной почты и коллекции вложений сообщения. Кроме того, этот код представляет собой первый XML-запрос, посылаемый управляемым API EWS, если с его помощью [получаете вложения из письма](#bk_getattachewsma). Значения некоторых атрибутов укорочены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-p104">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to get an email message and the collection of attachments on the message. This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [get all attachments from an email](#bk_getattachewsma). The values of some attributes are shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange207_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Attachments" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="ERu/AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7dfaa-132">В ответ на запрос **GetItem** сервер отправляет сообщение [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx), содержащее элемент [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError** (что говорит об успешном извлечении письма) и значения [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) существующих вложений.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-132">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values of the existing attachments.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
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
              <t:ItemId Id="ERu/AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAYEMnd" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="5zTzlqU=" />
                  <t:Name>FileAttachment.txt</t:Name>
                  <t:Size>212</t:Size>
                  <t:LastModifiedTime>2014-05-14T17:59:30</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>false</t:IsContactPhoto>
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="Ktum21o=" />
                  <t:Name>Attached Message Item</t:Name>
                  <t:Size>3063</t:Size>
                  <t:LastModifiedTime>2014-05-14T17:59:30</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                </t:ItemAttachment>
              </t:Attachments>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="7dfaa-133">Теперь, когда у вас есть значения [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx), вызовите операцию [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) для всех вложений, которые необходимо извлечь.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-133">Now that you have the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values, call [GetAttachment](http://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) on each attachment you want to retrieve.</span></span> 
  
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
    <m:GetAttachment>
      <m:AttachmentIds>
        <t:AttachmentId Id="5zTzlqU=" />
      </m:AttachmentIds>
    </m:GetAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7dfaa-134">При извлечении только элемента вложения в ответ на запрос **GetAttachment** сервер отправляет сообщение [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx), содержащее элемент [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError** (что говорит об успешном извлечении вложения) и все элементы элемента вложения, т. е. сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-134">When retrieving an item attachment, the server responds to the **GetAttachment** request with a [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was retrieved successfully, and all the elements for the attached item, which in this case is an email message.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="Ktum21o=" />
              <t:Name>Attached Message Item</t:Name>
              <t:Message>
                <t:ItemClass>IPM.Note</t:ItemClass>
                <t:Subject>Message Item Subject</t:Subject>
                <t:Body BodyType="HTML">&amp;lt;meta http-equiv="Content-Type" 
                    content="text/html; charset=utf-8"&amp;gt;Message Item Body</t:Body>
                <t:Size>2859</t:Size>
                <t:IsSubmitted>false</t:IsSubmitted>
                <t:IsDraft>true</t:IsDraft>
                <t:IsFromMe>false</t:IsFromMe>
                <t:IsResend>false</t:IsResend>
                <t:IsUnmodified>false</t:IsUnmodified>
                <t:DateTimeCreated>2014-05-14T17:59:37Z</t:DateTimeCreated>
                <t:ResponseObjects>
                  <t:ForwardItem />
                </t:ResponseObjects>
                <t:DisplayCc />
                <t:DisplayTo>primary; emaildelegate</t:DisplayTo>
                <t:HasAttachments>false</t:HasAttachments>
                <t:Culture>en</t:Culture>
                <t:EffectiveRights>
                  <t:CreateAssociated>false</t:CreateAssociated>
                  <t:CreateContents>false</t:CreateContents>
                  <t:CreateHierarchy>false</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                </t:EffectiveRights>
                <t:LastModifiedName>primary</t:LastModifiedName>
                <t:LastModifiedTime>2014-05-14T17:59:30Z</t:LastModifiedTime>
                <t:IsAssociated>false</t:IsAssociated>
                <t:WebClientReadFormQueryString>?ItemID=AAMk3D&amp;amp;exvsurl=1&amp;amp;viewmodel=
                    ReadMessageItem</t:WebClientReadFormQueryString>
                <t:ConversationId Id="AAQkADIwM2ZlM2ZlLWMwYjctNDg2N/Rc+d0=" />
                <t:ToRecipients>
                  <t:Mailbox>
                    <t:Name>primary</t:Name>
                    <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                    <t:MailboxType>Mailbox</t:MailboxType>
                  </t:Mailbox>
                  <t:Mailbox>
                    <t:Name>emaildelegate</t:Name>
                    <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                    <t:MailboxType>Mailbox</t:MailboxType>
                  </t:Mailbox>
                </t:ToRecipients>
                <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                <t:ConversationIndex>AQHPb55BxR5Fm0Arx0yY4xbL9Fz53Q==</t:ConversationIndex>
                <t:ConversationTopic>Message Item Subject</t:ConversationTopic>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:ItemAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="7dfaa-135">При извлечении вложенного файла в ответ на запрос **GetAttachment** сервер отправляет сообщение [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx), содержащее элемент [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError** (что говорит об успешном извлечении вложения) и все элементы вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-135">When retrieving a file attachment, the server responds to the **GetAttachment** request with a [GetAttachmentResponse](http://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was retrieved successfully, and all the elements of the file attachment.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="5zTzlqU=" />
              <t:Name>FileAttachment.txt</t:Name>
              <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="save-an-attached-email-by-using-the-ews-managed-api"></a><span data-ttu-id="7dfaa-136">Сохранение вложенного сообщения электронной почты с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="7dfaa-136">Save an attached email by using the EWS Managed API</span></span>
<span data-ttu-id="7dfaa-137"><a name="bk_saveitemattach"> </a></span><span class="sxs-lookup"><span data-stu-id="7dfaa-137"></span></span>

<span data-ttu-id="7dfaa-138">Чтобы сохранить содержимое вложения сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange, необходимо сохранить [MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) в файл.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-138">In order to save the contents of an email attachment using the EWS Managed API, you need to save the [MimeContent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) to a file.</span></span> <span data-ttu-id="7dfaa-139">При этом будут потеряны все расширенные свойства, заданные для элемента, например звонящему флаги и категорий.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-139">In doing so, you will lose any extended properties set on the item, such as follow-up flags and categories.</span></span> <span data-ttu-id="7dfaa-140">В этом примере сохраняет вложения электронной почты в папку C:\temp\.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-140">This example saves the email attachment to the to the C:\temp\ folder.</span></span> 
  
<span data-ttu-id="7dfaa-141">Обратите внимание, что вам не удастся переместить или скопировать вложение в другую папку, так как элемент вложения не является строго типизированным. Поэтому если нужно переместить вложение в другую папку, используйте приведенный ниже пример кода, а затем [импортируйте файл](how-to-import-items-by-using-ews-in-exchange.md) в другую папку.</span><span class="sxs-lookup"><span data-stu-id="7dfaa-141">Note that you cannot move or copy the item attachment to another folder because the item attachment is not a strongly-typed item, so if you're trying to move an attachment to a different folder, use the following code example and then [import the file](how-to-import-items-by-using-ews-in-exchange.md) into a different folder.</span></span> 
  
```cs
public static void SaveEmailAttachment(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message item and retrieve the attachments collection.
    // This method results in an GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment is ItemAttachment)
        {
            ItemAttachment itemAttachment = attachment as ItemAttachment;
            itemAttachment.Load(ItemSchema.MimeContent);
            string fileName = "C:\\Temp\\" + itemAttachment.Item.Subject + ".eml";
            // Write the bytes of the attachment into a file.
            File.WriteAllBytes(fileName, itemAttachment.Item.MimeContent.Content);
            Console.WriteLine("Email attachment name: "+ itemAttachment.Item.Subject + ".eml");
        }
    }
}
```

## <a name="see-also"></a><span data-ttu-id="7dfaa-142">См. также</span><span class="sxs-lookup"><span data-stu-id="7dfaa-142">See also</span></span>


- [<span data-ttu-id="7dfaa-143">Attachments and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="7dfaa-143">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="7dfaa-144">Добавление вложения с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7dfaa-144">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7dfaa-145">Удаление вложений с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="7dfaa-145">Delete attachments by using EWS in Exchange</span></span>](how-to-delete-attachments-by-using-ews-in-exchange.md)
    

