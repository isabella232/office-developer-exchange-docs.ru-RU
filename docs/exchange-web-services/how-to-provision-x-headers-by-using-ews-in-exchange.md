---
title: Подготовка заголовков x с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Узнайте, как подготовить x-заголовки для почтового ящика с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 409ddb944bbac7a60242de39cdf7ae13b17cc76a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527770"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a><span data-ttu-id="8f654-103">Подготовка заголовков x с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="8f654-103">Provision x-headers by using EWS in Exchange</span></span>

<span data-ttu-id="8f654-104">Узнайте, как подготовить x-заголовки для почтового ящика с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="8f654-104">Learn how to provision x-headers for a mailbox by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="8f654-105">X-заголовки не являются стандартными заголовками, которые добавляются в коллекцию заголовков электронной почты для передачи информации.</span><span class="sxs-lookup"><span data-stu-id="8f654-105">X-headers are non-standard headers that are added to the header collection of an email to communicate information.</span></span> <span data-ttu-id="8f654-106">Например, Exchange помечает сообщения с помощью заголовка **X-MS-Exchange-Organization-SCL** для указания уровня вероятности нежелательной почты (SCL), назначенного для сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8f654-106">For example, Exchange stamps messages with the **X-MS-Exchange-Organization-SCL** header to indicate the spam confidence level (SCL) attributed to the email.</span></span> <span data-ttu-id="8f654-107">Почтовые клиенты, такие как Outlook, могут использовать эти сведения для определения типа действий, выполняемых с сообщением (например, Outlook может запретить отображение изображений, пока пользователь не выберет действие).</span><span class="sxs-lookup"><span data-stu-id="8f654-107">Email clients like Outlook can use that information to determine what type of action to take on the email (for example, Outlook can prevent images from displaying unless the user takes an action).</span></span> 
  
<span data-ttu-id="8f654-108">Exchange добавляет входящие x заголовков в схему почтовых ящиков в качестве именованного свойства при первом получении сообщения электронной почты с таким x – заголовком.</span><span class="sxs-lookup"><span data-stu-id="8f654-108">Exchange adds incoming x-headers to the mailbox schema as a named property the first time it receives an email with that x-header.</span></span> <span data-ttu-id="8f654-109">Значение x-заголовка не сохраняется в первом сообщении электронной почты; Однако он сохраняется во всех последующих сообщениях электронной почты, которые содержат x-заголовок.</span><span class="sxs-lookup"><span data-stu-id="8f654-109">The x-header value is not saved on that first email; however, it is saved on all subsequent emails that include the x-header.</span></span> <span data-ttu-id="8f654-110">По этой причине приложение должно подготовить x – заголовки, прежде чем ожидать их использования.</span><span class="sxs-lookup"><span data-stu-id="8f654-110">For this reason, your application should provision x-headers before you expect to use them.</span></span> <span data-ttu-id="8f654-111">Сопоставление между именованным свойством и заголовком x происходит при транспортной доставке сообщения электронной почты в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="8f654-111">The mapping between a named property and an x-header occurs in the transport delivery of the email to the mailbox.</span></span> <span data-ttu-id="8f654-112">Это означает, что вам необходимо получать электронную почту через транспортную доставку; Вы не можете просто сохранить электронное письмо с заголовком x для почтового ящика, чтобы создать сопоставление с именованным свойством.</span><span class="sxs-lookup"><span data-stu-id="8f654-112">This means that you need to receive the email via transport delivery; you cannot just save an email that includes the x-header to a mailbox to create the mapping to a named property.</span></span>
  
> [!NOTE]
> <span data-ttu-id="8f654-113">Если вы обнаружите, что x-заголовки не сохраняются, определите, отфильтровывает ли [агент транспорта](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) или [брандмауэр заголовков](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) свои x-заголовки, прежде чем они получится к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="8f654-113">If you find that x-headers aren't being saved, determine whether a [transport agent](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) or [header firewall](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) is filtering out your x-headers before they get to the mailbox.</span></span> <span data-ttu-id="8f654-114">r</span><span class="sxs-lookup"><span data-stu-id="8f654-114">r</span></span>
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a><span data-ttu-id="8f654-115">Подготовка x-заголовка с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="8f654-115">Provision an x-header by using the EWS Managed API</span></span>
<span data-ttu-id="8f654-116"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="8f654-116"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="8f654-117">В приведенном ниже примере кода показано, как использовать метод [EmailMessage. Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) управляемого API EWS для подготовки x-заголовка для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="8f654-117">The following code example shows how to use the EWS Managed API [EmailMessage.Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to provision an x-header for a mailbox.</span></span> <span data-ttu-id="8f654-118">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а целевой почтовый ящик не превысил [квоту для именованных свойств](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8f654-118">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the target mailbox hasn't exceeded the [quota for named properties](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx).</span></span>
  
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

## <a name="provision-an-x-header-by-using-ews"></a><span data-ttu-id="8f654-119">Подготовка x – заголовка с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="8f654-119">Provision an x-header by using EWS</span></span>
<span data-ttu-id="8f654-120"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="8f654-120"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="8f654-121">В приведенном ниже примере кода показано, как использовать операцию [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания и отправки электронной почты для подготовки почтового ящика к заголовку x.</span><span class="sxs-lookup"><span data-stu-id="8f654-121">The following code example shows how to use the EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) operation to create and send an email to provision a mailbox with an x-header.</span></span> <span data-ttu-id="8f654-122">Это XML-запрос, отправляемый управляемым API EWS при [подготовке x-заголовка с помощью управляемого API EWS](#bk_example1).</span><span class="sxs-lookup"><span data-stu-id="8f654-122">This is the XML request that is sent by the EWS Managed API when you [Provision an x-header by using the EWS Managed API](#bk_example1).</span></span>
  
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

## <a name="version-differences"></a><span data-ttu-id="8f654-123">Различия версий</span><span class="sxs-lookup"><span data-stu-id="8f654-123">Version differences</span></span>
<span data-ttu-id="8f654-124"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="8f654-124"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="8f654-125">При первом заполнении x-заголовка в Exchange Online, Exchange Online в составе Office 365 или локальной версии Exchange, начиная с Exchange Server 2010, значение нового пользовательского x-заголовка не будет записано в сохраненное сообщение.</span><span class="sxs-lookup"><span data-stu-id="8f654-125">The first time that you provision an x-header in Exchange Online, Exchange Online as part of Office 365, or an on-premises version of Exchange starting with Exchange Server 2010, the value of a new custom x-header will not be written to the stored message.</span></span> <span data-ttu-id="8f654-126">Это связано с тем, что x-заголовок сначала должен быть сопоставлен с именованным свойством в почтовом ящике пользователя.</span><span class="sxs-lookup"><span data-stu-id="8f654-126">This is because the x-header must first be mapped to a named property in the user's mailbox.</span></span> <span data-ttu-id="8f654-127">Сопоставление выполняется при первом запросе на добавление именованных свойств.</span><span class="sxs-lookup"><span data-stu-id="8f654-127">The mapping occurs upon the first request to add the named properties.</span></span> <span data-ttu-id="8f654-128">Когда происходит последующий запрос на создание именованного свойства, свойство и значение хранятся в сообщении.</span><span class="sxs-lookup"><span data-stu-id="8f654-128">When a subsequent request to create the named property occurs, the property and value are stored on the message.</span></span> <span data-ttu-id="8f654-129">В Exchange 2007 при первом заголовке x-заголовка в базу данных почтовых ящиков создается сопоставление для x-заголовка для именованного свойства в базе данных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="8f654-129">In Exchange 2007, the first time an x-header is written to a mailbox database, a mapping is created for the x-header to a named property across the mailbox database.</span></span> <span data-ttu-id="8f654-130">При последующем запросе на создание именованного свойства заголовок x обрабатывается и сохраняется для любого почтового ящика в базе данных Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="8f654-130">When a subsequent request to create the named property occurs, the x-header is processed and stored for any mailbox in the Exchange 2007 database.</span></span>
  
## <a name="next-steps"></a><span data-ttu-id="8f654-131">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="8f654-131">Next steps</span></span>
<span data-ttu-id="8f654-132"><a name="bk_example1"> </a></span><span class="sxs-lookup"><span data-stu-id="8f654-132"><a name="bk_example1"> </a></span></span>

<span data-ttu-id="8f654-133">В этой статье показано, как подготовить x – заголовок для одного почтового ящика, отправив пользователю сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8f654-133">This article shows you how to provision an x-header for a single mailbox by sending an email to a user.</span></span> <span data-ttu-id="8f654-134">Вы также можете подготовить x – заголовок для многих пользователей, [отправив пакетную почту в список получателей](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) в Организации вызывающего абонента.</span><span class="sxs-lookup"><span data-stu-id="8f654-134">You can also provision an x-header for many users by [sending a batch email to a list of recipients](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) in the caller's organization.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8f654-135">См. также</span><span class="sxs-lookup"><span data-stu-id="8f654-135">See also</span></span>


- [<span data-ttu-id="8f654-136">Свойства и расширенные свойства в веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="8f654-136">Properties and extended properties in EWS in Exchange</span></span>](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [<span data-ttu-id="8f654-137">Exchange 2013: подготовка настраиваемых X – заголовков программным способом</span><span class="sxs-lookup"><span data-stu-id="8f654-137">Exchange 2013: Provision custom X-headers programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [<span data-ttu-id="8f654-138">Именованные свойства, X – заголовки и</span><span class="sxs-lookup"><span data-stu-id="8f654-138">Named Properties, X-Headers, and You</span></span>](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [<span data-ttu-id="8f654-139">Именованные свойства, Round 2: что находится впереди</span><span class="sxs-lookup"><span data-stu-id="8f654-139">Named Properties, Round 2: What lies Ahead</span></span>](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [<span data-ttu-id="8f654-140">Брандмауэр заголовков</span><span class="sxs-lookup"><span data-stu-id="8f654-140">Header Firewall</span></span>](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [<span data-ttu-id="8f654-141">EWS, MIME и отсутствующие заголовки сообщений Интернета</span><span class="sxs-lookup"><span data-stu-id="8f654-141">EWS, MIME, and the missing Internet message headers</span></span>](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [<span data-ttu-id="8f654-142">Обработка сообщений электронной почты в пакетах с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="8f654-142">Process email messages in batches by using EWS in Exchange</span></span>](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

