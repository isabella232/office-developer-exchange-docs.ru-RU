---
title: Создание агента транспорта SmtpReceiveAgent для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Узнайте, как создать настраиваемые агента транспорта SmtpReceiveAgent для использования с Exchange 2013.
ms.openlocfilehash: a74d5baae6334c5e17acb6335206964b48f320e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761415"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="9af48-103">Создание агента транспорта SmtpReceiveAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9af48-103">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="9af48-104">Узнайте, как создать настраиваемые агента транспорта SmtpReceiveAgent для использования с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="9af48-104">Find out how to create a custom SmtpReceiveAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="9af48-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="9af48-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="9af48-106">Связанные фрагменты кода и примеры приложений:</span><span class="sxs-lookup"><span data-stu-id="9af48-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="9af48-107">Exchange 2013: Создание агента транспорта преобразования текста</span><span class="sxs-lookup"><span data-stu-id="9af48-107">Exchange 2013: Build a body conversion transport agent</span></span>](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
<span data-ttu-id="9af48-108">Классы [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) дают возможность расширить поведение транспортной службы на сервере клиентского доступа или транспортной службы на сервере почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="9af48-108">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes enable you to extend the behavior of the Front End Transport service on a Client Access Server or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="9af48-109">Можно использовать эти классы для реализации агенты транспорта, которые предназначены для отвечать на сообщения, возникших в вашей организации.</span><span class="sxs-lookup"><span data-stu-id="9af48-109">You can use these classes to implement transport agents that are designed to respond to messages as they come into your organization.</span></span> 
  
<span data-ttu-id="9af48-110">Классы [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) содержат событий, перечисленных в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="9af48-110">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes include the events listed in the following table.</span></span> 
  
<span data-ttu-id="9af48-111">**В таблице 1. События класса SmtpReceiveAgent**</span><span class="sxs-lookup"><span data-stu-id="9af48-111">**Table 1. SmtpReceiveAgent class events**</span></span>

|<span data-ttu-id="9af48-112">**Событие**</span><span class="sxs-lookup"><span data-stu-id="9af48-112">**Event**</span></span>|<span data-ttu-id="9af48-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9af48-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9af48-114">OnAuthCommand</span><span class="sxs-lookup"><span data-stu-id="9af48-114">OnAuthCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |<span data-ttu-id="9af48-115">Используется, когда агента нужны сведения, которая предоставляется только в команде SMTP с **проверкой Подлинности на основе** , такие как агент, который принимает, либо отклоняет пытается доставить сообщение на основе типа метод проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9af48-115">Use when your agent requires information that is provided only in the SMTP **AUTH** command, such as an agent that accepts or rejects attempts to deliver a message based on the type of authentication method used.</span></span>  <br/> |
|[<span data-ttu-id="9af48-116">OnConnect</span><span class="sxs-lookup"><span data-stu-id="9af48-116">OnConnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |<span data-ttu-id="9af48-117">Используется, когда агента нужны сведения, которая предоставляется только при открытии подключения по протоколу SMTP для транспортной службы внешнего интерфейса, таких как агент, который выполняет действие на основе адреса или домена удаленный SMTP-сервера.</span><span class="sxs-lookup"><span data-stu-id="9af48-117">Use when your agent requires information that is provided only when a connection is opened via SMTP to the Front End Transport service, such as an agent that performs an action based on the address or domain of the remote SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="9af48-118">OnDataCommand</span><span class="sxs-lookup"><span data-stu-id="9af48-118">OnDataCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |<span data-ttu-id="9af48-119">Используйте это событие, когда агента требуется информация, содержащаяся в команде SMTP **данных** .</span><span class="sxs-lookup"><span data-stu-id="9af48-119">Use this event when your agent requires information that is provided in the SMTP **DATA** command.</span></span>  <br/> |
|[<span data-ttu-id="9af48-120">OnDisconnect</span><span class="sxs-lookup"><span data-stu-id="9af48-120">OnDisconnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |<span data-ttu-id="9af48-121">Используется, когда агента нужны сведения, доступные во время отключения, такие как текущую дату и время, чтобы выполнить вычисления времени.</span><span class="sxs-lookup"><span data-stu-id="9af48-121">Use when your agent requires information that is available at the time of disconnection, such as the current date and time, in order to perform time calculations.</span></span>  <br/> |
|[<span data-ttu-id="9af48-122">OnEhloCommand</span><span class="sxs-lookup"><span data-stu-id="9af48-122">OnEhloCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |<span data-ttu-id="9af48-123">Используется, когда агента требуется информация, содержащаяся в команде SMTP **EHLO** ; Например, если ваше Агент принимает или отклоняет на основе удостоверений, представленные в команде **EHLO** .</span><span class="sxs-lookup"><span data-stu-id="9af48-123">Use when your agent requires information that is provided in the SMTP **EHLO** command; for example, if your agent accepts or rejects messages based on the identity provided in the **EHLO** command.</span></span>  <br/> |
|[<span data-ttu-id="9af48-124">OnEndOfAuthentication</span><span class="sxs-lookup"><span data-stu-id="9af48-124">OnEndOfAuthentication</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |<span data-ttu-id="9af48-125">Используется, когда агента нужны сведения, доступные удаленный сервер по завершении процесса проверки подлинности; Например, агент, который выполняет действие в сообщении, основываясь на информации проверки подлинности, предоставляемый удаленный SMTP-сервера или клиента.</span><span class="sxs-lookup"><span data-stu-id="9af48-125">Use when your agent requires information that is available after the remote server completes the authentication process; for example, for an agent that performs an action on a message based on the authentication information provided by the remote SMTP server or client.</span></span>  <br/> |
|[<span data-ttu-id="9af48-126">OnEndOfData</span><span class="sxs-lookup"><span data-stu-id="9af48-126">OnEndOfData</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |<span data-ttu-id="9af48-127">Используется, когда агента нужно выполнить действие на основе данных, который доступен в окне сообщения.</span><span class="sxs-lookup"><span data-stu-id="9af48-127">Use when your agent must perform an action based on data that is available in the message.</span></span> <span data-ttu-id="9af48-128">Это событие не будет срабатывать в службе транспорта переднего плана.</span><span class="sxs-lookup"><span data-stu-id="9af48-128">This event will not fire on the Front End Transport service.</span></span> <span data-ttu-id="9af48-129">Если ваше агента транспорта должен использовать данное событие, необходимо установить его на сервере почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="9af48-129">If your transport agent has to use this event, you have to install it on a Mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="9af48-130">OnEndOfHeaders</span><span class="sxs-lookup"><span data-stu-id="9af48-130">OnEndOfHeaders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |<span data-ttu-id="9af48-131">Используется, когда агента нужно выполнить действие на основе сведений, доступные в заголовках отправляемого сообщения.</span><span class="sxs-lookup"><span data-stu-id="9af48-131">Use when your agent must perform an action based on information that is available in the headers of the submitted message.</span></span>  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a><span data-ttu-id="9af48-132">Создание настраиваемых SmtpReceiveAgent агента транспорта</span><span class="sxs-lookup"><span data-stu-id="9af48-132">Creating a custom SmtpReceiveAgent transport agent</span></span>

<span data-ttu-id="9af48-133">Следующая процедура описывается создание пользовательских SmtpReceiveAgent агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="9af48-133">The following procedure describes how to create a custom SmtpReceiveAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="9af48-134">Создание агента транспорта</span><span class="sxs-lookup"><span data-stu-id="9af48-134">To create the transport agent</span></span>

1. <span data-ttu-id="9af48-135">Добавьте ссылки на пространства имен.</span><span class="sxs-lookup"><span data-stu-id="9af48-135">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   <span data-ttu-id="9af48-136">Эти пространства имен можно найти на сервере Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="9af48-136">You can find these namespaces on your Exchange 2013 server.</span></span> <span data-ttu-id="9af48-137">При добавлении ссылки на следующие пространства имен, будут иметь доступ к элементам [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) также другие классы, используемые в [Exchange 2013: создание агента транспорта преобразования текста](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) образца.</span><span class="sxs-lookup"><span data-stu-id="9af48-137">When you add a reference to these namespaces, you will have access to the [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a body conversion transport agent](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) sample.</span></span> 
    
2. <span data-ttu-id="9af48-138">Реализация производного класса для класса [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="9af48-138">Implement the derived class for the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BodyConversionFactory : SmtpReceiveAgentFactory
      {
          /// <summary>
          /// Create a new BodyConversion
          /// </summary>
          /// <param name="server">Exchange server</param>
          /// <returns>A new BodyConversion</returns>
          public override SmtpReceiveAgent CreateAgent(SmtpServer server)
          {
              return new BodyConversion();
          }
      }
  
   ```

   <span data-ttu-id="9af48-139">Этот код будет создать экземпляр производного класса и переопределить метод **CreateAgent** для создания экземпляра настраиваемого агент.</span><span class="sxs-lookup"><span data-stu-id="9af48-139">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> 
    
3. <span data-ttu-id="9af48-140">Определение агента.</span><span class="sxs-lookup"><span data-stu-id="9af48-140">Define your agent.</span></span>
    
   ```cs
     public class BodyConversion : SmtpReceiveAgent
      {
          // Your custom code goes here
          /// <summary>
          /// The constructor registers an end of data event handler.
          /// </summary>
          public BodyConversion()
          {
              Debug.WriteLine("[BodyConversion] Agent constructor");
              this.OnEndOfData += new EndOfDataEventHandler(this.OnEndOfDataHandler);
          }
      }
  
   ```

   <span data-ttu-id="9af48-141">После определения класса агента, можно добавить пользовательские функции.</span><span class="sxs-lookup"><span data-stu-id="9af48-141">After you define your agent class, you can add your custom functionality.</span></span> <span data-ttu-id="9af48-142">В этом примере событие [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) перенаправляется на настраиваемый обработчик событий.</span><span class="sxs-lookup"><span data-stu-id="9af48-142">In this example, the [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) event is redirected to your custom event handler.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="9af48-143">См. также</span><span class="sxs-lookup"><span data-stu-id="9af48-143">See also</span></span>

- [<span data-ttu-id="9af48-144">Транспорта концепции агентов в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9af48-144">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="9af48-145">Справочник по агента транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9af48-145">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="9af48-146">SmtpReceiveAgentFactory</span><span class="sxs-lookup"><span data-stu-id="9af48-146">SmtpReceiveAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [<span data-ttu-id="9af48-147">SmtpReceiveAgent</span><span class="sxs-lookup"><span data-stu-id="9af48-147">SmtpReceiveAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

