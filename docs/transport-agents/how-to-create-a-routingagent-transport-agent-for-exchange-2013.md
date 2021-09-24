---
title: Создание транспортного агента RoutingAgent для Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Узнайте, как создать настраиваемый транспортный агент RoutingAgent для использования с Exchange 2013 г.
ms.openlocfilehash: 70dbfc3c25e18195bb4b42fd3e750da11b0423d6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534176"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Создание транспортного агента RoutingAgent для Exchange 2013 г.

Узнайте, как создать настраиваемый транспортный агент RoutingAgent для использования с Exchange 2013 г.
  
**Применяется к:** Exchange Server 2013 г.
  
Связанные фрагменты кода и примеры приложений:

- [Exchange 2013 г.: Создание транспортного агента для ведения журнала пропускной способности](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
Классы [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) и [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) являются базовыми классами для транспортных агентов, предназначенных для работы на транспортной службе на сервере почтовых ящиков Exchange Server 2013 г. Класс [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) предоставляет события, перечисленные в следующей таблице, для которых можно реализовать обработчики в транспортном агенте RoutingAgent. 
  
**Таблица 1. События класса RoutingAgent**

|**Event**|**Описание**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Происходит после того, как сервер выполняет преобразование контента, если это необходимо.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Происходит после того, как все получатели сообщения будут устранены и до того, как будет определена маршрутивка.  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Происходит после того, как сервер передает сообщение в следующий переход и при необходимости выполняет преобразование контента. Сервер может использовать больше ресурсов для обработки каждого сообщения в событии [OnRoutedMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) чем событие [OnSubmittedMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) так как сервер выполнит любое необходимое преобразование контента и определит следующий переход в маршрут сообщения перед выполнением кода в обработнике событий [OnRoutedMessage.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Происходит после того, как сообщение будет отобрано из очереди отправки. Используйте [событие OnSubmittedMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) если транспортному агенту RoutingAgent не требуется преобразование контента, разрешенные получатели или данные маршрутирования.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Создание настраиваемой транспортной агент RoutingAgent

Следующая процедура описывает создание настраиваемой транспортной агент RoutingAgent. 
  
### <a name="to-create-the-transport-agent"></a>Создание транспортного агента

1. Добавьте ссылки на пространства имен.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Эти пространства имен можно найти на Exchange сервере. Добавив ссылку на эти пространства имен, вы сможете получить доступ к участникам [RoutingAgent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) а также к другим классам, используемым в Exchange [2013 г. Сборка](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) образца транспортного агента для ведения журнала пропускной способности. 
    
2. Реализация полученного класса для [класса RoutingAgentFactory.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   Этот код мгновенно выводится из полученного класса и переопределяет метод **CreateAgent** для создания экземпляра нового настраиваемого агента. Дополнительные методы, такие как **Close,** также могут быть переопределены в этом классе для выполнения настраиваемого кода. 
    
3. Определите агента.
    
   ```cs
      public class BandwidthLogger : RoutingAgent
      {
          // Your custom code goes here
          public BandwidthLogger(SmtpServer server)
          {
              Debug.WriteLine(logPrefix + "Agent constructor");
              this.server = server;
              this.OnSubmittedMessage += SubmittedMessage;
              this.OnRoutedMessage += RoutedMessage;
          }
      }
  
   ```

   После определения класса агента можно добавить настраиваемые функциональные возможности. В этом примере два события [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)перенаправляются в настраиваемые обработчики событий. 
    
## <a name="see-also"></a>См. также

- [Концепции транспортного агента в Exchange 2013 г.](transport-agent-concepts-in-exchange-2013.md)    
- [Ссылка агента транспорта на Exchange 2013 г.](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

