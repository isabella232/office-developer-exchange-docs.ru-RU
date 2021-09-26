---
title: Примеры кода транспортного агента для Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 626345ec-918f-4d91-932f-e6ce92553ccb
description: Сведения о примере транспортных агентов, доступных Exchange 2013 г.
ms.openlocfilehash: 56334f661947cffceaf18eb257feeb6504a71ecb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545718"
---
# <a name="transport-agent-code-samples-for-exchange-2013"></a>Примеры кода транспортного агента для Exchange 2013 г.

Сведения о примере транспортных агентов, доступных Exchange 2013 г.
  
**Применяется к:** Exchange Server 2013 г.
  
Вы можете использовать API, включенные в Exchange Server 2013 г., для разработки агентов, расширяют функции транспорта. В этой статье данная статья содержит сведения о доступных примерах агентов, которые помогут вам узнать, как программным образом расширять поведение транспорта. В примере агенты включают исходный код для каждого компонента. 
  
В следующей таблице перечислены примеры агентов для Exchange 2013 г.
  
**Таблица 1. Образцы транспортного агента**

|**Название примера**|**Описание**|
|:-----|:-----|
|[Exchange 2013 г.: создание агента транспорта антивируса](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-6e544269) <br/> |Этот агент отвечает на события [OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) и [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и отправляет входящие сообщения на неработающим сервером, который асинхронно проверяет сообщение и возвращает измененную версию.  <br/> |
|[Exchange 2013 г.: Создание транспортного агента для ведения журнала пропускной способности](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) <br/> |Этот агент отвечает на события [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и [OnRoutedMessage,](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) фиксирует использование пропускной способности для указанных получателей и регистрирует сведения об использовании пропускной способности в текстовом файле.  <br/> |
|[Exchange 2013 г. Создание транспортного агента преобразования тела](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-body-ed36ecb0) <br/> |Этот агент фильтрует скрипты из сообщений электронной почты, определяя формат входящих сообщений и решая, должна ли происходить фильтрация. Если требуется фильтрация, содержимое преобразуется в HTML, фильтруется и возвращается в исходный формат.  <br/> |
|[Exchange 2013 г. Создание транспортного агента для ведения журналов SMTP](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-fc23dc33) <br/> |Этот агент отвечает на [событие OnEndOfData](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfData.aspx) и асинхронно регистрирует сообщение в файл на локальном жестком диске.  <br/> |
|[Exchange 2013 г. Создайте транспортный агент, который временно блокирует отправителей](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-52a767d8) <br/> |Этот агент отвечает на события [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) и [OnRcptCommand](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnRcptCommand.aspx) и определяет, отправлял ли отправитель сообщения ранее сообщения службе переднего транспорта. Если отправитель ранее не отправил сообщение службе транспорта переднего конца, отправитель добавляется в список отправителей, и сообщение отклоняется с ответом, который сообщает клиенту попробовать еще раз позже (также известный как серый список). Если отправитель находится в списке предыдущих отправителей, агент не отклоняет сообщение.  <br/> |
|[Exchange 2013 г. Создание транспортного агента для ведения журнала почтовых ящиков](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-fc8632e5) <br/> |Этот агент отвечает на событие конвейера транспорта [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) и синхронно регистрирует сообщение в файл на локальном жестком диске.  <br/> |
|[Exchange 2013 г.: создание транспортного агента X-header](https://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-an-32f62f5a) <br/> |Этот агент отвечает на событие [OnEndOfHeaders](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.OnEndOfHeaders.aspx) и читает и изменит X-headers в сообщениях.  <br/> |
   
## <a name="see-also"></a>См. также

- [Концепции транспортного агента в Exchange 2013 г.](transport-agent-concepts-in-exchange-2013.md)    
- [Ссылка агента транспорта на Exchange 2013 г.](transport-agent-reference-for-exchange-2013.md)    
- [Создание транспортного агента RoutingAgent для Exchange 2013 г.](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)   
- [Создание транспортного агента SmtpReceiveAgent для Exchange 2013 г.](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)    
- [Создание транспортного агента DeliveryAgent для Exchange 2013 г.](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    

