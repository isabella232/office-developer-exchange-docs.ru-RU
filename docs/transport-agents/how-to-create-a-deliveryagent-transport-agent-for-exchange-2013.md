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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761289"
---
# <a name="create-a-deliveryagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="964da-103">Создание агента транспорта DeliveryAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="964da-103">Create a DeliveryAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="964da-104">Узнайте, как создать настраиваемые агента транспорта DeliveryAgent для использования с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="964da-104">Find out how to create a custom DeliveryAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="964da-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="964da-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="964da-106">[DeliveryAgentFactory\<диспетчера\> ](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) и [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) классы являются базовые классы для агенты транспорта, которые предназначены для выполнения в службе транспорта на сервере почтовых ящиков Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="964da-106">The [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) and [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) classes are the base classes for transport agents that are designed to run on the Transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="964da-107">Обработчики могут реализовать в вашей DeliveryAgent агента транспорта для событий, предоставляемых классом [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) , перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="964da-107">You might implement handlers in your DeliveryAgent transport agent for the events provided by the [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) class that are listed in the following table.</span></span> 
  
<span data-ttu-id="964da-108">**В таблице 1. События класса DeliveryAgent**</span><span class="sxs-lookup"><span data-stu-id="964da-108">**Table 1. DeliveryAgent class events**</span></span>

|<span data-ttu-id="964da-109">**Событие**</span><span class="sxs-lookup"><span data-stu-id="964da-109">**Event**</span></span>|<span data-ttu-id="964da-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="964da-110">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="964da-111">OnCloseConnection</span><span class="sxs-lookup"><span data-stu-id="964da-111">OnCloseConnection</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnCloseConnection.aspx) <br/> |<span data-ttu-id="964da-112">Возникает после последнего элемента почты было доставлено и закрытия подключения.</span><span class="sxs-lookup"><span data-stu-id="964da-112">Occurs after the last mail item has been delivered and the connection is closed.</span></span>  <br/> |
|[<span data-ttu-id="964da-113">OnDeliverMailItem</span><span class="sxs-lookup"><span data-stu-id="964da-113">OnDeliverMailItem</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnDeliverMailItem.aspx) <br/> |<span data-ttu-id="964da-114">Происходит, когда элемент почты готова к доставки.</span><span class="sxs-lookup"><span data-stu-id="964da-114">Occurs when a mail item is ready to be delivered.</span></span>  <br/> |
|[<span data-ttu-id="964da-115">OnOpenConnection</span><span class="sxs-lookup"><span data-stu-id="964da-115">OnOpenConnection</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnOpenConnection.aspx) <br/> |<span data-ttu-id="964da-116">Происходит при открытии агента доставки для доставки электронной почты.</span><span class="sxs-lookup"><span data-stu-id="964da-116">Occurs when the delivery agent is opened for mail delivery.</span></span>  <br/> |
   
## <a name="creating-a-custom-deliveryagent-transport-agent"></a><span data-ttu-id="964da-117">Создание настраиваемых DeliveryAgent агента транспорта</span><span class="sxs-lookup"><span data-stu-id="964da-117">Creating a custom DeliveryAgent transport agent</span></span>

<span data-ttu-id="964da-118">Следующая процедура описывается создание пользовательских DeliveryAgent агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="964da-118">The following procedure describes how to create a custom DeliveryAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="964da-119">Создание агента транспорта</span><span class="sxs-lookup"><span data-stu-id="964da-119">To create the transport agent</span></span>

1. <span data-ttu-id="964da-120">Добавьте ссылки на пространства имен.</span><span class="sxs-lookup"><span data-stu-id="964da-120">Add references to the namespaces.</span></span>
    
   ```cs
        using Microsoft.Exchange.Data.Transport;
        using Microsoft.Exchange.Data.Transport.Delivery;
    
   ```

   <span data-ttu-id="964da-121">Эти пространства имен можно найти на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="964da-121">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="964da-122">Добавление ссылки на следующие пространства имен, имеется доступ к членам [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) .</span><span class="sxs-lookup"><span data-stu-id="964da-122">By adding a reference to these namespaces, you will have access to the [DeliveryAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx) members.</span></span> 
    
2. <span data-ttu-id="964da-123">Реализация производного класса для [DeliveryAgentFactory\<диспетчера\> ](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) класса.</span><span class="sxs-lookup"><span data-stu-id="964da-123">Implement the derived class for the [DeliveryAgentFactory\<Manager\>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx) class.</span></span> 
    
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

   <span data-ttu-id="964da-124">Этот код будет создать экземпляр производного класса и переопределить метод **CreateAgent** для создания экземпляра настраиваемого агент.</span><span class="sxs-lookup"><span data-stu-id="964da-124">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="964da-125">Дополнительные методы, такие как **Закрытие**, можно также переопределить в этом классе для выполнения пользовательского кода.</span><span class="sxs-lookup"><span data-stu-id="964da-125">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> <span data-ttu-id="964da-126">Класс [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) создается переопределить свойство [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) и задать протокола, который будет использоваться агентом.</span><span class="sxs-lookup"><span data-stu-id="964da-126">A [DeliveryAgentManager](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx) class is created to override the [SupportedDeliveryProtocol](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.SupportedDeliveryProtocol.aspx) property and set the protocol your agent will use.</span></span> 
    
3. <span data-ttu-id="964da-127">Определение агента.</span><span class="sxs-lookup"><span data-stu-id="964da-127">Define your agent.</span></span>
    
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

   <span data-ttu-id="964da-128">После определения класса агента вы можно добавить пользовательские функции.</span><span class="sxs-lookup"><span data-stu-id="964da-128">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="964da-129">В этом примере три события, [OnCloseConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnCloseConnection.aspx) , [OnDeliverMailItem](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnDeliverMailItem.aspx) и [OnOpenConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnOpenConnection.aspx) перенаправляются к настраиваемым обработчикам событий.</span><span class="sxs-lookup"><span data-stu-id="964da-129">In this example, the three events, [OnCloseConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnCloseConnection.aspx) , [OnDeliverMailItem](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnDeliverMailItem.aspx) and [OnOpenConnection](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgent.OnOpenConnection.aspx) , are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="964da-130">См. также</span><span class="sxs-lookup"><span data-stu-id="964da-130">See also</span></span>

- [<span data-ttu-id="964da-131">Транспорта концепции агентов в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="964da-131">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)
- [<span data-ttu-id="964da-132">Справочник по агента транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="964da-132">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="964da-133">DeliveryAgentFactory\<Manager\></span><span class="sxs-lookup"><span data-stu-id="964da-133">DeliveryAgentFactory\<Manager\></span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentFactory`1.aspx)   
- [<span data-ttu-id="964da-134">DeliveryAgent</span><span class="sxs-lookup"><span data-stu-id="964da-134">DeliveryAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.DeliveryType.DeliveryAgent.aspx)    
- [<span data-ttu-id="964da-135">DeliveryAgentManager</span><span class="sxs-lookup"><span data-stu-id="964da-135">DeliveryAgentManager</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Delivery.DeliveryAgentManager.aspx)
    

