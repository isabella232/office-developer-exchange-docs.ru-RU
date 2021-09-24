---
title: Подготовка x-headers с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Узнайте, как создать x-headers для почтового ящика с помощью управляемого API или EWS EWS в Exchange.
ms.openlocfilehash: e60092e0d40d5815cdf3fd4ed588e2f74978c245
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521118"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Подготовка x-headers с помощью EWS в Exchange

Узнайте, как создать x-headers для почтового ящика с помощью управляемого API или EWS EWS в Exchange.
  
X-headers — это нестандартные загонщики, которые добавляются в коллекцию загонщиков электронной почты для связи с информацией. Например, Exchange сообщения с загонщиком **X-MS-Exchange-Organization-SCL,** чтобы указать уровень доверия нежелательной почты (SCL), приписываемого электронной почте. Клиенты электронной почты, такие как Outlook, могут использовать эту информацию для определения типа действий, которые необходимо принять для электронной почты (например, Outlook могут запретить отображение изображений, если пользователь не принимает меры). 
  
Exchange добавляет входящие x-headers в схему почтовых ящиков в качестве имени свойства при первом приеме электронной почты с этим x-header. Значение x-header не сохранено на первом сообщении электронной почты; однако он сохранен на всех последующих сообщениях электронной почты, включая x-header. По этой причине приложение должно закавыкать x-headers, прежде чем вы ожидаете их использовать. Сопоставление между именем свойства и x-header происходит при доставке электронной почты в почтовый ящик. Это означает, что вам необходимо получать сообщение электронной почты с помощью транспортной доставки; вы не можете просто сохранить электронную почту, включаемую x-header в почтовый ящик, чтобы создать сопоставление с именем свойства.
  
> [!NOTE]
> Если вы найдете, что x-headers не сохраняются, определите, отфильтровывал ли агент транспорта или брандмауэр заготавлителей, прежде чем они доберются до почтового ящика. [](https://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) [](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx) r
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Подготовка x-header с помощью управляемого API EWS
<a name="bk_example1"> </a>

В следующем примере кода показано, как использовать метод EWS Managed API [EmailMessage.Send](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) для обеспечения x-header для почтового ящика. В этом примере предполагается, что служба является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и что целевой почтовый ящик не превысил квоту для  [именных свойств.](https://technet.microsoft.com/library/bb851492%28v=EXCHG.80%29.aspx)
  
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

## <a name="provision-an-x-header-by-using-ews"></a>Подготовка x-header с помощью EWS
<a name="bk_example1"> </a>

В следующем примере кода показано, как использовать операцию EWS [CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания и отправки электронной почты для обеспечения почтового ящика с помощью x-header. Это XML-запрос, который отправляется управляемым API EWS при предоставлении X-header с помощью [управляемого API EWS.](#bk_example1)
  
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

## <a name="version-differences"></a>Различия версий
<a name="bk_example1"> </a>

При первом предоставлении x-header в Exchange Online, Exchange Online в Office 365 или локальной версии Exchange начиная с Exchange Server 2010 г., значение нового настраиваемого x-header не будет записано в сохраненное сообщение. Это потому, что x-header необходимо сначала соеденить к именитого свойства в почтовом ящике пользователя. Сопоставление происходит при первом запросе на добавление именных свойств. При последующем запросе на создание имени имени свойства свойство и значение сохраняются в сообщении. В Exchange 2007 г. при первом написании x-header в базу данных почтовых ящиков создается сопоставление для x-header с именем свойства в базе данных почтовых ящиков. При последующем запросе на создание имени свойства x-header обрабатывается и хранится для любого почтового ящика в базе данных Exchange 2007 г.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_example1"> </a>

В этой статье показано, как разместить x-header для одного почтового ящика, отправив сообщение электронной почты пользователю. Вы также можете разозвать x-header для многих пользователей, отправив пакетное сообщение электронной почты в список получателей в организации вызываемого пользователя. [](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) 
  
## <a name="see-also"></a>См. также


- [Свойства и расширенные свойства в веб-службах Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013 г. Подготовка настраиваемого X-headers программным образом](https://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Named Properties, X-Headers и You](https://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Named Properties, Round 2: What lies Ahead](https://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Брандмауэр header](https://technet.microsoft.com/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS, MIME и отсутствующие заглавные сообщения в Интернете](https://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Обработка сообщений электронной почты пакетами с помощью EWS в Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

