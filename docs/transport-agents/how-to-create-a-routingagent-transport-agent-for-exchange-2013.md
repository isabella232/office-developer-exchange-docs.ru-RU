---
title: Создание агента транспорта RoutingAgent для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Узнайте, как создать настраиваемый агент транспорта RoutingAgent для использования с Exchange 2013.
ms.openlocfilehash: d07f68494acd26940a4837bbbfc7a0505114bd20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761299"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a>Создание агента транспорта RoutingAgent для Exchange 2013

Узнайте, как создать настраиваемый агент транспорта RoutingAgent для использования с Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
Связанные фрагменты кода и примеры приложений:

- [Exchange 2013: создание агента транспорта журналов пропускной способности](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
Классы [раутингажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) и [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) являются базовыми классами для агентов транспорта, которые предназначены для запуска в службе транспорта на сервере почтовых ящиков Exchange Server 2013. Класс [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) предоставляет события, перечисленные в следующей таблице, для которых вы можете реализовать обработчики в агенте транспорта RoutingAgent. 
  
**Таблица 1. События класса RoutingAgent**

|**Event**|**Описание**|
|:-----|:-----|
|[онкатегоризедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |Происходит, когда сервер выполняет преобразование контента, если это необходимо.  <br/> |
|[OnResolvedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |Возникает после того, как все получатели сообщения были разрешены и до того, как будет определена маршрутизация.  <br/> |
|[онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |Возникает после того, как сервер направляет сообщение на следующий прыжок и выполняет преобразование контента, если это необходимо. Сервер может использовать больше ресурсов для обработки каждого сообщения в событии [онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) по сравнению с событием [онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , так как сервер выполняет все необходимое преобразование контента и определяет следующий прыжок в маршруте для сообщения перед выполнением кода в обработчике событий [онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .  <br/> |
|[онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |Возникает после того, как сообщение отправится из очереди. Используйте событие [онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , если агент транспорта RoutingAgent не нуждается в преобразовании контента, разрешенных получателях или данных маршрутизации.  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a>Создание настраиваемого агента транспорта RoutingAgent

В следующей процедуре описано, как создать настраиваемый агент транспорта RoutingAgent. 
  
### <a name="to-create-the-transport-agent"></a>Создание агента транспорта

1. Добавьте ссылки на пространства имен.
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   Эти пространства имен можно найти на сервере Exchange. Добавив ссылку на эти пространства имен, вы получите доступ к элементам [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) , а также к другим классам, используемым в [Exchange 2013: Создание примера агента транспорта журналов пропускной способности](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) . 
    
2. Реализуйте производный класс для класса [раутингажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) . 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   В этом коде создается экземпляр производного класса и переопределяется метод **креатеажент** для создания экземпляра нового настраиваемого агента. Дополнительные методы, такие как **Close**, также могут быть переопределены в этом классе для выполнения пользовательского кода. 
    
3. Определите свой агент.
    
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

   Определив класс агента, вы можете добавить пользовательские функции. В этом примере два события [онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и [онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)перенаправлены в обработчики пользовательских событий. 
    
## <a name="see-also"></a>См. также

- [Основные понятия, связанные с агентами транспорта в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Справочник по агентам транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [раутингажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

