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
# <a name="provision-x-headers-by-using-ews-in-exchange"></a>Подготовка к работе x заголовков с помощью веб-служб Exchange в Exchange

Узнайте, как подготовить x заголовков для почтового ящика с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
X-заголовков, нестандартный заголовки, добавляемые в коллекцию заголовок сообщения электронной почты, обмена данными. Например обмен сообщениями пометок с заголовка **X-MS-Exchange-организации-вероятности нежелательной почты** для указания уровень вероятности нежелательной почты (SCL) атрибутами, сообщение электронной почты. Отправить по электронной почте клиенты, как Outlook можно использовать эти сведения, чтобы определить, какой тип действие, которое выполняется на сообщение электронной почты (например, Outlook можно запретить изображения отображение Если пользователь выполняет действие). 
  
Exchange добавляет входящих x заголовков в схеме почтового ящика в качестве именованного свойства первый раз, она получает сообщение электронной почты с x заголовка. Значение x заголовка не сохраняется на первом сообщение электронной почты; Тем не менее он сохраняется на всех последующих по электронной почте, включая x заголовка. По этой причине приложение следует подготовить x заголовков перед предполагается, что их использования. Сопоставление между именованного свойства и x заголовка используется в транспорта доставки электронной почты в почтовый ящик. Это означает, что необходимо получать электронную почту с помощью доставки транспорта; просто не могут сохранять сообщения электронной почты, которая включает в себя x заголовка в почтовый ящик создается сопоставление для именованного свойства.
  
> [!NOTE]
> Если не сохраняются x заголовков, определите, ли [агента транспорта](http://code.msdn.microsoft.com/Exchange-2013-Build-an-32f62f5a) или [заголовок брандмауэра](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx) фильтрации x заголовков прежде чем они станут к почтовому ящику. 
  
## <a name="provision-an-x-header-by-using-the-ews-managed-api"></a>Подготовка x заголовка с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_example1"> </a>

В следующем примере кода показано, как использовать метод управляемый API EWS [EmailMessage.Send](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) для подготовки x заголовка для почтового ящика. В этом примере предполагается, что **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и что целевой почтовый ящик не превышении [квот для именованных свойств](http://technet.microsoft.com/en-us/library/bb851492%28v=EXCHG.80%29.aspx).
  
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

## <a name="provision-an-x-header-by-using-ews"></a>Подготовка x заголовка с помощью веб-служб Exchange
<a name="bk_example1"> </a>

В следующем примере кода показано, как использовать операцию EWS [CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) для создания и отправки сообщения электронной почты для подготовки почтового ящика с x заголовка. Это XML-запрос, отправляемого управляемый API EWS при вы [Provision x заголовка с помощью управляемого интерфейса API веб-служб Exchange](#bk_example1).
  
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

Первый раз, Подготовка x заголовка в Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange Server 2010, значение нового пользовательского x заголовка не будут записываться в сохраненных сообщение. Это x заголовка сначала должен быть сопоставлен именованное свойство в почтовом ящике пользователя. Сопоставление осуществляется при первом запросе Добавление именованного свойства. В случае последующего запроса для создания именованного свойства свойства и значения, хранятся в окне сообщения. В Exchange 2007, при первом x заголовка записывается в базу данных почтовых ящиков, сопоставление будет создан x заголовка для именованного свойства для базы данных почтовых ящиков. В случае последующего запроса для создания именованного свойства x заголовка обрабатываются и сохраняются для любого почтового ящика в базе данных Exchange 2007.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_example1"> </a>

В этой статье показано, как подготовить x заголовка для одного почтового ящика, отправив сообщение электронной почты для пользователя. Также вы можете подготовить x заголовка для нескольких пользователей, [отправляет сообщения электронной почты пакета список получателей](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md) в организации вызывающего абонента. 
  
## <a name="see-also"></a>См. также


- [Свойства и расширенные свойства в веб-службах Exchange](properties-and-extended-properties-in-ews-in-exchange.md)
    
- [Exchange 2013: Подготовка пользовательских X-заголовков программными средствами](http://code.msdn.microsoft.com/exchange/Exchange-2013-Provision-d4ef5719)
    
- [Именованные свойства, X-заголовков и](http://blogs.technet.com/b/exchange/archive/2009/04/06/3407221.aspx)
    
- [Именованные свойства Round 2: Что находится издержек](http://blogs.technet.com/b/exchange/archive/2009/06/12/3407672.aspx)
    
- [Заголовок брандмауэра](http://technet.microsoft.com/en-us/library/bb232136%28v=exchg.150%29.aspx)
    
- [Веб-служб Exchange, MIME и отсутствующие заголовков сообщений Интернета](http://msdn.microsoft.com/library/office/hh545614%28v=exchg.140%29.aspx)
    
- [Обрабатывать сообщения электронной почты в пакетах с помощью веб-служб Exchange в Exchange](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    

