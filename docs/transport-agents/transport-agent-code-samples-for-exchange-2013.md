---
title: Транспорта агента образцы кода для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Найдите сведения о агенты транспорта примера, доступных для Exchange 2013.
ms.openlocfilehash: 122a3351748fa6ffd823a51ce65ffb913332cb2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761316"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Транспорта агента образцы кода для Exchange 2013

Найдите сведения о агенты транспорта примера, доступных для Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
Можно использовать интерфейсы API, которые включены в Exchange Server 2013 для разработки агенты, расширения функциональных возможностей транспорта. В этой статье сведения об агентах примеры, которые помогут вам в этой статье описывается расширение поведения транспорта программными средствами. Пример агенты включают исходный код для каждого компонента. 
  
В следующей таблице перечислены агенты пример для Exchange 2013.
  
**В таблице 1. Примеры агента транспорта**

|**Пример имени**|**Описание**|
|:-----|:-----|
|[Exchange 2013: Построение агент передачи](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |Данный агент отвечает на события [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) и [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и отправляет входящие сообщения на сервер вне процесса асинхронно проверки сообщения и возвращает измененную версию.  <br/> |
|[Exchange 2013: Создание агента транспорта пропускной способности ведения журнала](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |Данный агент отвечает на события [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) , захватывает использование пропускной способности для указанного получателей и записывает сведения об использовании пропускной способности в текстовый файл.  <br/> |
|[Exchange 2013: Создание агента транспорта преобразования текста](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |Данный агент фильтр скрипты из сообщений электронной почты, определив формат входящего сообщения и фильтрации должно выполняться при принятии решения. При необходимости фильтрации содержимого преобразования в формат HTML, фильтруемых и затем преобразуется в формат источника.  <br/> |
|[Exchange 2013: Создание агента транспорта SMTP ведения журнала](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |Данный агент отвечает на событие [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) и асинхронно записывает сообщение в файл на локальный жесткий диск.  <br/> |
|[Exchange 2013: Создание агента транспорта, временно блокирует отправителей](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |Данный агент отвечает на события [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) и [OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) и определяет, ли отправителя сообщения ранее отправленных сообщений к службе транспорта переднего плана. Если отправитель ранее не отправлено сообщение в службу транспорта переднего плана, отправитель будет добавлен в список отправителей и сообщение отклоняется, ответ, сообщающий клиента, чтобы повторить попытку позже (также известной как graylisting). Если отправитель входит в список предыдущих отправителей, агент не отклоняет сообщение.  <br/> |
|[Exchange 2013: Создание агента транспорта ведения журналов сервера почтовых ящиков](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |Данный агент отвечает на события [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) транспортный конвейер и синхронно регистрирует сообщение файла на локальный жесткий диск.  <br/> |
|[Exchange 2013: Создание агента транспорта X-заголовка](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |Данный агент отвечает на событие [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) и читать и изменять X-заголовков в сообщениях.  <br/> |
   
## <a name="see-also"></a>См. также

- [Транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Справочник по агента транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [Создание агента транспорта RoutingAgent для Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Создание агента транспорта SmtpReceiveAgent для Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Создание агента транспорта DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

