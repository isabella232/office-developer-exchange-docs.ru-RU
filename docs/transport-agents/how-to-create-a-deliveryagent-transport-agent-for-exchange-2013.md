---
title: Создание агента транспорта DeliveryAgent для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: Узнайте, как создать настраиваемые агента транспорта DeliveryAgent для использования с Exchange 2013.
ms.openlocfilehash: 44ee5dc465f4435f0b835d264331cb719fe875c1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761289"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Создание агента транспорта DeliveryAgent для Exchange 2013

Узнайте, как создать настраиваемые агента транспорта DeliveryAgent для использования с Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
[DeliveryAgentFactory\<диспетчера\> ](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) и [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) классы являются базовые классы для агенты транспорта, которые предназначены для выполнения в службе транспорта на сервере почтовых ящиков Exchange Server 2013. Обработчики могут реализовать в вашей DeliveryAgent агента транспорта для событий, предоставляемых классом [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) , перечисленные в следующей таблице. 
  
**В таблице 1. События класса DeliveryAgent**

|**Событие**|**Описание**|
|:-----|:-----|
|[OnCloseConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnCloseConnection.aspx) <br/> |Возникает после последнего элемента почты было доставлено и закрытия подключения.  <br/> |
|[OnDeliverMailItem](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnDeliverMailItem.aspx) <br/> |Происходит, когда элемент почты готова к доставки.  <br/> |
|[OnOpenConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnOpenConnection.aspx) <br/> |Происходит при открытии агента доставки для доставки электронной почты.  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>Создание настраиваемых DeliveryAgent агента транспорта

Следующая процедура описывается создание пользовательских DeliveryAgent агента транспорта. 
  
### <a name="to-create-the-transport-agent"></a>Создание агента транспорта

1. Добавьте ссылки на пространства имен.
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   Эти пространства имен можно найти на сервере Exchange. Добавление ссылки на следующие пространства имен, имеется доступ к членам [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) . 
    
2. Реализация производного класса для [DeliveryAgentFactory\<диспетчера\> ](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) класса. 
    
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

   Этот код будет создать экземпляр производного класса и переопределить метод **CreateAgent** для создания экземпляра настраиваемого агент. Дополнительные методы, такие как **Закрытие**, можно также переопределить в этом классе для выполнения пользовательского кода. Класс [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) создается переопределить свойство [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) и задать протокола, который будет использоваться агентом. 
    
3. Определение агента.
    
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

   После определения класса агента вы можно добавить пользовательские функции. В этом примере три события, [OnCloseConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnCloseConnection.aspx) , [OnDeliverMailItem](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnDeliverMailItem.aspx) и [OnOpenConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnOpenConnection.aspx) перенаправляются к настраиваемым обработчикам событий. 
    
## <a name="see-also"></a>См. также

- [Транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Справочник по агента транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx)   
- [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx)    
- [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx)
    

