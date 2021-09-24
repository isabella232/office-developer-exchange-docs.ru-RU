---
title: Создание транспортного агента SmtpReceiveAgent для Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: cdc7c462-74a7-49d6-95b2-155d783840e9
description: Узнайте, как создать настраиваемый транспортный агент SmtpReceiveAgent для использования с Exchange 2013 г.
ms.openlocfilehash: a441f93113798c10421e9073e266c28fd87bca8d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513033"
---
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Создание транспортного агента SmtpReceiveAgent для Exchange 2013 г.

Узнайте, как создать настраиваемый транспортный агент SmtpReceiveAgent для использования с Exchange 2013 г.
  
**Применяется к:** Exchange Server 2013 г.
  
Связанные фрагменты кода и примеры приложений:

- [Exchange 2013 г. Создание транспортного агента преобразования тела](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
Классы [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) позволяют расширить поведение передней транспортной службы на сервере клиентского доступа или транспортной службе на сервере почтовых ящиков. Эти классы можно использовать для реализации транспортных агентов, предназначенных для реагирования на сообщения при их ввозе в организацию. 
  
Классы [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) включают события, перечисленные в следующей таблице. 
  
**Таблица 1. События класса SmtpReceiveAgent**

|**Event**|**Описание**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |Используйте, когда вашему агенту требуются сведения, предоставляемые только в команде SMTP **AUTH,** например агент, который принимает или отклоняет попытки доставки сообщения в зависимости от типа используемого метода проверки подлинности.  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |Используйте, когда агенту требуются сведения, предоставляемые только в том случае, если подключение через SMTP открывается к службе переднего транспорта, например агенту, который выполняет действие на основе адреса или домена удаленного сервера SMTP.  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |Используйте это событие, если вашему агенту требуются сведения, предоставляемые в команде SMTP **DATA.**  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |Используйте, когда агенту требуется информация, доступная во время отключения, например текущая дата и время, для выполнения расчетов времени.  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |Использование, когда агенту требуется информация, представленная в команде SMTP **EHLO;** например, если агент принимает или отклоняет сообщения на основе удостоверения, предоставленного в команде **EHLO.**  <br/> |
|[OnEndOfAuthentication](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |Использование, когда агенту требуется информация, доступная после завершения процесса проверки подлинности удаленным сервером; например, для агента, который выполняет действия по сообщению на основе сведений о проверке подлинности, предоставляемых удаленным сервером SMTP или клиентом.  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |Используйте, когда агент должен выполнить действие на основе данных, доступных в сообщении. Это событие не будет работать на переднем конце транспортной службы. Если транспортному агенту необходимо использовать это событие, необходимо установить его на сервер почтовых ящиков.  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |Используйте, когда агент должен выполнить действие на основе сведений, доступных в заглавных главах отправленного сообщения.  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>Создание настраиваемого транспортного агента SmtpReceiveAgent

Следующая процедура описывает создание настраиваемого транспортного агента SmtpReceiveAgent. 
  
### <a name="to-create-the-transport-agent"></a>Создание транспортного агента

1. Добавьте ссылки на пространства имен.
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   Эти пространства имен можно найти на Exchange 2013 года. При добавлении ссылки на эти пространства имен у вас будет доступ к участникам [SmtpReceiveAgent,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) а также к другим классам, используемым в [Exchange 2013: Сборка](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) образца транспортного агента преобразования тела. 
    
2. Реализация полученного класса для [класса SmtpReceiveAgentFactory.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) 
    
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

   Этот код мгновенно выводится из полученного класса и переопределяет метод **CreateAgent** для создания экземпляра нового настраиваемого агента. 
    
3. Определите агента.
    
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

   После определения класса агента можно добавить настраиваемые функции. В этом примере событие [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) перенаправляется на настраиваемый обработник событий. 
    
## <a name="see-also"></a>См. также

- [Концепции транспортного агента в Exchange 2013 г.](transport-agent-concepts-in-exchange-2013.md)    
- [Ссылка агента транспорта на Exchange 2013 г.](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

