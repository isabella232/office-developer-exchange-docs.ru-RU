---
title: Создание агента транспорта SmtpReceiveAgent для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Узнайте, как создать настраиваемый агент транспорта SmtpReceiveAgent для использования с Exchange 2013.
ms.openlocfilehash: 5ba021d02849ffc7e125029f0fd18ebf14c3f8da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459141"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="0c88c-103">Создание агента транспорта SmtpReceiveAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c88c-103">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="0c88c-104">Узнайте, как создать настраиваемый агент транспорта SmtpReceiveAgent для использования с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="0c88c-104">Find out how to create a custom SmtpReceiveAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="0c88c-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="0c88c-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="0c88c-106">Связанные фрагменты кода и примеры приложений:</span><span class="sxs-lookup"><span data-stu-id="0c88c-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="0c88c-107">Exchange 2013: создание агента транспорта преобразования текста</span><span class="sxs-lookup"><span data-stu-id="0c88c-107">Exchange 2013: Build a body conversion transport agent</span></span>](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
<span data-ttu-id="0c88c-108">Классы [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) позволяют расширять поведение транспортной службы внешнего интерфейса на сервере клиентского доступа или в службе транспорта на сервере почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="0c88c-108">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes enable you to extend the behavior of the Front End Transport service on a Client Access Server or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="0c88c-109">Вы можете использовать эти классы для реализации агентов транспорта, которые отвечают за сообщения, поступающие в вашу организацию.</span><span class="sxs-lookup"><span data-stu-id="0c88c-109">You can use these classes to implement transport agents that are designed to respond to messages as they come into your organization.</span></span> 
  
<span data-ttu-id="0c88c-110">Классы [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) включают события, перечисленные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="0c88c-110">The [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes include the events listed in the following table.</span></span> 
  
<span data-ttu-id="0c88c-111">**Таблица 1. События класса SmtpReceiveAgent**</span><span class="sxs-lookup"><span data-stu-id="0c88c-111">**Table 1. SmtpReceiveAgent class events**</span></span>

|<span data-ttu-id="0c88c-112">**Event**</span><span class="sxs-lookup"><span data-stu-id="0c88c-112">**Event**</span></span>|<span data-ttu-id="0c88c-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0c88c-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0c88c-114">онаускомманд</span><span class="sxs-lookup"><span data-stu-id="0c88c-114">OnAuthCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |<span data-ttu-id="0c88c-115">Используйте, когда агенту требуются сведения, которые предоставляются только в команде **проверки подлинности** SMTP, например агент, который принимает или отвергает попытки доставки сообщения на основе используемого типа метода проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="0c88c-115">Use when your agent requires information that is provided only in the SMTP **AUTH** command, such as an agent that accepts or rejects attempts to deliver a message based on the type of authentication method used.</span></span>  <br/> |
|[<span data-ttu-id="0c88c-116">OnConnect</span><span class="sxs-lookup"><span data-stu-id="0c88c-116">OnConnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |<span data-ttu-id="0c88c-117">Используйте, когда агенту требуются сведения, которые предоставляются только при открытии подключения через SMTP к внешней службе транспорта, например к агенту, выполняющему действие на основе адреса или домена удаленного SMTP-сервера.</span><span class="sxs-lookup"><span data-stu-id="0c88c-117">Use when your agent requires information that is provided only when a connection is opened via SMTP to the Front End Transport service, such as an agent that performs an action based on the address or domain of the remote SMTP server.</span></span>  <br/> |
|[<span data-ttu-id="0c88c-118">ондатакомманд</span><span class="sxs-lookup"><span data-stu-id="0c88c-118">OnDataCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |<span data-ttu-id="0c88c-119">Используйте это событие, когда агенту требуются сведения, указанные в команде **данных** SMTP.</span><span class="sxs-lookup"><span data-stu-id="0c88c-119">Use this event when your agent requires information that is provided in the SMTP **DATA** command.</span></span>  <br/> |
|[<span data-ttu-id="0c88c-120">OnDisconnect</span><span class="sxs-lookup"><span data-stu-id="0c88c-120">OnDisconnect</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |<span data-ttu-id="0c88c-121">Используйте, когда агенту требуются сведения, доступные во время отключения, такие как текущая дата и время, для выполнения вычислений.</span><span class="sxs-lookup"><span data-stu-id="0c88c-121">Use when your agent requires information that is available at the time of disconnection, such as the current date and time, in order to perform time calculations.</span></span>  <br/> |
|[<span data-ttu-id="0c88c-122">онехлокомманд</span><span class="sxs-lookup"><span data-stu-id="0c88c-122">OnEhloCommand</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |<span data-ttu-id="0c88c-123">Используйте, когда агенту требуются сведения, указанные в команде EHLO в команде **EHLO** ; Например, если агент принимает или отклоняет сообщения на основе удостоверения, указанного в команде **EHLO** .</span><span class="sxs-lookup"><span data-stu-id="0c88c-123">Use when your agent requires information that is provided in the SMTP **EHLO** command; for example, if your agent accepts or rejects messages based on the identity provided in the **EHLO** command.</span></span>  <br/> |
|[<span data-ttu-id="0c88c-124">онендофаусентикатион</span><span class="sxs-lookup"><span data-stu-id="0c88c-124">OnEndOfAuthentication</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |<span data-ttu-id="0c88c-125">Используйте, когда агенту требуются сведения, доступные после того, как удаленный сервер завершит процесс проверки подлинности; Например, для агента, выполняющего действие с сообщением на основе сведений о проверке подлинности, предоставленных удаленным сервером или клиентом SMTP.</span><span class="sxs-lookup"><span data-stu-id="0c88c-125">Use when your agent requires information that is available after the remote server completes the authentication process; for example, for an agent that performs an action on a message based on the authentication information provided by the remote SMTP server or client.</span></span>  <br/> |
|[<span data-ttu-id="0c88c-126">OnEndOfData</span><span class="sxs-lookup"><span data-stu-id="0c88c-126">OnEndOfData</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |<span data-ttu-id="0c88c-127">Используйте, когда агент должен выполнить действие на основе данных, доступных в сообщении.</span><span class="sxs-lookup"><span data-stu-id="0c88c-127">Use when your agent must perform an action based on data that is available in the message.</span></span> <span data-ttu-id="0c88c-128">Это событие не будет запускаться для транспортной службы внешнего интерфейса.</span><span class="sxs-lookup"><span data-stu-id="0c88c-128">This event will not fire on the Front End Transport service.</span></span> <span data-ttu-id="0c88c-129">Если агент транспорта должен использовать это событие, его необходимо установить на сервере почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="0c88c-129">If your transport agent has to use this event, you have to install it on a Mailbox server.</span></span>  <br/> |
|[<span data-ttu-id="0c88c-130">OnEndOfHeaders</span><span class="sxs-lookup"><span data-stu-id="0c88c-130">OnEndOfHeaders</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |<span data-ttu-id="0c88c-131">Используйте, когда агент должен выполнить действие на основе сведений, доступных в заголовках отправленного сообщения.</span><span class="sxs-lookup"><span data-stu-id="0c88c-131">Use when your agent must perform an action based on information that is available in the headers of the submitted message.</span></span>  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a><span data-ttu-id="0c88c-132">Создание настраиваемого агента транспорта SmtpReceiveAgent</span><span class="sxs-lookup"><span data-stu-id="0c88c-132">Creating a custom SmtpReceiveAgent transport agent</span></span>

<span data-ttu-id="0c88c-133">В следующей процедуре описано, как создать настраиваемый агент транспорта SmtpReceiveAgent.</span><span class="sxs-lookup"><span data-stu-id="0c88c-133">The following procedure describes how to create a custom SmtpReceiveAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="0c88c-134">Создание агента транспорта</span><span class="sxs-lookup"><span data-stu-id="0c88c-134">To create the transport agent</span></span>

1. <span data-ttu-id="0c88c-135">Добавьте ссылки на пространства имен.</span><span class="sxs-lookup"><span data-stu-id="0c88c-135">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   <span data-ttu-id="0c88c-136">Эти пространства имен можно найти на сервере Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0c88c-136">You can find these namespaces on your Exchange 2013 server.</span></span> <span data-ttu-id="0c88c-137">При добавлении ссылки на эти пространства имен вы получите доступ к элементам [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) , а также к другим классам, используемым в [Exchange 2013: построение образца агента транспорта преобразования текста](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) .</span><span class="sxs-lookup"><span data-stu-id="0c88c-137">When you add a reference to these namespaces, you will have access to the [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a body conversion transport agent](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) sample.</span></span> 
    
2. <span data-ttu-id="0c88c-138">Реализуйте производный класс для класса [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="0c88c-138">Implement the derived class for the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) class.</span></span> 
    
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

   <span data-ttu-id="0c88c-139">В этом коде создается экземпляр производного класса и переопределяется метод **креатеажент** для создания экземпляра нового настраиваемого агента.</span><span class="sxs-lookup"><span data-stu-id="0c88c-139">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> 
    
3. <span data-ttu-id="0c88c-140">Определите свой агент.</span><span class="sxs-lookup"><span data-stu-id="0c88c-140">Define your agent.</span></span>
    
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

   <span data-ttu-id="0c88c-141">Определив класс агента, вы можете добавить пользовательские функции.</span><span class="sxs-lookup"><span data-stu-id="0c88c-141">After you define your agent class, you can add your custom functionality.</span></span> <span data-ttu-id="0c88c-142">В этом примере событие [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) перенаправляется в обработчик настраиваемых событий.</span><span class="sxs-lookup"><span data-stu-id="0c88c-142">In this example, the [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) event is redirected to your custom event handler.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="0c88c-143">См. также</span><span class="sxs-lookup"><span data-stu-id="0c88c-143">See also</span></span>

- [<span data-ttu-id="0c88c-144">Основные понятия, связанные с агентами транспорта в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c88c-144">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="0c88c-145">Справочник по агентам транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="0c88c-145">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="0c88c-146">смтпрецеивеажентфактори</span><span class="sxs-lookup"><span data-stu-id="0c88c-146">SmtpReceiveAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [<span data-ttu-id="0c88c-147">SmtpReceiveAgent</span><span class="sxs-lookup"><span data-stu-id="0c88c-147">SmtpReceiveAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

