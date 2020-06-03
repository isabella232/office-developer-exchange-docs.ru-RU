---
title: Повышение производительности при использовании автообнаружения для Exchange
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: e65ff6b2-3810-43ad-9728-27308891b193
description: Сведения о том, как улучшить производительность процесса автообнаружения в приложении.
ms.openlocfilehash: 844b56084b4f0b5e49b4ee095688d58ce469baca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456334"
---
# <a name="improving-performance-when-using-autodiscover-for-exchange"></a>Повышение производительности при использовании автообнаружения для Exchange

Информация, содержащаяся в этом документе, может относиться к функциям и продуктам предварительной версии и может претерпеть значительные изменения до окончательного коммерческого выпуска. Настоящий документ предоставляется "как есть" и служит только для информационных целей. Корпорация Майкрософт не предоставляет никаких гарантий, явных или подразумеваемых, в связи с этим документом Сведения о том, как улучшить производительность процесса автообнаружения в приложении.
  
Существует много причин, чтобы как службы автообнаружения. Настройка приложений для подключения к Exchange без вмешательства пользователя отлично! Если вы читаете в этой статье, известно все причины использования и привлекательности автообнаружения, поэтому их не будут перечислены ниже. Вместо этого мы будем говорить о потенциальных недостаток: производительности.
  
Службы автообнаружения изначально не медленных процесс, но он не является по определению fast либо. [Процесс автообнаружения](autodiscover-for-exchange.md) включает много сети и, которая представляется потенциал задержки. Процесс автоматического обнаружения состоит из трех этапов; все три иметь возможность влиять на производительность. 
  
- Определение пула кандидатов конечной точки службы автообнаружения  для приложений, работающих на компьютерах, присоединенный к домену, это может включать в себя [операции поиска SCP](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md), которая включает в себя общение с доменными службами Active Directory (AD DS).
    
- При каждом кандидат  для этого необходимо запроса и ответа HTTP для каждой конечной точки кандидата.
    
- Альтернативными  кандидатов в пуле кандидата конечной точки службы автообнаружения не создают результаты, можно выполнить после запроса GET (HTTP-запросов и ответов) и поиск в DNS.
    
В рабочей области это не выглядит как значительная. Тем не менее, например, вы можете сценарий пула кандидатов конечной точки службы автообнаружения  это больше, чем один или два URL-адресов, куда не удается найти working один до последнего URL-адрес в пуле. Задержка может стать более заметно. Таким образом что можно сделать?
  
## <a name="consider-the-need-for-scp-lookup"></a>Следует учитывать необходимость поиска SCP

Когда объекты SCP присутствует и также настроен, они ускорить процесс автоматического обнаружения. В других ситуациях Однако они может снизить его. Если SCP не используется в вашей среде, пропустите всей SCP подстановки часть процесса автообнаружения для экономии времени.
  
Управляемый API EWS упрощает: просто задайте для свойства [ExchangeService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablescplookup%28v=exchg.80%29.aspx) значение **false** до вызова метода [ExchangeService.AutodiscoverUrl](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.autodiscoverurl%28v=exchg.80%29.aspx) . Если вы используете класс [AutodiscoverService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx) , присвойте свойству [AutodiscoverService.EnableScpLookup](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice.enablescplookup%28v=exchg.80%29.aspx) для **false** до вызова любого из методов. 
  
## <a name="use-autodiscover-less-often"></a>Часто используемых автообнаружения меньше

Автообнаружение не предназначены для использования часто используется в приложениях. Назначение за автообнаружения-приложение может использовать для получения сведений о конфигурации и кэшировать эти сведения на определенный период времени. Если не кэширование сведений о конфигурации, рассмотрите возможность добавления кэширование для приложения, чтобы уменьшить количество раз, используйте службы автообнаружения.
  
Даже в том случае, если вы уже кэширования, оцените, как долго кэша данных конфигурации. Стандартный  чтобы [Обновить данные о автообнаружения каждые 24 часа](how-to-refresh-configuration-information-by-using-autodiscover.md), но можно расширить указанное время. Следует проверить с помощью целевых средах и прийти «время жизни» для вашей конфигурации, которая работает для вас.
  
## <a name="minimize-requested-data"></a>Минимизация запрошенные данные

If you're using the **AutodiscoverService** class in the EWS Managed API, or the [Операция GetUserSettings (SOAP)](https://msdn.microsoft.com/library/758d965c-ef63-4de4-9120-e293abf14ff8%28Office.15%29.aspx) operation via SOAP, you have direct control over what settings are returned in the response. Although you can request quite a few settings, chances are that your application only needs a handful of them. Every setting that you request requires more processing on the server, which means more time waiting for a response. Evaluate the settings you are requesting, and eliminate any that you don't need. 
  
Если вы используете метод **ExchangeService.AutodiscoverUrl** в управляемый API веб-служб Exchange, не может изменить параметры, которые вы запрашиваете. Тем не менее этот метод уже является очень эффективным. только его запрашивает параметры **ExternalEwsUrl** и **InternalEwsUrl**[перечисление UserSettingName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.usersettingname%28v=exchg.80%29.aspx).
  
При использовании службы автообнаружения POX, [не могут запрашивать определенных свойств](autodiscover-for-exchange.md#bk_Options).
  
## <a name="see-also"></a>См. также


- [Автообнаружение в Exchange](autodiscover-for-exchange.md)
    
- [Обнаружение конечных точек автообнаружения с помощью поиска SCP в Exchange](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md)
    
- [Обновление сведений о конфигурации с помощью службы автообнаружения](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Класс ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)
    
- [Класс AutodiscoverService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.autodiscover.autodiscoverservice%28v=exchg.80%29.aspx)
    

