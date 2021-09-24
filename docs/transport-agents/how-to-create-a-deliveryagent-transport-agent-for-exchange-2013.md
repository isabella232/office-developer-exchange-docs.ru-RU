---
title: Создание транспортного агента DeliveryAgent для Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: Узнайте, как создать настраиваемый транспортный агент DeliveryAgent для использования с Exchange 2013 г.
ms.openlocfilehash: b465c3bbd4658bea700d5be9f4eb16ae81693717
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526935"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Создание транспортного агента DeliveryAgent для Exchange 2013 г.

Узнайте, как создать настраиваемый транспортный агент DeliveryAgent для использования с Exchange 2013 г.
  
**Применяется к:** Exchange Server 2013 г.
  
Классы [DeliveryAgentFactory \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) и [DeliveryAgent](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) являются базовыми классами для транспортных агентов, предназначенных для работы на транспортной службе на сервере почтовых ящиков 2013 Exchange Server 2013 года. Вы можете реализовать обработчики в транспортном агенте DeliveryAgent для событий, предоставляемых классом [DeliveryAgent,](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) которые указаны в следующей таблице. 
  
**Таблица 1. События класса DeliveryAgent**

|**Event**|**Описание**|
|:-----|:-----|
|[OnCloseConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) <br/> |Происходит после доставки последнего элемента почты и закрытия подключения.  <br/> |
|[OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) <br/> |Возникает, когда элемент почты будет готов к доставке.  <br/> |
|[OnOpenConnection](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx) <br/> |Происходит, когда агент доставки открыт для доставки почты.  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>Создание настраиваемой транспортной службы DeliveryAgent

В следующей процедуре описывается, как создать настраиваемый транспортный агент DeliveryAgent. 
  
### <a name="to-create-the-transport-agent"></a>Создание транспортного агента

1. Добавьте ссылки на пространства имен.
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   Эти пространства имен можно найти на Exchange сервере. Добавив ссылку на эти пространства имен, вы сможете получить доступ к участникам [DeliveryAgent.](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) 
    
2. Реализация полученного класса для [класса DeliveryAgentFactory. \<Manager\> ](https://msdn.microsoft.com/library/dd877550(v=exchg.150).aspx) 
    
   ```cs
      public class MyDeliveryAgentFactory : DeliveryAgentFactory<MyDeliveryAgentFactory.MyDeliveryAgentManager>
      {
          static MyDeliveryAgentFactory()
          {
          }
          public override DeliveryAgent CreateAgent(SmtpServer server)
          {
              return new MyDeliveryAgent(server);
          }
          public sealed class MyDeliveryAgentManager : DeliveryAgentManager
          {
              /// <summary>
              /// Gets the supported delivery protocol.
              /// </summary>
              public override string SupportedDeliveryProtocol
              {
                  get { return "MyProtocol"; }
              }
          }
      }
  
   ```

   Этот код мгновенно выводится из полученного класса и переопределяет метод **CreateAgent** для создания экземпляра нового настраиваемого агента. Дополнительные методы, такие как **Close,** также могут быть переопределены в этом классе для выполнения настраиваемого кода. Для переопределения свойства [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) создается класс [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) и устанавливается протокол, который будет использовать агент. 
    
3. Определите агента.
    
   ```cs
      public class MyDeliveryAgent : DeliveryAgent
      {
          public MyDeliveryAgent(SmtpServer server)
          {
              this.OnCloseConnection += CloseConnection;
              this.OnDeliverMailItem += DeliverMailItem;
              this.OnOpenConnection += OpenConnection;
          }
      }
  
   ```

   После определения класса агента можно добавить настраиваемые функциональные возможности. В этом примере три [события, OnCloseConnection,](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) [OnDeliverMailItem](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)и [OnOpenConnection,](https://msdn.microsoft.com/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)перенаправляются в настраиваемые обработчики событий. 
    
## <a name="see-also"></a>См. также

- [Концепции транспортного агента в Exchange 2013 г.](transport-agent-concepts-in-exchange-2013.md)
- [Ссылка агента транспорта на Exchange 2013 г.](transport-agent-reference-for-exchange-2013.md)          

 