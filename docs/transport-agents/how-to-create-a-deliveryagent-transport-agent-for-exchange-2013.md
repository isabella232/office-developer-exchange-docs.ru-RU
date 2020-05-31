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
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="e57e2-103">Создание агента транспорта DeliveryAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e57e2-103">Create a DeliveryAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="e57e2-104">Узнайте, как создать настраиваемый агент транспорта DeliveryAgent для использования с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="e57e2-104">Find out how to create a custom DeliveryAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="e57e2-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="e57e2-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="e57e2-106">Классы [деливеряжентфактори\<Manager\> ](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) и [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) являются базовыми классами для агентов транспорта, которые предназначены для запуска в службе транспорта на сервере почтовых ящиков Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e57e2-106">The [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) and [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) classes are the base classes for transport agents that are designed to run on the Transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="e57e2-107">Вы можете реализовать обработчики в агенте транспорта DeliveryAgent для событий, предоставляемых классом [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) , которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e57e2-107">You might implement handlers in your DeliveryAgent transport agent for the events provided by the [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) class that are listed in the following table.</span></span> 
  
<span data-ttu-id="e57e2-108">**Таблица 1. События класса DeliveryAgent**</span><span class="sxs-lookup"><span data-stu-id="e57e2-108">**Table 1. DeliveryAgent class events**</span></span>

|<span data-ttu-id="e57e2-109">**Event**</span><span class="sxs-lookup"><span data-stu-id="e57e2-109">**Event**</span></span>|<span data-ttu-id="e57e2-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e57e2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e57e2-111">[онклосеконнектион](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="e57e2-111">[OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="e57e2-112">Происходит после доставки последней почтовой позиции и закрытия подключения.</span><span class="sxs-lookup"><span data-stu-id="e57e2-112">Occurs after the last mail item has been delivered and the connection is closed.</span></span>  <br/> |
|<span data-ttu-id="e57e2-113">[онделивермаилитем](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="e57e2-113">[OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="e57e2-114">Происходит, когда почтовый элемент готов к доставке.</span><span class="sxs-lookup"><span data-stu-id="e57e2-114">Occurs when a mail item is ready to be delivered.</span></span>  <br/> |
|<span data-ttu-id="e57e2-115">[онопенконнектион](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)</span><span class="sxs-lookup"><span data-stu-id="e57e2-115">[OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx)</span></span> <br/> |<span data-ttu-id="e57e2-116">Возникает при открытии агента доставки для доставки почты.</span><span class="sxs-lookup"><span data-stu-id="e57e2-116">Occurs when the delivery agent is opened for mail delivery.</span></span>  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a><span data-ttu-id="e57e2-117">Создание настраиваемого агента транспорта DeliveryAgent</span><span class="sxs-lookup"><span data-stu-id="e57e2-117">Creating a custom DeliveryAgent transport agent</span></span>

<span data-ttu-id="e57e2-118">В следующей процедуре описано, как создать настраиваемый агент транспорта DeliveryAgent.</span><span class="sxs-lookup"><span data-stu-id="e57e2-118">The following procedure describes how to create a custom DeliveryAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="e57e2-119">Создание агента транспорта</span><span class="sxs-lookup"><span data-stu-id="e57e2-119">To create the transport agent</span></span>

1. <span data-ttu-id="e57e2-120">Добавьте ссылки на пространства имен.</span><span class="sxs-lookup"><span data-stu-id="e57e2-120">Add references to the namespaces.</span></span>
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   <span data-ttu-id="e57e2-121">Эти пространства имен можно найти на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="e57e2-121">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="e57e2-122">Добавив ссылку на эти пространства имен, вы получите доступ к элементам [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) .</span><span class="sxs-lookup"><span data-stu-id="e57e2-122">By adding a reference to these namespaces, you will have access to the [DeliveryAgent](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent(v=exchg.150).aspx) members.</span></span> 
    
2. <span data-ttu-id="e57e2-123">Реализуйте производный класс для [класса\<диспетчера\> деливеряжентфактори](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) .</span><span class="sxs-lookup"><span data-stu-id="e57e2-123">Implement the derived class for the [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/en-us/library/dd877550(v=exchg.150).aspx) class.</span></span> 
    
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

   <span data-ttu-id="e57e2-124">В этом коде создается экземпляр производного класса и переопределяется метод **креатеажент** для создания экземпляра нового настраиваемого агента.</span><span class="sxs-lookup"><span data-stu-id="e57e2-124">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="e57e2-125">Дополнительные методы, такие как **Close**, также могут быть переопределены в этом классе для выполнения пользовательского кода.</span><span class="sxs-lookup"><span data-stu-id="e57e2-125">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> <span data-ttu-id="e57e2-126">Класс [деливеряжентманажер](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) создается для переопределения свойства [суппортедделиверипротокол](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) и установки протокола, который будет использоваться агентом.</span><span class="sxs-lookup"><span data-stu-id="e57e2-126">A [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) class is created to override the [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) property and set the protocol your agent will use.</span></span> 
    
3. <span data-ttu-id="e57e2-127">Определите свой агент.</span><span class="sxs-lookup"><span data-stu-id="e57e2-127">Define your agent.</span></span>
    
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

   <span data-ttu-id="e57e2-128">Определив класс агента, вы можете добавить пользовательские функции.</span><span class="sxs-lookup"><span data-stu-id="e57e2-128">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="e57e2-129">В этом примере три события, [онклосеконнектион](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [онделивермаилитем](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx)и [онопенконнектион](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), перенаправляются в обработчики пользовательских событий.</span><span class="sxs-lookup"><span data-stu-id="e57e2-129">In this example, the three events, [OnCloseConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.oncloseconnection(v=exchg.150).aspx), [OnDeliverMailItem](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.ondelivermailitem(v=exchg.150).aspx), and [OnOpenConnection](https://msdn.microsoft.com/en-us/library/microsoft.exchange.data.transport.delivery.deliveryagent.onopenconnection(v=exchg.150).aspx), are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="e57e2-130">См. также</span><span class="sxs-lookup"><span data-stu-id="e57e2-130">See also</span></span>

- [<span data-ttu-id="e57e2-131">Основные понятия, связанные с агентами транспорта в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e57e2-131">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="e57e2-132">Справочник по агентам транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="e57e2-132">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)          

 