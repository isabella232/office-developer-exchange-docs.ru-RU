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
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Создание агента транспорта SmtpReceiveAgent для Exchange 2013

Узнайте, как создать настраиваемый агент транспорта SmtpReceiveAgent для использования с Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
Связанные фрагменты кода и примеры приложений:

- [Exchange 2013: создание агента транспорта преобразования текста](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
Классы [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) позволяют расширять поведение транспортной службы внешнего интерфейса на сервере клиентского доступа или в службе транспорта на сервере почтовых ящиков. Вы можете использовать эти классы для реализации агентов транспорта, которые отвечают за сообщения, поступающие в вашу организацию. 
  
Классы [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) включают события, перечисленные в следующей таблице. 
  
**Таблица 1. События класса SmtpReceiveAgent**

|**Event**|**Описание**|
|:-----|:-----|
|[онаускомманд](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |Используйте, когда агенту требуются сведения, которые предоставляются только в команде **проверки подлинности** SMTP, например агент, который принимает или отвергает попытки доставки сообщения на основе используемого типа метода проверки подлинности.  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |Используйте, когда агенту требуются сведения, которые предоставляются только при открытии подключения через SMTP к внешней службе транспорта, например к агенту, выполняющему действие на основе адреса или домена удаленного SMTP-сервера.  <br/> |
|[ондатакомманд](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |Используйте это событие, когда агенту требуются сведения, указанные в команде **данных** SMTP.  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |Используйте, когда агенту требуются сведения, доступные во время отключения, такие как текущая дата и время, для выполнения вычислений.  <br/> |
|[онехлокомманд](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |Используйте, когда агенту требуются сведения, указанные в команде EHLO в команде **EHLO** ; Например, если агент принимает или отклоняет сообщения на основе удостоверения, указанного в команде **EHLO** .  <br/> |
|[онендофаусентикатион](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |Используйте, когда агенту требуются сведения, доступные после того, как удаленный сервер завершит процесс проверки подлинности; Например, для агента, выполняющего действие с сообщением на основе сведений о проверке подлинности, предоставленных удаленным сервером или клиентом SMTP.  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |Используйте, когда агент должен выполнить действие на основе данных, доступных в сообщении. Это событие не будет запускаться для транспортной службы внешнего интерфейса. Если агент транспорта должен использовать это событие, его необходимо установить на сервере почтовых ящиков.  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |Используйте, когда агент должен выполнить действие на основе сведений, доступных в заголовках отправленного сообщения.  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>Создание настраиваемого агента транспорта SmtpReceiveAgent

В следующей процедуре описано, как создать настраиваемый агент транспорта SmtpReceiveAgent. 
  
### <a name="to-create-the-transport-agent"></a>Создание агента транспорта

1. Добавьте ссылки на пространства имен.
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   Эти пространства имен можно найти на сервере Exchange Server 2013. При добавлении ссылки на эти пространства имен вы получите доступ к элементам [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) , а также к другим классам, используемым в [Exchange 2013: построение образца агента транспорта преобразования текста](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) . 
    
2. Реализуйте производный класс для класса [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) . 
    
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

   В этом коде создается экземпляр производного класса и переопределяется метод **креатеажент** для создания экземпляра нового настраиваемого агента. 
    
3. Определите свой агент.
    
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

   Определив класс агента, вы можете добавить пользовательские функции. В этом примере событие [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) перенаправляется в обработчик настраиваемых событий. 
    
## <a name="see-also"></a>См. также

- [Основные понятия, связанные с агентами транспорта в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Справочник по агентам транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

