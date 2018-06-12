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
# <a name="create-an-smtpreceiveagent-transport-agent-for-exchange-2013"></a>Создание агента транспорта SmtpReceiveAgent для Exchange 2013

Узнайте, как создать настраиваемые агента транспорта SmtpReceiveAgent для использования с Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
Связанные фрагменты кода и примеры приложений:

- [Exchange 2013: Создание агента транспорта преобразования текста](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0)
  
Классы [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) дают возможность расширить поведение транспортной службы на сервере клиентского доступа или транспортной службы на сервере почтовых ящиков. Можно использовать эти классы для реализации агенты транспорта, которые предназначены для отвечать на сообщения, возникших в вашей организации. 
  
Классы [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) содержат событий, перечисленных в следующей таблице. 
  
**В таблице 1. События класса SmtpReceiveAgent**

|**Событие**|**Описание**|
|:-----|:-----|
|[OnAuthCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnAuthCommand.aspx) <br/> |Используется, когда агента нужны сведения, которая предоставляется только в команде SMTP с **проверкой Подлинности на основе** , такие как агент, который принимает, либо отклоняет пытается доставить сообщение на основе типа метод проверки подлинности.  <br/> |
|[OnConnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnConnect.aspx) <br/> |Используется, когда агента нужны сведения, которая предоставляется только при открытии подключения по протоколу SMTP для транспортной службы внешнего интерфейса, таких как агент, который выполняет действие на основе адреса или домена удаленный SMTP-сервера.  <br/> |
|[OnDataCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDataCommand.aspx) <br/> |Используйте это событие, когда агента требуется информация, содержащаяся в команде SMTP **данных** .  <br/> |
|[OnDisconnect](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnDisconnect.aspx) <br/> |Используется, когда агента нужны сведения, доступные во время отключения, такие как текущую дату и время, чтобы выполнить вычисления времени.  <br/> |
|[OnEhloCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEhloCommand.aspx) <br/> |Используется, когда агента требуется информация, содержащаяся в команде SMTP **EHLO** ; Например, если ваше Агент принимает или отклоняет на основе удостоверений, представленные в команде **EHLO** .  <br/> |
|[OnEndOfAuthentication](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfAuthentication.aspx) <br/> |Используется, когда агента нужны сведения, доступные удаленный сервер по завершении процесса проверки подлинности; Например, агент, который выполняет действие в сообщении, основываясь на информации проверки подлинности, предоставляемый удаленный SMTP-сервера или клиента.  <br/> |
|[OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) <br/> |Используется, когда агента нужно выполнить действие на основе данных, который доступен в окне сообщения. Это событие не будет срабатывать в службе транспорта переднего плана. Если ваше агента транспорта должен использовать данное событие, необходимо установить его на сервере почтовых ящиков.  <br/> |
|[OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) <br/> |Используется, когда агента нужно выполнить действие на основе сведений, доступные в заголовках отправляемого сообщения.  <br/> |
   
## <a name="creating-a-custom-smtpreceiveagent-transport-agent"></a>Создание настраиваемых SmtpReceiveAgent агента транспорта

Следующая процедура описывается создание пользовательских SmtpReceiveAgent агента транспорта. 
  
### <a name="to-create-the-transport-agent"></a>Создание агента транспорта

1. Добавьте ссылки на пространства имен.
    
   ```cs
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Smtp;
      using Microsoft.Exchange.Data.Transport.Email;
      using Microsoft.Exchange.Data.TextConverters;
  
   ```

   Эти пространства имен можно найти на сервере Exchange 2013. При добавлении ссылки на следующие пространства имен, будут иметь доступ к элементам [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) также другие классы, используемые в [Exchange 2013: создание агента транспорта преобразования текста](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) образца. 
    
2. Реализация производного класса для класса [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) . 
    
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

   Этот код будет создать экземпляр производного класса и переопределить метод **CreateAgent** для создания экземпляра настраиваемого агент. 
    
3. Определение агента.
    
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

   После определения класса агента, можно добавить пользовательские функции. В этом примере событие [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) перенаправляется на настраиваемый обработчик событий. 
    
## <a name="see-also"></a>См. также

- [Транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Справочник по агента транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx)    
- [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx)
    

