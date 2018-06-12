---
title: Агент транспорта новые и обновленные интерфейсы API в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0a1ad73a-3085-4793-af4d-e4216484c93e
description: Узнайте, какие интерфейсы API, новых или обновленных в Exchange 2013 для агентов транспорта.
ms.openlocfilehash: 0caafaf9629da1066d14357416862a7d67b961aa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761315"
---
# <a name="new-and-updated-transport-agent-apis-in-exchange-2013"></a>Агент транспорта новые и обновленные интерфейсы API в Exchange 2013

Узнайте, какие интерфейсы API, новых или обновленных в Exchange 2013 для агентов транспорта.

**Применимо к:** Exchange Server 2013 
  
В этой статье перечислены типы, которые являются новыми или обновленными в Exchange Server 2013, влияющие на агенты транспорта. Чтобы узнать об изменениях в Exchange 2013, которые влияют на агенты транспорта, видеть [транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md).
  
## <a name="new-types-for-transport-agent-development-in-exchange-2013"></a>Новые типы для разработки агента транспорта в Exchange 2013

Следующие типы являются новыми в Exchange 2013:
  
- [NextHopCategory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.NextHopCategory.aspx)
    
- [RiskLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.RiskLevel.aspx)
    
## <a name="updated-types-for-transport-agent-development-in-exchange-2013"></a>Обновленные типы для передачи агента разработки в Exchange 2013

В Exchange 2013 были обновлены следующие типы:
  
- [ExchangeConfigurationException](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ExchangeConfigurationException.aspx)
    
- [CalendarWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.iCalendar.CalendarWriter.aspx)
    
- [TnefReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefReader.aspx)
    
- [TnefWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.ContentTypes.Tnef.TnefWriter.aspx)
    
- [AddressHeader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.AddressHeader.aspx)
    
- [ComplexHeader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.ComplexHeader.aspx)
    
- [EncodingFlags](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.EncodingFlags.aspx)
    
- [HeaderId](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.HeaderId.aspx)
    
- [HeaderList](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.HeaderList.aspx)
    
- [MimeComplianceStatus](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeComplianceStatus.aspx)
    
- [MimeGroup](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeGroup.aspx)
    
- [MimeNode](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimeNode.aspx)
    
- [MimePart.PartSubtree](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimePart.PartSubtree.aspx)
    
- [MimePart.SubtreeEnumerator](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.MimePart.SubtreeEnumerator.aspx)
    
- [BinHexEncoder](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Mime.Encoders.BinHexEncoder.aspx)
    
- [ConverterStream](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterStream.aspx)
    
- [ConverterWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.ConverterWriter.aspx)
    
- [HtmlReader](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlReader.aspx)
    
- [HtmlTagContext.AttributeCollection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlTagContext.AttributeCollection.aspx)
    
- [HtmlWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlWriter.aspx)
    
- [HtmlWriter](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.TextConverters.HtmlWriter.aspx)
    
- [AcceptedDomainCollection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.AcceptedDomainCollection.aspx)
    
- [EnvelopeRecipientCollection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.EnvelopeRecipientCollection.aspx)
    
- [EnvelopeRecipientCollection.Enumerator](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.EnvelopeRecipientCollection.Enumerator.aspx)
    
- [MailItem](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.MailItem.aspx)
    
- [PermissionCheckResults](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.PermissionCheckResults.aspx)
    
- [ReadOnlyEnvelopeRecipientCollection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.ReadOnlyEnvelopeRecipientCollection.aspx)
    
- [RecipientType](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.RecipientType.aspx)
    
- [RemoteDomainCollection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.RemoteDomainCollection.aspx)
    
- [RoutingAddress](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.RoutingAddress.aspx)
    
- [RoutingDomain](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.RoutingDomain.aspx)
    
- [RoutingHost](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.RoutingHost.aspx)
    
- [RoutingOverride](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.RoutingOverride.aspx)
    
- [AttachmentCollection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.AttachmentCollection.aspx)
    
- [AttachmentCollection.Enumerator](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.AttachmentCollection.Enumerator.aspx)
    
- [EmailRecipientCollection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailRecipientCollection.aspx)
    
- [EmailRecipientCollection.Enumerator](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Email.EmailRecipientCollection.Enumerator.aspx)
    
- [QueuedMessageEventSource](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.QueuedMessageEventSource.aspx)
    
- [RecipientExpansionInfo](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RecipientExpansionInfo.aspx)
    
- [ResolvedMessageEventHandler](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.ResolvedMessageEventHandler.aspx)
    
- [ResolvedMessageEventSource](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.ResolvedMessageEventSource.aspx)
    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    
- [ConnectEventArgs](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.ConnectEventArgs.aspx)
    
- [DisconnectReason](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.DisconnectReason.aspx)
    
- [EhloCommandEventArgs](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.EhloCommandEventArgs.aspx)
    
- [MailCommandEventArgs](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.MailCommandEventArgs.aspx)
    
- [ReceiveEventSource](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.ReceiveEventSource.aspx)
    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    
- [SmtpResponse](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpResponse.aspx)
    
- [SmtpSession](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpSession.aspx)
    
## <a name="see-also"></a>См. также

- [Транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)  
- [Создание агенты транспорта для Exchange 2013](creating-transport-agents-for-exchange-2013.md)  
- [Справочник по агента транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)
    

