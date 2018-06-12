---
title: Подготовка к работе x заголовков с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Узнайте, как подготовить x заголовков для почтового ящика с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: de572764921da432cfa203b3dcf166d1d34dd0cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761099"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a><span data-ttu-id="f6f70-103">Подготовка к работе x заголовков с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f6f70-103">Provision x-headers by using EWS in Exchange</span></span>

<span data-ttu-id="f6f70-104">Узнайте, как подготовить x заголовков для почтового ящика с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6f70-104">Learn how to provision x-headers for a mailbox by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="f6f70-105">X-заголовков, нестандартный заголовки, добавляемые в коллекцию заголовок сообщения электронной почты, обмена данными.</span><span class="sxs-lookup"><span data-stu-id="f6f70-105">X-headers are non-standard headers that are added to the header collection of an email to communicate information.</span></span> <span data-ttu-id="f6f70-106">Например обмен сообщениями пометок с заголовка **X-MS-Exchange-организации-вероятности нежелательной почты** для указания уровень вероятности нежелательной почты (SCL) атрибутами, сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="f6f70-106">For example, Exchange stamps messages with the **X-MS-Exchange-Organization-SCL** header to indicate the spam confidence level (SCL) attributed to the email.</span></span> <span data-ttu-id="f6f70-107">Отправить по электронной почте клиенты, как Outlook можно использовать эти сведения, чтобы определить, какой тип действие, которое выполняется на сообщение электронной почты (например, Outlook можно запретить изображения отображение Если пользователь выполняет действие).</span><span class="sxs-lookup"><span data-stu-id="f6f70-107">Email clients like Outlook can use that information to determine what type of action to take on the email (for example, Outlook can prevent images from displaying unless the user takes an action).</span></span> 
  
<span data-ttu-id="f6f70-108">Exchange добавляет входящих x заголовков в схеме почтового ящика в качестве именованного свойства первый раз, она получает сообщение электронной почты с x заголовка.</span><span class="sxs-lookup"><span data-stu-id="f6f70-108">Exchange adds incoming x-headers to the mailbox schema as a named property the first time it receives an email with that x-header.</span></span> <span data-ttu-id="f6f70-109">Значение x заголовка не сохраняется на первом сообщение электронной почты; Тем не менее он сохраняется на всех последующих по электронной почте, включая x заголовка.</span><span class="sxs-lookup"><span data-stu-id="f6f70-109">The x-header value is not saved on that first email; however, it is saved on all subsequent emails that include the x-header.</span></span> <span data-ttu-id="f6f70-110">По этой причине приложение следует подготовить x заголовков перед предполагается, что их использования.</span><span class="sxs-lookup"><span data-stu-id="f6f70-110">For this reason, your application should provision x-headers before you expect to use them.</span></span> <span data-ttu-id="f6f70-111">Сопоставление между именованного свойства и x заголовка используется в транспорта доставки электронной почты в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="f6f70-111">The mapping between a named property and an x-header occurs in the transport delivery of the email to the mailbox.</span></span> <span data-ttu-id="f6f70-112">Это означает, что необходимо получать электронную почту с помощью доставки транспорта; просто не могут сохранять сообщения электронной почты, которая включает в себя x заголовка в почтовый ящик создается сопоставление для именованного свойства.</span><span class="sxs-lookup"><span data-stu-id="f6f70-112">This means that you need to receive the email via transport delivery; you cannot just save an email that includes the x-header to a mailbox to create the mapping to a named property.</span></span>
  
> [!NOTE]
> <span data-ttu-id="f6f70-113">Если не сохраняются x заголовков, определите, ли [агента транспорта](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) или [заголовок брандмауэра](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx) фильтрации x заголовков прежде чем они станут к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="f6f70-113">If you find that x-headers aren't being saved, determine whether a [transport agent](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) or [header firewall](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx) is filtering out your x-headers before they get to the mailbox.</span></span> 
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a><span data-ttu-id="f6f70-114">Подготовка x заголовка с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="f6f70-114">Provision an x-header by using the EWS Managed API</span></span>
<span data-ttu-id="f6f70-115"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="f6f70-115"></span></span>

<span data-ttu-id="f6f70-116">В следующем примере кода показано, как использовать метод управляемый API EWS [EmailMessage.Send](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) для подготовки x заголовка для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f6f70-116">The following code example shows how to use the EWS Managed API [EmailMessage.Send](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to provision an x-header for a mailbox.</span></span> <span data-ttu-id="f6f70-117">В этом примере предполагается, что **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и что целевой почтовый ящик не превышении [квот для именованных свойств](http://technet.microsoft.com/en-us/library/bb851492%28v=EXCHG.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f6f70-117">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the target mailbox hasn't exceeded the [quota for named properties](http://technet.microsoft.com/en-us/library/bb851492%28v=EXCHG.80%29.aspx).</span></span>
  
```cs
private static void ProvisionCustomXHeaderByEmail(ExchangeService service)
{
    // Create a definition for an extended property that will represent a custom x-header. X-headers must be created in the
    // InternetHeaders property set. The x-header name must match the name of the x-header sent in the subsequent emails so
    // the x-header and value are saved on the email.
    ExtendedPropertyDefinition xExperimentalHeader = new ExtendedPropertyDefinition(DefaultExtendedPropertySet.InternetHeaders,
                                                                                            "X-Experimental",
                                                                                            MapiPropertyType.String);
    // Create an item that is used to provision the custom x-header.
    EmailMessage email = new EmailMessage(service);
    email.ToRecipients.Add("user@contoso.com");
    email.SetExtendedProperty(xExperimentalHeader, "Provision X-Experimental Internet message header");
    try
    {
        // The mapping of the named property happens in transport delivery.
        email.Send();
        if (service.ServerInfo.MajorVersion == 12)
        {
            Console.WriteLine("Provisioned the X-Experimental across the mailbox database that hosts the user's mailbox.");
        }
        else // For versions of Exchange starting with Exchange 2010
        {
            Console.WriteLine("Provisioned the X-Experimental for the user's mailbox. You will need to run this " +
                                "for each mailbox that needs to process this x-header.");
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Error: {0}", ex.Message);
    }
}
```

## <a name="provision-an-x-header-by-using-ews"></a><span data-ttu-id="f6f70-118">Подготовка x заголовка с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="f6f70-118">Provision an x-header by using EWS</span></span>
<span data-ttu-id="f6f70-119"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="f6f70-119"></span></span>

<span data-ttu-id="f6f70-120">В следующем примере кода показано, как использовать операцию EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания и отправки сообщения электронной почты для подготовки почтового ящика с x заголовка.</span><span class="sxs-lookup"><span data-stu-id="f6f70-120">The following code example shows how to use the EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) operation to create and send an email to provision a mailbox with an x-header.</span></span> <span data-ttu-id="f6f70-121">Это XML-запрос, отправляемого управляемый API EWS при вы [Provision x заголовка с помощью управляемого интерфейса API веб-служб Exchange](#bk_example1).</span><span class="sxs-lookup"><span data-stu-id="f6f70-121">This is the XML request that is sent by the EWS Managed API when you [Provision an x-header by using the EWS Managed API](#bk_example1).</span></span>
  
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
    <m:CreateItem MessageDisposition="SendOnly">
      <m:Items>
        <t:Message>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI DistinguishedPropertySetId="InternetHeaders"
                                PropertyName="X-Experimental"
                                PropertyType="String" />
            <t:Value>Provision X-Experimental Internet message header</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>user@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

## <a name="version-differences"></a><span data-ttu-id="f6f70-122">Различия версий</span><span class="sxs-lookup"><span data-stu-id="f6f70-122">Version differences</span></span>
<span data-ttu-id="f6f70-123"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="f6f70-123"></span></span>

<span data-ttu-id="f6f70-124">Первый раз, Подготовка x заголовка в Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange Server 2010, значение нового пользовательского x заголовка не будут записываться в сохраненных сообщение.</span><span class="sxs-lookup"><span data-stu-id="f6f70-124">The first time that you provision an x-header in Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2010, the value of a new custom x-header will not be written to the stored message.</span></span> <span data-ttu-id="f6f70-125">Это x заголовка сначала должен быть сопоставлен именованное свойство в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6f70-125">This is because the x-header must first be mapped to a named property in the user's mailbox.</span></span> <span data-ttu-id="f6f70-126">Сопоставление осуществляется при первом запросе Добавление именованного свойства.</span><span class="sxs-lookup"><span data-stu-id="f6f70-126">The mapping occurs upon the first request to add the named properties.</span></span> <span data-ttu-id="f6f70-127">В случае последующего запроса для создания именованного свойства свойства и значения, хранятся в окне сообщения.</span><span class="sxs-lookup"><span data-stu-id="f6f70-127">When a subsequent request to create the named property occurs, the property and value are stored on the message.</span></span> <span data-ttu-id="f6f70-128">В Exchange 2007, при первом x заголовка записывается в базу данных почтовых ящиков, сопоставление будет создан x заголовка для именованного свойства для базы данных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="f6f70-128">In Exchange 2007, the first time an x-header is written to a mailbox database, a mapping is created for the x-header to a named property across the mailbox database.</span></span> <span data-ttu-id="f6f70-129">В случае последующего запроса для создания именованного свойства x заголовка обрабатываются и сохраняются для любого почтового ящика в базе данных Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="f6f70-129">When a subsequent request to create the named property occurs, the x-header is processed and stored for any mailbox in the Exchange 2007 database.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="f6f70-130">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="f6f70-130">Next steps</span></span>
<span data-ttu-id="f6f70-131"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="f6f70-131"></span></span>

<span data-ttu-id="f6f70-132">В этой статье показано, как подготовить x заголовка для одного почтового ящика, отправив сообщение электронной почты для пользователя.</span><span class="sxs-lookup"><span data-stu-id="f6f70-132">This article shows you how to provision an x-header for a single mailbox by sending an email to a user.</span></span> <span data-ttu-id="f6f70-133">Также вы можете подготовить x заголовка для нескольких пользователей, [отправляет сообщения электронной почты пакета список получателей](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) в организации вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="f6f70-133">You can also provision an x-header for many users by [sending a batch email to a list of recipients](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) in the caller's organization.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="f6f70-134">См. также</span><span class="sxs-lookup"><span data-stu-id="f6f70-134">See also</span></span>


- [<span data-ttu-id="f6f70-135">Свойства и расширенные свойства в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="f6f70-135">Properties and extended properties in EWS in Exchange</span></span>](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [<span data-ttu-id="f6f70-136">Exchange 2013: Подготовка пользовательских X-заголовков программными средствами</span><span class="sxs-lookup"><span data-stu-id="f6f70-136">Exchange 2013: Provision custom X-headers programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [<span data-ttu-id="f6f70-137">Именованные свойства, X-заголовков и</span><span class="sxs-lookup"><span data-stu-id="f6f70-137">Named Properties, X-Headers, and You</span></span>](http://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [<span data-ttu-id="f6f70-138">Именованные свойства Round 2: Что находится издержек</span><span class="sxs-lookup"><span data-stu-id="f6f70-138">Named Properties, Round 2: What lies Ahead</span></span>](http://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [<span data-ttu-id="f6f70-139">Заголовок брандмауэра</span><span class="sxs-lookup"><span data-stu-id="f6f70-139">Header Firewall</span></span>](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="f6f70-140">Веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета</span><span class="sxs-lookup"><span data-stu-id="f6f70-140">EWS, MIME, and the missing Internet message headers</span></span>](http://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [<span data-ttu-id="f6f70-141">Обрабатывать сообщения электронной почты в пакетах с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f6f70-141">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

