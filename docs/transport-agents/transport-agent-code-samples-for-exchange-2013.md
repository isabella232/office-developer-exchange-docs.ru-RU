---
title: Примеры кода агента транспорта для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Найдите сведения о примерах агентов транспорта, доступных для Exchange 2013.
ms.openlocfilehash: 122a3351748fa6ffd823a51ce65ffb913332cb2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761316"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Примеры кода агента транспорта для Exchange 2013

Найдите сведения о примерах агентов транспорта, доступных для Exchange 2013.
  
**Применимо к:** Exchange Server 2013
  
Вы можете использовать API, включенные в Exchange Server 2013, для разработки агентов, расширяющих функциональные возможности транспорта. В этой статье представлены сведения о примерах агентов, которые помогут вам узнать, как программно расширить поведение транспорта. В примерах агентов есть исходный код для каждого компонента. 
  
В следующей таблице приведены примеры агентов для Exchange 2013.
  
**Таблица 1. Примеры агентов транспорта**

|**Имя примера**|**Описание**|
|:-----|:-----|
|[Exchange 2013: создание антивирусного агента транспорта](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |Этот агент отвечает на события [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) и [онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , а также отправляет входящее сообщение на сервер вне процесса, который асинхронно проверяет сообщение и возвращает измененную версию.  <br/> |
|[Exchange 2013: создание агента транспорта журналов пропускной способности](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |Этот агент отвечает на события [онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и [онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) , записывает использование пропускной способности для указанных получателей и записывает сведения об использовании полосы пропускания в текстовый файл.  <br/> |
|[Exchange 2013: создание агента транспорта преобразования текста](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |Этот агент фильтрует сценарии из сообщений электронной почты, определяя формат входящего сообщения и принимая решение о необходимости фильтрации. Если фильтрация необходима, содержимое преобразуется в формат HTML, фильтруется, а затем преобразуется обратно в исходный формат.  <br/> |
|[Exchange 2013: создание агента транспорта ведения журнала SMTP](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |Этот агент реагирует на событие [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) и асинхронно записывает сообщение в файл на локальном жестком диске.  <br/> |
|[Exchange 2013: создание агента транспорта, который временно блокирует отправители](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |Этот агент отвечает на события [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) и [онркпткомманд](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) и определяет, были ли отправители сообщений ранее отправили сообщения в службу транспорта переднего плана. Если отправитель ранее не отправлял сообщение в службу транспорта переднего плана, отправитель добавляется в список отправителей, а сообщение отклоняется с ответом, который сообщает клиенту, что он повторит попытку позже (также известно, как грайлистинг). Если отправитель находится в списке предыдущих отправителей, агент не отклоняет сообщение.  <br/> |
|[Exchange 2013: создание агента транспорта ведения журнала для сервера почтовых ящиков](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |Этот агент отвечает на событие конвейера транспорта [онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) и синхронно записывает сообщение в файл на локальном жестком диске.  <br/> |
|[Exchange 2013: построение агента транспорта X заголовков](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |Этот агент отвечает на событие [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) , а также считывает и изменяет X-заголовки в сообщениях.  <br/> |
   
## <a name="see-also"></a>См. также

- [Основные понятия, связанные с агентами транспорта в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)    
- [Справочник по агентам транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)    
- [Создание агента транспорта RoutingAgent для Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Создание агента транспорта SmtpReceiveAgent для Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Создание агента транспорта DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

