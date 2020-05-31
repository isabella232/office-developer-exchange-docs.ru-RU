---
title: Создание агента транспорта DeliveryAgent для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4af904d7-b315-4849-92b1-66018f76ffdf
description: Узнайте, как создать настраиваемый агент транспорта DeliveryAgent для использования с Exchange 2013.
ms.openlocfilehash: bc36c7b5e0fb8006c5927d423d7767dcc7382ce0
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353310"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a>Создание агента транспорта DeliveryAgent для Exchange 2013

Узнайте, как создать настраиваемый агент транспорта DeliveryAgent для использования с Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
Классы [деливеряжентфактори\<Manager\> ](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) и [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) являются базовыми классами для агентов транспорта, которые предназначены для запуска в службе транспорта на сервере почтовых ящиков Exchange Server 2013. Вы можете реализовать обработчики в агенте транспорта DeliveryAgent для событий, предоставляемых классом [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) , которые перечислены в следующей таблице. 
  
**Таблица 1. События класса DeliveryAgent**

|**Event**|**Описание**|
|:-----|:-----|
|[онклосеконнектион](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx) <br/> |Происходит после доставки последней почтовой позиции и закрытия подключения.  <br/> |
|[онделивермаилитем](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx) <br/> |Происходит, когда почтовый элемент готов к доставке.  <br/> |
|[онопенконнектион](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx) <br/> |Возникает при открытии агента доставки для доставки почты.  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a>Создание настраиваемого агента транспорта DeliveryAgent

В следующей процедуре описано, как создать настраиваемый агент транспорта DeliveryAgent. 
  
### <a name="to-create-the-transport-agent"></a>Создание агента транспорта

1. Добавьте ссылки на пространства имен.
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   Эти пространства имен можно найти на сервере Exchange. Добавив ссылку на эти пространства имен, вы получите доступ к элементам [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) . 
    
2. Реализуйте производный класс для [класса\<диспетчера\> деливеряжентфактори](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) . 
    
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

   В этом коде создается экземпляр производного класса и переопределяется метод **креатеажент** для создания экземпляра нового настраиваемого агента. Дополнительные методы, такие как **Close**, также могут быть переопределены в этом классе для выполнения пользовательского кода. Класс [деливеряжентманажер](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) создается для переопределения свойства [суппортедделиверипротокол](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) и установки протокола, который будет использоваться агентом. 
    
3. Определите свой агент.
    
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

   Определив класс агента, вы можете добавить пользовательские функции. В этом примере три события, [онклосеконнектион](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [онделивермаилитем](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)и [онопенконнектион](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), перенаправляются в обработчики пользовательских событий. 
    
## <a name="see-also"></a>См. также

- [Основные понятия, связанные с агентами транспорта в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)
- [Справочник по агентам транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)          

 