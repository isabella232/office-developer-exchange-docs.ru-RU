---
title: Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Найдите материалы, которые помогут вам устранить неполадки управляемого API EWS или приложения EWS.
localization_priority: Priority
ms.openlocfilehash: 7c7cbe8c93edec5ad99df079c6eb96286c1ba063
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463743"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange

Найдите материалы, которые помогут вам устранить неполадки управляемого API EWS или приложения EWS.
  
Все это не всегда запланировано. Иногда не удается выполнить запросы EWS, а также приводятся неожиданные результаты. Это может быть очень сложно, особенно если причина неочевидна. Надеюсь, что это никогда не произойдет, но в этой статье представлены сведения о средствах и ресурсах, которые можно использовать для устранения неполадок.
  
> [!NOTE]
> В этой статье приводятся общие рекомендации по устранению неполадок и источники сведений об устранении неполадок. К сожалению, невозможно получить подробные инструкции по устранению неполадок. Помощь в устранении неполадок, связанных с конкретной ошибкой, приведено в разделе [Дополнительные действия](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Проверка запросов и ответов SOAP

Если бы они не работали должным образом, она, в своюмся, может увидеть, что происходит. Первая строка запроса при исследовании проблемы с помощью EWS или управляемого API EWS — проверка запросов, которые приложение отправляет по сети, и ответы, отправляемые сервером обратно.
  
Управляемый API EWS упрощает анализ запросов и ответов SOAP с помощью [встроенных функций трассировки](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md). Если вы используете EWS, у вас может быть или нет доступа к аналогичной функции трассировки в зависимости от того, какие платформы или классы вы используете для отправки запросов. Однако вы всегда можете использовать средство трассировки сети, например, [Network Monitor](https://www.microsoft.com/download/details.aspx?id=4865) или [Fiddler](http://www.telerik.com/fiddler) , для проверки сетевого трафика и просмотра полезных данных запроса и ответа. 
  
Кроме того, вы можете [инструментировать клиентские запросы](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) для расширения информации, доступной в запросах и ответах. 
  
После выполнения запросов и ответов ответьте на следующие вопросы: правильно ли они выглядят? Предполагается, что ваше приложение посылается должным образом? Имеете смысл принимать ответы?
  
## <a name="examine-error-codes"></a>Проверка кодов ошибок

Иногда код ошибки может быть достаточно большим, даже если на первый взгляд он не имеет смысла. Указывает, что направляется [регулирование](ews-throttling-in-exchange.md)клиента? Возможно, вызов службы автообнаружения для [обновления сведений о конфигурации](how-to-refresh-configuration-information-by-using-autodiscover.md) выполняется по порядку? 
  
Дополнительные сведения об обработке определенных ошибок можно найти в следующих статьях:
  
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)
    
- [Обработка ошибок, связанных с уведомлениями, в EWS в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с синхронизацией, в EWS в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удалением, в EWS в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Проверка версий

В операциях EWS существует несколько различных компонентов, и их версии могут влиять на результаты.
  
**Таблица 1. Компоненты с версиями, которые могут повлиять на процессы EWS**

|**Компонент**|**Управляемый API EWS**|**Службы EWS**|**Примечания**|
|:-----|:-----|:-----|:-----|
|Запрошенная версия сервера  <br/> |Свойство [ексчанжесервицебасе. рекуестедсерверверсион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |Элемент [рекуестсерверверсион](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Это значение определяет, какая версия схемы EWS используется для обработки запроса EWS. Убедитесь, что указанная здесь версия схемы имеет смысл для отправляемого запроса. Некоторые свойства и операции недоступны в более ранних версиях схемы.  <br/> |
|Версия сервера  <br/> |Свойство [ексчанжесервицебасе. серверинфо](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |Элемент [серверверсионинфо](https://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Это значение возвращается сервером в ответах EWS и указывает версию сервера, который обработал ответ. Убедитесь, что это значение ожидается. Если это возможно, убедитесь, что на сервере Exchange выполняется Последнее обновление основной версии Exchange.  <br/> |
|Версия управляемого API EWS  <br/> |Свойство версии продукта для файла Microsoft. Exchange. WebServices. dll.  <br/> |Неприменимо  <br/> |Если вы используете управляемый API EWS, убедитесь, что вы используете [самую последнюю версию](https://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Проверка доступа

По умолчанию EWS включена, но [можно изменить значения по умолчанию](how-to-control-access-to-ews-in-exchange.md). С помощью командлета [Get-OrganizationConfig](https://technet.microsoft.com/library/bb124754.aspx) убедитесь, что на сервере включена EWS, а также командлет [Get-CASMailbox](https://technet.microsoft.com/library/aa997571.aspx) , чтобы убедиться, что для почтового ящика пользователя включена EWS. Кроме того, проверьте оба ответа командлета для списка разрешенных или заблокированных служб EWS и убедитесь, что приложение не заблокировано с помощью EWS. 
  
Кроме того, необходимо убедиться, что [Параметры проверки подлинности по умолчанию](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx) в виртуальном каталоге EWS не были изменены. 
  
## <a name="try-another-ews-client"></a>Попробуйте другой клиент EWS

Иногда бывает полезно попробовать один и тот же запрос от другого клиента и сравнить результаты. Если другой клиент получает разные результаты, что отличается? Выяснить, чем отличается успешный запрос, и неудачный запрос может помочь объяснить причину сбоя конкретного запроса.
  
Несмотря на то, что вы наверняка можете написать другой клиент для тестирования, вам не нужно! [Евседитор](http://ewseditor.codeplex.com/) — это пример клиента, который использует управляемый API EWS и EWS. Вы можете скачать клиент (включая исходный код) и использовать его для попытаться использовать те же запросы, что и при неисправности в вашем приложении. 
  
## <a name="examine-iis-logs"></a>Проверка журналов IIS

Если у вас есть доступ к серверу Exchange, функции ведения журнала, предоставляемые службами IIS на серверах клиентского доступа, могут предоставить дополнительные сведения об ошибках. Однако имейте в виду, что журналы IIS будут полезны только при получении сообщения об ошибке HTTP.
  
Службы IIS предоставляют два разных метода ведения журнала: мониторинг [журналов IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) и [неудачные запросы](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis). Для работы с журналами IIS можно использовать [средство Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), включающее ряд встроенных запросов EWS.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_NextSteps"> </a>

Теперь, когда вы узнали о средствах и ресурсах, которые можно использовать для устранения неполадок, может потребоваться помощь в понимании сведений, предоставляемых этими средствами. Ниже приведены некоторые способы получения справки.
  
- [Форум по разработке Exchange Server в MSDN](https://social.msdn.microsoft.com/Forums/home?category=exchangeserver) — задайте вопрос СООБЩЕСТВУ разработчиков MSDN для Exchange Server. 
    
- [Сайте StackOverflow](http://stackoverflow.com/tags/ews) — задайте вопрос сообщества сайте StackOverflow. Не забудьте пометить сообщение с помощью "EWS". 
    
- [Служба поддержки Майкрософт](https://support.microsoft.com/ph/730/en-us) — обратитесь за помощью к специалисту службы поддержки Майкрософт. 
    
## <a name="see-also"></a>См. также


См. следующие статьи:
  
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Трассировка запросов и ответов для устранения неполадок в приложениях управляемого API EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [Инструментирование запросов клиентов для EWS и REST в Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [EWS регулирование в Exchange](ews-throttling-in-exchange.md)
    
- [Обновление сведений о конфигурации с помощью службы автообнаружения](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)
    
- [Обработка ошибок, связанных с уведомлениями, в EWS в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с синхронизацией, в EWS в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удалением, в EWS в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [Настройка ведения журнала в службах IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [Устранение неудачных запросов с помощью трассировки в IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Введение: Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Параметры по умолчанию для виртуальных каталогов Exchange](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx)
    
Скачайте следующие компоненты:
  
- [Сетевой монитор Microsoft 3.4](https://www.microsoft.com/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler);
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [Управляемый API веб-служб Exchange](https://go.microsoft.com/fwlink/?LinkID=255472)
    

