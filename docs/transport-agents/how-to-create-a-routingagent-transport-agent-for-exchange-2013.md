---
title: Создание агента транспорта RoutingAgent для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Узнайте, как создать настраиваемые агента транспорта RoutingAgent для использования с Exchange 2013.
ms.openlocfilehash: d07f68494acd26940a4837bbbfc7a0505114bd20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761299"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Создание агента транспорта RoutingAgent для Exchange 2013

Узнайте, как создать настраиваемые агента транспорта RoutingAgent для использования с Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
Связанные фрагменты кода и примеры приложений:

- [Exchange 2013: Создание агента транспорта пропускной способности ведения журнала](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
Классы, [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) и [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) , базовые классы для агенты транспорта, которые предназначены для выполнения в службе транспорта на сервере почтовых ящиков Exchange Server 2013. Класс [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) предоставляет события, указанные в следующей таблице, для которого может внедрить обработчики в вашей RoutingAgent агента транспорта. 
  
**В таблице 1. События класса RoutingAgent**

|**Событие**|**Описание**|
|:-----|:-----|
|[OnCategorizedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Возникает после сервер выполняет преобразование содержимого, если это необходимо.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Возникает после устранения возможных всех получателей сообщения и перед маршрутизацией определяется.  <br/> |
|[OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Возникает после сервер перенаправляет сообщение до следующего прыжка и выполняет преобразование содержимого при необходимости. Сервер может использовать дополнительные ресурсы для обработки каждого сообщения в событии [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) чем событие [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , так как сервер будет выполнять любые необходимые преобразования содержимого и определение следующего прыжка в маршрут для сообщения Перед выполнением кода в обработчик событий [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .  <br/> |
|[OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Возникает после сообщения взят из очереди отправки. Используйте событие [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , если агента транспорта RoutingAgent не требуется преобразования содержимого, разрешить получателей или маршрутизации данных.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Создание настраиваемых RoutingAgent агента транспорта

Следующая процедура описывается создание пользовательских RoutingAgent агента транспорта. 
  
### <a name="to-create-the-transport-agent"></a>Создание агента транспорта

1. Добавьте ссылки на пространства имен.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Эти пространства имен можно найти на сервере Exchange. Добавление ссылки на следующие пространства имен, будет обеспечивает доступ к членам [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) также другие классы, используемые в [Exchange 2013: создание агента транспорта ведения журнала пропускной способности](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) образца. 
    
2. Реализация производного класса для класса [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) . 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   Этот код будет создать экземпляр производного класса и переопределить метод **CreateAgent** для создания экземпляра настраиваемого агент. Дополнительные методы, такие как **Закрытие**, можно также переопределить в этом классе для выполнения пользовательского кода. 
    
3. Определение агента.
    
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

   После определения класса агента вы можно добавить пользовательские функции. В этом примере два события [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)перенаправляются к настраиваемым обработчикам событий. 
    
## <a name="see-also"></a>См. также

- [Транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Справочник по агента транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

