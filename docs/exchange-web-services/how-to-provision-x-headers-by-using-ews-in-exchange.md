---
title: Подготовка заголовков x с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 45a99a14-a85f-47f8-af48-18eb6c6cc230
description: Узнайте, как подготовить x-заголовки для почтового ящика с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: de572764921da432cfa203b3dcf166d1d34dd0cd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761099"
---
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Подготовка заголовков x с помощью EWS в Exchange

Узнайте, как подготовить x-заголовки для почтового ящика с помощью управляемого API EWS или EWS в Exchange.
  
X-заголовки не являются стандартными заголовками, которые добавляются в коллекцию заголовков электронной почты для передачи информации. Например, Exchange помечает сообщения с помощью заголовка **X-MS-Exchange-Organization-SCL** для указания уровня вероятности нежелательной почты (SCL), назначенного для сообщения электронной почты. Почтовые клиенты, такие как Outlook, могут использовать эти сведения для определения типа действий, выполняемых с сообщением (например, Outlook может запретить отображение изображений, пока пользователь не выберет действие). 
  
Exchange добавляет входящие x заголовков в схему почтовых ящиков в качестве именованного свойства при первом получении сообщения электронной почты с таким x – заголовком. Значение x-заголовка не сохраняется в первом сообщении электронной почты; Однако он сохраняется во всех последующих сообщениях электронной почты, которые содержат x-заголовок. По этой причине приложение должно подготовить x – заголовки, прежде чем ожидать их использования. Сопоставление между именованным свойством и заголовком x происходит при транспортной доставке сообщения электронной почты в почтовый ящик. Это означает, что вам необходимо получать электронную почту через транспортную доставку; Вы не можете просто сохранить электронное письмо с заголовком x для почтового ящика, чтобы создать сопоставление с именованным свойством.
  
> [!NOTE]
> Если вы обнаружите, что x-заголовки не сохраняются, определите, отфильтровывает ли [агент транспорта](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) или [брандмауэр заголовков](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx) свои x-заголовки, прежде чем они получится к почтовому ящику. 
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Подготовка x-заголовка с помощью управляемого API EWS
<a name="bk_example1"> </a>

В приведенном ниже примере кода показано, как использовать метод [EmailMessage. Send](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) управляемого API EWS для подготовки x-заголовка для почтового ящика. В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а целевой почтовый ящик не превысил [квоту для именованных свойств](http://technet.microsoft.com/en-us/library/bb851492%28v=EXCHG.80%29.aspx).
  
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

## <a name="provision-an-x-header-by-using-ews"></a>Подготовка x – заголовка с помощью EWS
<a name="bk_example1"> </a>

В приведенном ниже примере кода показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания и отправки электронной почты для подготовки почтового ящика к заголовку x. Это XML-запрос, отправляемый управляемым API EWS при [подготовке x-заголовка с помощью управляемого API EWS](#bk_example1).
  
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

## <a name="version-differences"></a>Различия версий
<a name="bk_example1"> </a>

При первом заполнении x-заголовка в Exchange Online, Exchange Online в составе Office 365 или локальной версии Exchange, начиная с Exchange Server 2010, значение нового пользовательского x-заголовка не будет записано в сохраненное сообщение. Это связано с тем, что x-заголовок сначала должен быть сопоставлен с именованным свойством в почтовом ящике пользователя. Сопоставление выполняется при первом запросе на добавление именованных свойств. Когда происходит последующий запрос на создание именованного свойства, свойство и значение хранятся в сообщении. В Exchange 2007 при первом заголовке x-заголовка в базу данных почтовых ящиков создается сопоставление для x-заголовка для именованного свойства в базе данных почтовых ящиков. При последующем запросе на создание именованного свойства заголовок x обрабатывается и сохраняется для любого почтового ящика в базе данных Exchange 2007.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_example1"> </a>

В этой статье показано, как подготовить x – заголовок для одного почтового ящика, отправив пользователю сообщение электронной почты. Вы также можете подготовить x – заголовок для многих пользователей, [отправив пакетную почту в список получателей](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) в Организации вызывающего абонента. 
  
## <a name="see-also"></a>См. также


- [Свойства и расширенные свойства в веб-службах Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013: подготовка настраиваемых X – заголовков программным способом](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Именованные свойства, X – заголовки и](http://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Именованные свойства, Round 2: что находится впереди](http://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Брандмауэр заголовков](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx)
    
- [EWS, MIME и отсутствующие заголовки сообщений Интернета](http://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Обработка сообщений электронной почты в пакетах с помощью EWS в Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

