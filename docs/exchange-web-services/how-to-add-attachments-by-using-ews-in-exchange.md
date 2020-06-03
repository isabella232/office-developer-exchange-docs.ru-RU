---
title: Добавление вложений с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 0cbce436-2ae6-4fcc-bd8b-f517a0724e55
description: Узнайте, как создавать новые элементы с вложениями или добавлять вложения в существующие элементы с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: fa98eb437d1289f25cfb827b6fa9b351d842bd40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528267"
---
# <a name="add-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="1489c-103">Добавление вложений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1489c-103">Add attachments by using EWS in Exchange</span></span>

<span data-ttu-id="1489c-104">Узнайте, как создавать новые элементы с вложениями или добавлять вложения в существующие элементы с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="1489c-104">Learn how to create new items with attachments, or add attachments to existing items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="1489c-105">С помощью управляемого API EWS или веб-служб Exchange можно добавлять вложенные файлы или вложения элементов в новые или существующие элементы.</span><span class="sxs-lookup"><span data-stu-id="1489c-105">You can add file attachments or item attachments to new or existing items by using the EWS Managed API or EWS.</span></span> <span data-ttu-id="1489c-106">Если вы используете управляемый API EWS, вы можете использовать один и тот же метод для добавления вложений в новые или существующие элементы; Тем не менее, метод изменяется, если вы используете вложение файла или элемента.</span><span class="sxs-lookup"><span data-stu-id="1489c-106">If you are using the EWS Managed API, you use the same method to add attachments to new or existing items; however, the method changes if you're using a file or item attachment.</span></span> <span data-ttu-id="1489c-107">Если вы используете EWS, то же самое действие можно использовать для добавления вложенного файла или элемента в элемент, но если вы добавляете вложение в новый или существующий элемент, операция изменяется.</span><span class="sxs-lookup"><span data-stu-id="1489c-107">Conversely, if you are using EWS, you use the same operation to add either a file or item attachment to an item, but the operation changes if you're adding the attachment to a new or existing item.</span></span>
  
<span data-ttu-id="1489c-108">**Таблица 1. Методы управляемого API EWS и операции EWS для добавления вложений**</span><span class="sxs-lookup"><span data-stu-id="1489c-108">**Table 1. EWS Managed API methods and EWS operations for adding attachments**</span></span>

|<span data-ttu-id="1489c-109">**Задача**</span><span class="sxs-lookup"><span data-stu-id="1489c-109">**Task**</span></span>|<span data-ttu-id="1489c-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="1489c-110">**EWS Managed API method**</span></span>|<span data-ttu-id="1489c-111">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="1489c-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1489c-112">Добавление вложенного файла в новую или существующую электронную почту</span><span class="sxs-lookup"><span data-stu-id="1489c-112">Add a file attachment to a new or existing email</span></span>  <br/> |[<span data-ttu-id="1489c-113">Аттачментколлектион. Аддфилеаттачмент</span><span class="sxs-lookup"><span data-stu-id="1489c-113">AttachmentCollection.AddFileAttachment</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="1489c-114">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) для нового сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="1489c-114">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) for a new email</span></span>  <br/> <span data-ttu-id="1489c-115">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) для добавления в существующую электронную почту</span><span class="sxs-lookup"><span data-stu-id="1489c-115">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) to add to an existing email</span></span>  <br/> |
|<span data-ttu-id="1489c-116">Добавление вложения элемента в новую или существующую электронную почту</span><span class="sxs-lookup"><span data-stu-id="1489c-116">Add an item attachment to a new or existing email</span></span>  <br/> |[<span data-ttu-id="1489c-117">Аттачментколлектион. Аддитематтачмент</span><span class="sxs-lookup"><span data-stu-id="1489c-117">AttachmentCollection.AddItemAttachment</span></span>](https://msdn.microsoft.com/library/dd634986%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="1489c-118">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) для нового сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="1489c-118">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) for a new email</span></span>  <br/> <span data-ttu-id="1489c-119">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) для добавления в существующую электронную почту</span><span class="sxs-lookup"><span data-stu-id="1489c-119">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) to add to an existing email</span></span>  <br/> |
   
## <a name="create-an-email-with-file-and-item-attachments-by-using-the-ews-managed-api"></a><span data-ttu-id="1489c-120">Создание сообщения электронной почты с вложениями файлов и элементов с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="1489c-120">Create an email with file and item attachments by using the EWS Managed API</span></span>
<span data-ttu-id="1489c-121"><a name="bk_createattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1489c-121"><a name="bk_createattachewsma"> </a></span></span>

<span data-ttu-id="1489c-122">В приведенном ниже примере кода показано, как создать сообщение электронной почты с несколькими вложенными файлами и вложением элемента, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="1489c-122">The following code example shows how to create an email with multiple file attachments and an item attachment by:</span></span> 
  
1. <span data-ttu-id="1489c-123">Использование объекта [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) для создания сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-123">Using the [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message.</span></span> 
    
2. <span data-ttu-id="1489c-124">Добавление вложений к сообщению с помощью методов [аттачментколлектион. аддфилеаттачмент](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) и [аттачментколлектион. аддитематтачмент](https://msdn.microsoft.com/library/dd634986%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1489c-124">Using the [AttachmentCollection.AddFileAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) and [AttachmentCollection.AddItemAttachment](https://msdn.microsoft.com/library/dd634986%28v=exchg.80%29.aspx) methods to add attachments to the message.</span></span> 
    
3. <span data-ttu-id="1489c-125">С помощью метода [EmailMessage. SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) отправьте сообщение получателям и сохраните сообщение в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="1489c-125">Using the [EmailMessage.SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipients and save the message in the Sent Items folder.</span></span> 
    
<span data-ttu-id="1489c-126">В этом примере кода показаны четыре способа, с помощью которых можно добавить файл вложения в элемент с помощью управляемого API EWS:</span><span class="sxs-lookup"><span data-stu-id="1489c-126">This code example shows the four ways in which a file attachment can be added to an item by using the EWS Managed API:</span></span>
  
- <span data-ttu-id="1489c-127">С помощью полного расположения файлов.</span><span class="sxs-lookup"><span data-stu-id="1489c-127">By using a fully qualified file location.</span></span>
    
- <span data-ttu-id="1489c-128">С помощью полного расположения файла и имени вложения.</span><span class="sxs-lookup"><span data-stu-id="1489c-128">By using a fully qualified file location and a new attachment name.</span></span>
    
- <span data-ttu-id="1489c-129">С помощью массива байтов.</span><span class="sxs-lookup"><span data-stu-id="1489c-129">By using a byte array.</span></span>
    
- <span data-ttu-id="1489c-130">С помощью потока.</span><span class="sxs-lookup"><span data-stu-id="1489c-130">By using a stream.</span></span>
    
<span data-ttu-id="1489c-131">Обратите внимание, что вложение элемента в этом примере создается одновременно с сообщением электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-131">Note that the item attachment in this example is created at the same time as the email message.</span></span> <span data-ttu-id="1489c-132">Чтобы добавить существующее сообщение электронной почты в качестве вложения элемента, ознакомьтесь со статьей [Добавление существующего элемента в новое сообщение электронной почты с помощью сохранитьmimecontent и управляемого API EWS](#bk_addexistingemailewsma).</span><span class="sxs-lookup"><span data-stu-id="1489c-132">To add an existing email message as an item attachment, see [Add an existing item to a new email by using the MimeContent and the EWS Managed API](#bk_addexistingemailewsma).</span></span>
  
<span data-ttu-id="1489c-133">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="1489c-133">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void CreateEmailWithAttachments(ExchangeService service)
{
    // Create an email message and set properties on the message.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Message with Attachments";
    message.Body = "This message contains four file attachments 
        and one message item attachment.";
    message.ToRecipients.Add("sadie@contoso.com");
    message.ToRecipients.Add("ronnie@contoso.com");
    // Add a file attachment by using the fully qualified location of the file. 
    message.Attachments.AddFileAttachment("C:\\temp\\FileAttachment.txt");
    // Add a file attachment by using the fully qualified string name, 
    // and specify the name of the attachment as it will appear in the email.
    // The new name of the file attachment is SecondAttachment.txt.
    message.Attachments.AddFileAttachment("SecondAttachment.txt", "C:\\temp\\FileAttachment2.txt");
    // Add a file attachment by using a byte array.
    // In this example, theBytes is the byte array that represents the content of the image file to attach.
    byte[] theBytes = File.ReadAllBytes("C:\\Temp\\Tulips.jpg");
    // The byte array file attachment is named ThirdAttachment.jpg.
    message.Attachments.AddFileAttachment("ThirdAttachment.jpg", theBytes);
    // Add a file attachment by using a stream.
    FileStream theStream = new FileStream("C:\\temp\\FileAttachment4.txt", FileMode.OpenOrCreate);
    // The streamed file attachment is named FourthAttachment.txt.
    message.Attachments.AddFileAttachment("FourthAttachment.txt", theStream);
    // Add an email message as an item attachment and set properties on the item.
    ItemAttachment<EmailMessage> itemAttachment = message.Attachments.AddItemAttachment<EmailMessage>();
    itemAttachment.Name = "Attached Message Item";
    itemAttachment.Item.Subject = "Message Item Subject";
    itemAttachment.Item.Body = "Message Item Body";
    itemAttachment.Item.ToRecipients.Add("sadie@contoso.com");
    itemAttachment.Item.ToRecipients.Add("ronnie@contoso.com");
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

## <a name="create-an-email-with-file-and-item-attachments-by-using-ews"></a><span data-ttu-id="1489c-134">Создание сообщения электронной почты с вложениями файлов и элементов с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="1489c-134">Create an email with file and item attachments by using EWS</span></span>
<span data-ttu-id="1489c-135"><a name="bk_createattachews"> </a></span><span class="sxs-lookup"><span data-stu-id="1489c-135"><a name="bk_createattachews"> </a></span></span>

<span data-ttu-id="1489c-136">В приведенном ниже примере кода показано, как использовать операцию [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) для создания сообщения электронной почты с четырьмя вложениями файлов и одним вложением элемента.</span><span class="sxs-lookup"><span data-stu-id="1489c-136">The following code example shows how to use the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation to create an email message with four file attachments and one item attachment.</span></span> <span data-ttu-id="1489c-137">Кроме того, это один из XML-запросов, отправляемых управляемым API EWS при [создании сообщения электронной почты с вложениями файлов и элементов](#bk_createattachewsma).</span><span class="sxs-lookup"><span data-stu-id="1489c-137">This is also one of the XML requests that the EWS Managed API sends when you [create an email with file and item attachments](#bk_createattachewsma).</span></span>
  
<span data-ttu-id="1489c-138">Обратите внимание, что вложение элемента в этом примере создается одновременно с сообщением электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-138">Note that the item attachment in this example is created at the same time as the email message.</span></span> <span data-ttu-id="1489c-139">Чтобы добавить существующее сообщение электронной почты в качестве вложения элемента, ознакомьтесь со статьей [Добавление существующего элемента в новое сообщение электронной почты с помощью сохранитьmimecontent и управляемого API EWS](#bk_addexistingemailewsma).</span><span class="sxs-lookup"><span data-stu-id="1489c-139">To add an existing email message as an item attachment, see [Add an existing item to a new email by using the MimeContent and the EWS Managed API](#bk_addexistingemailewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:Items>
        <t:Message>
          <t:Subject>Message with Attachments</t:Subject>
          <t:Body BodyType="HTML">This message contains four file attachments 
              and one message item attachment.</t:Body>
          <t:Attachments>
            <t:FileAttachment>
              <t:Name>FileAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>SecondAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>VGhpcyBpcyB0aGUgc2Vjb25kIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>ThirdAttachment.jpg</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>nAoAXNIZMVEZs5GKhdzRcLH/9k=</t:Content>
            </t:FileAttachment>
            <t:FileAttachment>
              <t:Name>FourthAttachment.txt</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:IsContactPhoto>false</t:IsContactPhoto>
              <t:Content>obWVudC4=…</t:Content>
            </t:FileAttachment>
            <t:ItemAttachment>
              <t:Name>Attached Message Item</t:Name>
              <t:IsInline>false</t:IsInline>
              <t:Message>
                <t:Subject>Message Item Subject</t:Subject>
                <t:Body BodyType="HTML">Message Item Body</t:Body>
                <t:ToRecipients>
                  <t:Mailbox>
                    <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                  </t:Mailbox>
                  <t:Mailbox>
                    <t:EmailAddress>mack@contoso.com</t:EmailAddress>
                  </t:Mailbox>
                </t:ToRecipients>
              </t:Message>
            </t:ItemAttachment>
          </t:Attachments>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
            <t:Mailbox>
              <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1489c-140">Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) **, которое**указывает, что сообщение и вложения были успешно созданы.</span><span class="sxs-lookup"><span data-stu-id="1489c-140">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email and the attachments were created successfully.</span></span> <span data-ttu-id="1489c-141">В ответ также включен идентификатор [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) нового сообщения и значения [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) для каждого вложения.</span><span class="sxs-lookup"><span data-stu-id="1489c-141">The [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message and the [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values for each of the attachments is also included in the response.</span></span> <span data-ttu-id="1489c-142">Значения некоторых атрибутов были сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="1489c-142">The values of some attributes have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="upV4AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXuktU" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="6ts3NuI=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="gOIZx1I=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="esRan5I=" />
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="t7sU6s=" />
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="XgDCggM=" />
                </t:ItemAttachment>
              </t:Attachments>
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="1489c-143">Чтобы [отправить созданное новое сообщение](how-to-send-email-messages-by-using-ews-in-exchange.md), вызовите операцию [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1489c-143">To [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md), call the [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-the-ews-managed-api"></a><span data-ttu-id="1489c-144">Добавление существующего элемента в новое сообщение электронной почты с помощью Сохранитьmimecontent и управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="1489c-144">Add an existing item to a new email by using the MimeContent and the EWS Managed API</span></span>
<span data-ttu-id="1489c-145"><a name="bk_addexistingemailewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1489c-145"><a name="bk_addexistingemailewsma"> </a></span></span>

<span data-ttu-id="1489c-146">Чтобы добавить существующий элемент в качестве вложения элемента в другой элемент, необходимо создать вложение нового элемента и скопировать содержимое существующего элемента в новый элемент.</span><span class="sxs-lookup"><span data-stu-id="1489c-146">To add an existing item as an item attachment to another item, you need to create a new item attachment and copy the content of the existing item to the new item.</span></span> <span data-ttu-id="1489c-147">Это можно сделать двумя способами:</span><span class="sxs-lookup"><span data-stu-id="1489c-147">There are two ways to do this:</span></span> 
  
1. <span data-ttu-id="1489c-148">Если вы работаете с сообщениями электронной почты, вы можете скопировать значение свойства [сохранитьmimecontent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) из сообщения электронной почты в только что созданный вложенный элемент.</span><span class="sxs-lookup"><span data-stu-id="1489c-148">If you're working with email messages specifically, you can copy the value of the [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) property from the email into the newly created item attachment.</span></span> <span data-ttu-id="1489c-149">Во время этого процесса будут утрачены некоторые свойства, такие как дальнейшие действия и категории, но они прекрасно подходят для стандартных сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-149">You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> 
    
2. <span data-ttu-id="1489c-150">Если требуется полная точность для всех типов элементов, можно выполнить привязку к существующему элементу и скопировать все свойства и расширенные свойства в новое вложение.</span><span class="sxs-lookup"><span data-stu-id="1489c-150">If you need full fidelity for all item types, you can bind to an existing item and copy all the properties and extended properties into the new attachment.</span></span>
    
<span data-ttu-id="1489c-151">В следующем примере кода показан первый способ, в результате чего копируется **сохранитьmimecontent** в новый вложенный элемент.</span><span class="sxs-lookup"><span data-stu-id="1489c-151">The following code example shows the first approach, copying the **MimeContent** into the new item attachment.</span></span> <span data-ttu-id="1489c-152">В приведенном ниже примере показано, как можно изменить код, чтобы использовать второй подход.</span><span class="sxs-lookup"><span data-stu-id="1489c-152">Following this example is a procedure that shows how you can modify the code to use the second approach.</span></span> 
  
<span data-ttu-id="1489c-153">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и что пользователь прошел проверку подлинности на сервере Exchange, а идентификатор **ItemId** является идентификатором [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) элемента, который необходимо присоединить.</span><span class="sxs-lookup"><span data-stu-id="1489c-153">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server, and that the **itemId** is the [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the item to attach.</span></span> 
  
```cs
public static void CreateEmailExistingItem(ExchangeService service, ItemId itemId)
{        
    // This method results in a GetItem call to EWS.
    EmailMessage msgToAttach = EmailMessage.Bind(service,itemId, 
        new PropertySet(ItemSchema.MimeContent, ItemSchema.Subject));
    // Create an email message and set properties on the message.
    EmailMessage message = new EmailMessage(service);
    message.Subject = "Message with Item Attachment (MimeContent)";
    message.Body = "The attachment to this message was created by copying
        the MimeContent from the original message and adding it to a new item attachment.";
    message.ToRecipients.Add("sadie@contoso.com");
    // Add an email message item attachment and set properties on the item.
    ItemAttachment<EmailMessage> itemAttachment = message.Attachments.AddItemAttachment<EmailMessage>();
    itemAttachment.Item.MimeContent = msgToAttach.MimeContent;
    itemAttachment.Name = msgToAttach.Subject;
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

<span data-ttu-id="1489c-154">Чтобы изменить этот пример, чтобы скопировать все свойства существующего элемента в новый вложенный элемент, выполните следующие действия:</span><span class="sxs-lookup"><span data-stu-id="1489c-154">To modify this example to copy each of the properties on the existing item into the new item attachment, do the following:</span></span> 
  
1. <span data-ttu-id="1489c-155">Измените свойство Set так, чтобы оно включало **свойство Set. фирсткласспропертиес** и все необходимые дополнительные свойства или расширенные свойства.</span><span class="sxs-lookup"><span data-stu-id="1489c-155">Change the property set to include **PropertySet.FirstClassProperties** and any additional properties or extended properties you need.</span></span> 
    
  ```cs
  // Add additional properties to the PropertySet.
  EmailMessage msgToAttach = EmailMessage.Bind(service, itemId, new PropertySet(PropertySet.FirstClassProperties));
  ```

2. <span data-ttu-id="1489c-156">Удалите следующую строку, так как свойство **сохранитьmimecontent** не требуется.</span><span class="sxs-lookup"><span data-stu-id="1489c-156">Remove the following line, because you do not need the **MimeContent** property.</span></span> 
    
  ```cs
  itemAttachment.Item.MimeContent = msgToAttach.MimeContent;
  ```

3. <span data-ttu-id="1489c-157">Повторите эту строку для каждого свойства, которое необходимо скопировать из существующего элемента в новое вложение.</span><span class="sxs-lookup"><span data-stu-id="1489c-157">Repeat this line for each property to copy from the existing item to the new attachment.</span></span> <span data-ttu-id="1489c-158">Не копируйте идентификатор **ItemId** в новый вложенный элемент, так как это свойство доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="1489c-158">Do not copy the **ItemId** into the new item attachment because that's a read-only property.</span></span> 
    
  ```cs
  itemAttachment.Item.Subject = msgToAttach.Subject;
  ```

4. <span data-ttu-id="1489c-159">Установите для вложения свойство [PidTagMessageFlags](https://msdn.microsoft.com/library/cc839733.aspx) (0x0E070003), которое требуется **Отправить**.</span><span class="sxs-lookup"><span data-stu-id="1489c-159">Set the [PidTagMessageFlags](https://msdn.microsoft.com/library/cc839733.aspx) (0x0E070003) property on the attachment to **Sent**.</span></span>
    
  ```cs
  ExtendedPropertyDefinition sent = new ExtendedPropertyDefinition(3591, MapiPropertyType.Integer);
  msgToAttach.Item.SetExtendedProperty(sent, "1");
  ```

## <a name="add-an-existing-item-to-a-new-email-by-using-the-mimecontent-and-ews"></a><span data-ttu-id="1489c-160">Добавление существующего элемента в новое сообщение электронной почты с помощью Сохранитьmimecontent и EWS</span><span class="sxs-lookup"><span data-stu-id="1489c-160">Add an existing item to a new email by using the MimeContent and EWS</span></span>
<span data-ttu-id="1489c-161"><a name="bk_addexistingemailews"> </a></span><span class="sxs-lookup"><span data-stu-id="1489c-161"><a name="bk_addexistingemailews"> </a></span></span>

<span data-ttu-id="1489c-162">Существует два способа добавления существующего элемента в новый элемент:</span><span class="sxs-lookup"><span data-stu-id="1489c-162">There are two ways to add an existing item to a new item:</span></span> 
  
1. <span data-ttu-id="1489c-163">Если вы работаете с сообщениями электронной почты, вы можете скопировать значение элемента [сохранитьmimecontent](https://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) из сообщения электронной почты в только что созданный вложенный элемент.</span><span class="sxs-lookup"><span data-stu-id="1489c-163">If you're working with email messages specifically, you can copy the value of the [MimeContent](https://msdn.microsoft.com/library/4f472a08-5653-4c54-ba65-831dfe32f20f%28Office.15%29.aspx) element from the email into the newly created item attachment.</span></span> <span data-ttu-id="1489c-164">Во время этого процесса будут утрачены некоторые свойства, такие как дальнейшие действия и категории, но они прекрасно подходят для стандартных сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-164">You will lose some properties during this process, such as follow up flags and categories, but it works great for standard email messages.</span></span> 
    
2. <span data-ttu-id="1489c-165">Если требуется полная точность для всех типов элементов, можно выполнить привязку к существующему элементу и скопировать все свойства и расширенные свойства в новое вложение.</span><span class="sxs-lookup"><span data-stu-id="1489c-165">If you need full fidelity for all item types, you can bind to an existing item and copy all the properties and extended properties into the new attachment.</span></span>
    
<span data-ttu-id="1489c-166">В приведенном ниже примере кода показано, как использовать элемент **сохранитьmimecontent** для копирования содержимого исходного элемента в значение **сохранитьmimecontent** нового вложения элемента.</span><span class="sxs-lookup"><span data-stu-id="1489c-166">The following code example shows how to use the **MimeContent** element to copy the content of the original item into the **MimeContent** value of the new item attachment.</span></span> <span data-ttu-id="1489c-167">В этом примере используются следующие операции:</span><span class="sxs-lookup"><span data-stu-id="1489c-167">The example uses the following operations:</span></span> 
  
1. <span data-ttu-id="1489c-168">[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) — для получения **сохранитьmimecontent** и [темы](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) сообщения, которое станет вложением элемента в новом сообщении.</span><span class="sxs-lookup"><span data-stu-id="1489c-168">[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) — To get the **MimeContent** and [Subject](https://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) of the message that will become the item attachment on the new message.</span></span> 
    
2. <span data-ttu-id="1489c-169">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) — для создания нового сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-169">[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) — To create the new email message.</span></span> 
    
3. <span data-ttu-id="1489c-170">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)— для создания нового вложения с помощью **сохранитьmimecontent** и **субъекта** , извлеченного операцией **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="1489c-170">[CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx)— To create the new attachment, using the **MimeContent** and **Subject** retrieved by the **GetItem** operation.</span></span> 
    
4. <span data-ttu-id="1489c-171">[SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) — для отправки и сохранения сообщения.</span><span class="sxs-lookup"><span data-stu-id="1489c-171">[SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) — To send and save the message.</span></span> 
    
<span data-ttu-id="1489c-172">Пример начинается с получения **сохранитьmimecontent** и **темы** существующего элемента.</span><span class="sxs-lookup"><span data-stu-id="1489c-172">The example starts by retrieving the **MimeContent** and the **Subject** of the existing item.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:MimeContent" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="jCrTAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1489c-173">Сервер отвечает на запрос **GetItem** с сообщением [жетитемреспонсе](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) **, которое**указывает, что сообщение было успешно получено, а **сохранитьmimecontent** и **Тема** сообщения.</span><span class="sxs-lookup"><span data-stu-id="1489c-173">The server responds to the **GetItem** request with a [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the **MimeContent** and **Subject** of the email.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="944"
                         MinorBuildNumber="11"
                         Version="V2_12"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
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
              <t:MimeContent CharacterSet="UTF-8">tDQe/Eo=…</t:MimeContent>
              <t:ItemId Id="jCrTAAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAZi+7u" />
              <t:Subject>Play tennis?</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="1489c-174">Затем вызовите операцию **CreateItem** , чтобы создать новое сообщение.</span><span class="sxs-lookup"><span data-stu-id="1489c-174">Next, call the **CreateItem** operation to create the new email.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:Items>
        <t:Message>
          <t:Subject>Message with Item Attachment (MimeContent)</t:Subject>
          <t:Body BodyType="HTML">The attachment to this message was created by copying the MimeContent from the original message and adding it to a new item attachment.</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>primary@contoso1000.onmicrosoft.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1489c-175">Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) **, которое**указывает, что сообщение было создано успешно.</span><span class="sxs-lookup"><span data-stu-id="1489c-175">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully.</span></span>
  
<span data-ttu-id="1489c-176">Затем создайте вложение нового элемента, используя **сохранитьmimecontent** и **тему** , извлеченную операцией **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="1489c-176">Next, create the new item attachment by using the **MimeContent** and **Subject** retrieved by the **GetItem** operation.</span></span> <span data-ttu-id="1489c-177">Значение элемента [парентитемид](https://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx) заполняется с помощью значения **ItemId** , возвращаемого в ответе **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="1489c-177">The value of the [ParentItemId](https://msdn.microsoft.com/library/72dc4391-72db-44d2-85d9-4718d59886a7%28Office.15%29.aspx) element is populated by using the **ItemId** value returned in the **CreateItem** response.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateAttachment>
      <m:ParentItemId Id="jDKsAAA=" />
      <m:Attachments>
        <t:ItemAttachment>
          <t:Name>Play tennis?</t:Name>
          <t:IsInline>false</t:IsInline>
          <t:Message>
            <t:MimeContent CharacterSet="UTF-8">tDQe/Eo=…</t:MimeContent>
          </t:Message>
        </t:ItemAttachment>
      </m:Attachments>
    </m:CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1489c-178">Сервер отвечает на запрос **CreateAttachment** с сообщением [креатеаттачментреспонсе](https://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) , равное **ошибке**, которое указывает, что вложение успешно создано, и [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) только что созданного вложения.</span><span class="sxs-lookup"><span data-stu-id="1489c-178">The server responds to the **CreateAttachment** request with a [CreateAttachmentResponse](https://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was created successfully, and the [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) of the newly created attachment.</span></span> 
  
<span data-ttu-id="1489c-179">После создания нового сообщения и присоединения элемента можно [Отправить новое сообщение](how-to-send-email-messages-by-using-ews-in-exchange.md) , вызвав операцию [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1489c-179">Now that the new message has been created, and the item was attached, you can [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md) by calling the [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="jDKsAAA="
                  ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAZi/q/" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1489c-180">Сервер отвечает на запрос **SendItem** с сообщением [сендитемреспонсе](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее, что**сообщение было отправлено успешно.</span><span class="sxs-lookup"><span data-stu-id="1489c-180">The server responds to the **SendItem** request with a [SendItemResponse](https://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was sent successfully.</span></span>
  
## <a name="create-an-email-with-an-inline-attachment-by-using-the-ews-managed-api"></a><span data-ttu-id="1489c-181">Создание сообщения электронной почты со встроенным вложением с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="1489c-181">Create an email with an inline attachment by using the EWS Managed API</span></span>
<span data-ttu-id="1489c-182"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1489c-182"><a name="bk_createinlineattachewsma"> </a></span></span>

<span data-ttu-id="1489c-183">В приведенном ниже примере кода показано, как создать сообщение электронной почты со встроенным вложением, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="1489c-183">The following code example shows how to create an email with an inline attachment by:</span></span>
  
1. <span data-ttu-id="1489c-184">Использование объекта [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) для создания сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-184">Using the [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message.</span></span> 
    
2. <span data-ttu-id="1489c-185">Установка для свойства [EmailMessage. Body](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) HTML-текста, содержащего встроенное вложение.</span><span class="sxs-lookup"><span data-stu-id="1489c-185">Setting the [EmailMessage.Body](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) property to an HTML body that includes an inline attachment.</span></span> 
    
3. <span data-ttu-id="1489c-186">Использование метода [аттачментколлектион. аддфилеаттачмент](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) для добавления вложения в сообщение.</span><span class="sxs-lookup"><span data-stu-id="1489c-186">Using the [AttachmentCollection.AddFileAttachment](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.addfileattachment%28v=exchg.80%29.aspx) method to add the attachment to the message.</span></span> 
    
4. <span data-ttu-id="1489c-187">С помощью метода [EmailMessage. SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) отправьте сообщение получателю и сохраните сообщение в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="1489c-187">Using the [EmailMessage.SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipient and save the message in the Sent Items folder.</span></span> 
    
<span data-ttu-id="1489c-188">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="1489c-188">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static void CreateEmailWithInlineAttachment(ExchangeService service)
{
    // Create the HTML body with the content identifier of the attachment.
    string html = @"<html>
                        <head>
                        </head>
                        <body>
                        <img width=100 height=100 id=""1"" src=""cid:Party.jpg"">
                        </body>
                        </html>";
         
    // Create the email message.
    EmailMessage message = new EmailMessage(service);
    message.Subject = "Inline Attachment";
    message.Body = new MessageBody(BodyType.HTML, html);
    message.ToRecipients.Add("sadie@contoso.com");
    // Add the attachment to the local copy of the email message.
    string file = @"C:\Temp\Party.jpg";
    message.Attachments.AddFileAttachment("Party.jpg", file);
    message.Attachments[0].IsInline = true;
    message.Attachments[0].ContentId = "Party.jpg";
         
    // Send the mail and save a copy in the Sent Items folder.
    // This method results in a CreateItem and SendItem call to EWS.
    message.SendAndSaveCopy();
}
```

## <a name="create-an-email-with-an-inline-attachment-by-using-ews"></a><span data-ttu-id="1489c-189">Создание сообщения электронной почты со встроенным вложением с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="1489c-189">Create an email with an inline attachment by using EWS</span></span>
<span data-ttu-id="1489c-190"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1489c-190"><a name="bk_createinlineattachewsma"> </a></span></span>

<span data-ttu-id="1489c-191">В приведенном ниже примере кода показано, как использовать операцию [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) для создания сообщения электронной почты с вложенным вложенным файлом.</span><span class="sxs-lookup"><span data-stu-id="1489c-191">The following code example shows how to use the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation to create an email message with an inline file attachment.</span></span> <span data-ttu-id="1489c-192">Атрибут **BodyType** элемента [Body](https://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) указывает на то, что содержимое имеет формат HTML и включает источник изображения.</span><span class="sxs-lookup"><span data-stu-id="1489c-192">The **BodyType** attribute of the [Body](https://msdn.microsoft.com/library/7851ea9b-9f87-4adc-a26f-7a27df4a9bca%28Office.15%29.aspx) element indicates that the content is in HTML format and includes the image source.</span></span> <span data-ttu-id="1489c-193">Кроме того, это один из XML-запросов, отправляемых управляемым API EWS при использовании управляемого API EWS для [создания сообщения электронной почты со встроенным вложением](#bk_createinlineattachewsma).</span><span class="sxs-lookup"><span data-stu-id="1489c-193">This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to [create an email with an inline attachment](#bk_createinlineattachewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:Items>
        <t:Message>
          <t:Subject>Inline Attachment</t:Subject>
          <t:Body BodyType="HTML">
            &amp;lt;html&amp;gt;
            &amp;lt;head&amp;gt;
            &amp;lt;/head&amp;gt;
            &amp;lt;body&amp;gt;
            &amp;lt;img width=100 height=100 id="1" src="cid:Party.jpg"&amp;gt;
            &amp;lt;/body&amp;gt;
            &amp;lt;/html&amp;gt;
          </t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1489c-194">В ответ на запрос **CreateItem** сервер отправляет сообщение [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), включающее параметр [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError**, которое указывает, что сообщение было успешно создано, и свойство [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) созданного сообщения.</span><span class="sxs-lookup"><span data-stu-id="1489c-194">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
<span data-ttu-id="1489c-195">Чтобы [отправить созданное новое сообщение](how-to-send-email-messages-by-using-ews-in-exchange.md), вызовите операцию [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1489c-195">To [send this newly created message](how-to-send-email-messages-by-using-ews-in-exchange.md), call the [SendItem](https://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="add-an-attachment-to-an-existing-email-by-using-the-ews-managed-api"></a><span data-ttu-id="1489c-196">Добавление вложения в существующее сообщение электронной почты с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="1489c-196">Add an attachment to an existing email by using the EWS Managed API</span></span>
<span data-ttu-id="1489c-197"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1489c-197"><a name="bk_createinlineattachewsma"> </a></span></span>

<span data-ttu-id="1489c-198">В приведенном ниже примере кода показано, как добавить вложение к существующему письму, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="1489c-198">The following code example shows how to add an attachment to an existing email by:</span></span> 
  
1. <span data-ttu-id="1489c-199">С помощью метода [EmailMessage. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) можно выполнить присоединение к существующему сообщению электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-199">Using the [EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message.</span></span> 
    
2. <span data-ttu-id="1489c-200">Добавление вложенного файла к сообщению с помощью метода **аддфилеаттачмент** .</span><span class="sxs-lookup"><span data-stu-id="1489c-200">Adding a file attachment to the message by using the **AddFileAttachment** method.</span></span> 
    
3. <span data-ttu-id="1489c-201">Сохранение обновлений путем вызова метода [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1489c-201">Saving the updates by calling the [EmailMessage.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method.</span></span> 
    
<span data-ttu-id="1489c-202">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="1489c-202">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```XML
public static void AddAttachmentToExisting(ExchangeService service, ItemId itemId)
{
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId);
    message.Attachments.AddFileAttachment("C:\\temp\\FileAttachment.txt");
    // This method results in a CreateAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="add-an-attachment-to-an-existing-email-by-using-ews"></a><span data-ttu-id="1489c-203">Добавление вложения в существующее сообщение электронной почты с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="1489c-203">Add an attachment to an existing email by using EWS</span></span>
<span data-ttu-id="1489c-204"><a name="bk_createinlineattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1489c-204"><a name="bk_createinlineattachewsma"> </a></span></span>

<span data-ttu-id="1489c-205">В приведенном ниже примере кода показано, как с помощью операции [CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) добавить вложенный файл к существующему сообщению электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1489c-205">The following code example shows how to use the [CreateAttachment](https://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation to add a file attachment to an existing email message.</span></span> <span data-ttu-id="1489c-206">Кроме того, это один из XML-запросов, отправляемых управляемым API EWS, когда вы используете управляемый API EWS, чтобы [Добавить вложение в существующую электронную почту](#bk_createinlineattachewsma).</span><span class="sxs-lookup"><span data-stu-id="1489c-206">This is also one of the XML requests that the EWS Managed API sends when you use the EWS Managed API to [add an attachment to an existing email](#bk_createinlineattachewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateAttachment>
      <m:ParentItemId Id="uqE2AAA=" />
      <m:Attachments>
        <t:FileAttachment>
          <t:Name>FileAttachment.txt</t:Name>
          <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
        </t:FileAttachment>
      </m:Attachments>
    </m:CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1489c-207">Сервер отвечает на запрос **CreateAttachment** с сообщением [креатеаттачментреспонсе](https://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) , равное **ошибке**, которое указывает, что вложение успешно создано, и [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) только что созданного вложения.</span><span class="sxs-lookup"><span data-stu-id="1489c-207">The server responds to the **CreateAttachment** request with a [CreateAttachmentResponse](https://msdn.microsoft.com/library/cf6bd8bb-5317-4a03-bd75-297dd359b5da%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the attachment was created successfully, and the [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) of the newly created attachment.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="yRLhCh8="
                              RootItemId="uqE2AAA="
                              RootItemChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXulcf" />
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:CreateAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="1489c-208">См. также</span><span class="sxs-lookup"><span data-stu-id="1489c-208">See also</span></span>


- [<span data-ttu-id="1489c-209">Вложение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1489c-209">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="1489c-210">Добавление вложений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1489c-210">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="1489c-211">Удаление вложений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1489c-211">Delete attachments by using EWS in Exchange</span></span>](how-to-delete-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="1489c-212">Получение вложений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1489c-212">Get attachments by using EWS in Exchange</span></span>](how-to-get-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="1489c-213">Отправка сообщений электронной почты с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1489c-213">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

