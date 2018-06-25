---
title: Средства и ресурсы, необходимые для устранения неполадок приложений веб-служб Exchange для Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Найдите ресурсы, которые помогут устранить управляемый API EWS или приложение веб-служб Exchange.
ms.openlocfilehash: d8d8ea736ca3b896642ad06f5987caeba8d8d059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761247"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Средства и ресурсы, необходимые для устранения неполадок приложений веб-служб Exchange для Exchange

Найдите ресурсы, которые помогут устранить управляемый API EWS или приложение веб-служб Exchange.
  
Что не всегда перейдите по плану. В некоторых случаях веб-служб Exchange сбоя или привести к непредсказуемым результатам. Это может быть неудобства, особенно в том случае, если не очевидны. Надеюсь никогда не подобное вам, но если это так, в этой статье содержатся сведения об инструментах и ресурсы, которые можно использовать для решения проблемы.
  
> [!NOTE]
> В этой статье предоставляет общие совет по устранению неполадок и источников сведений об устранении неполадок. К сожалению нельзя предоставить сведения об устранении неполадок. Устранение неполадок сведений об ошибке можно найти [Далее действия](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Просмотрите запросы и ответы SOAP

При действия не работает корректно, полезно действительно могут видеть, что происходит. Первая строка запроса при исследование проблем с веб-служб Exchange или управляемый API EWS для проверки запросов, которые приложение передает по сети и ответы, сервер отправляет обратно.
  
Управляемый API EWS упрощает анализ запросы и ответы SOAP с его [встроенные возможности трассировки](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md). При использовании веб-служб Exchange, вы может или может не иметь доступ к аналогичные возможности трассировки, в зависимости от того, какие платформы или классы, используется для отправки запросов. Тем не менее всегда можно использовать средство сетевой трассировки как [Fiddler](http://www.telerik.com/fiddler) или [Сетевого монитора](http://www.microsoft.com/en-us/download/details.aspx?id=4865) для проверки сетевого трафика и просматривать полезных данных запроса и ответа. 
  
Кроме того можно [инструментировать клиентских запросов](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) для расширения сведений, доступных в запросы и ответы. 
  
После того как запросы и ответы, ответьте на следующие: они отображаются правильно? Существуют значения, которые приложение отправляет ожидается? Смысл ответы?
  
## <a name="examine-error-codes"></a>Изучите кодов ошибок

В некоторых случаях код ошибки можно перейти значительное продвижение к точное проблемы, даже в том случае, если с первого взгляда кажется смысла. Ошибки обозначения, что клиент, [регулирование](ews-throttling-in-exchange.md)? Возможно вызова службы автообнаружения для [обновления сведений о конфигурации](how-to-refresh-configuration-information-by-using-autodiscover.md) является в порядке? 
  
Дополнительные сведения об обработке ошибок см в следующих статьях:
  
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)
    
- [Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с синхронизации в веб-служб Exchange в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удаления в веб-служб Exchange в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Проверка версии

Существует несколько разных компонентов, участвующих в операции EWS и версии этих компонентов, которые влияют на результаты.
  
**В таблице 1. Версий компонентов, которые могут повлиять на процессы веб-служб Exchange**

|**Компонент**|**Управляемый API EWS**|**Службы EWS**|**Примечания**|
|:-----|:-----|:-----|:-----|
|Запрошенный сервер версии  <br/> |Свойство [ExchangeServiceBase.RequestedServerVersion](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |Элемент [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Это значение определяет, какие версии схемы веб-служб Exchange используется для обработки запроса веб-служб Exchange. Убедитесь в том, что версию схемы, указанным здесь имеет смысл для запроса, что отправке. Некоторые свойства и операции, недоступны в более ранних версиях схемы.  <br/> |
|Версия сервера  <br/> |Свойство [ExchangeServiceBase.ServerInfo](http://msdn.microsoft.com/EN-US/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |Элемент [ServerVersionInfo](http://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Это значение возвращается в ответы веб-служб Exchange на сервере и указывает версию сервера, на котором обработки ответа. Убедитесь в том, что это значение является, как ожидалось. Если это возможно убедитесь в том, что запущен самое последнее обновление для вашей версии Exchange на сервере Exchange.  <br/> |
|Управляемый API EWS версии  <br/> |Свойство version продукта Microsoft.Exchange.WebServices.dll файла.  <br/> |Не применимо  <br/> |Если вы используете управляемый API веб-служб Exchange, убедитесь в том, что вы используете [наиболее поздней версии](http://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Проверка доступа

Веб-служб Exchange включена по умолчанию, но [можно изменить параметры по умолчанию](how-to-control-access-to-ews-in-exchange.md). С помощью командлета [Get-OrganizationConfig](http://technet.microsoft.com/en-us/library/bb124754.aspx) , убедитесь в том, что включен веб-служб Exchange на сервере и [Get-CASMailbox](http://technet.microsoft.com/en-us/library/aa997571.aspx) используется, чтобы убедиться в том, что веб-служб Exchange включена для почтового ящика пользователя. Также проверьте оба командлета ответа для запроса EWS разрешить или заблокировать список и убедитесь в том, что ваше приложение не блокируется с помощью веб-служб Exchange. 
  
Также необходимо убедиться в том, что [Параметры проверки подлинности по умолчанию](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx) в виртуальном каталоге EWS не были изменены. 
  
## <a name="try-another-ews-client"></a>Попробуйте другого клиентского веб-служб Exchange

В некоторых случаях будет полезно же запрос от другого клиента и сравнение полученных результатов. Если другой клиент получает разные результаты, каковы отличия? Чтобы определить, каковы отличия между успешный запрос и неудачных запросов может помочь поясняется, почему не удается выполнить запрос.
  
Хотя определенно можно написать другого клиента для тестирования с, не нужно. [EWSEditor](http://ewseditor.codeplex.com/) — это пример клиент, использующий управляемый API EWS и веб-служб Exchange. Можно загрузить клиента (в том числе исходный код) и попробуйте же запросы, которые выполняются в приложении. 
  
## <a name="examine-iis-logs"></a>В журналах IIS

Если у вас есть доступ к серверу Exchange, функциональные возможности ведения журнала, предоставляемые Internet Information Services (IIS) на серверах клиентского доступа можно указать дополнительные сведения об ошибках. Тем не менее следует иметь в виду, входящему в IIS будет только полезны, если вы получили ошибку HTTP.
  
Службы IIS предоставляют два различных методов ведения журнала: [ведения журналов служб IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) и [Отслеживание неудачных запросов](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis). Для работы с журналами IIS можно использовать [С Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), которая включает в себя ряд встроенных запросов веб-служб Exchange.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_NextSteps"> </a>

Теперь, когда вы знаете об средства и ресурсы, которые можно использовать для устранения неполадок, может понадобиться справки, общие сведения о сведений, предоставленных эти средства. Ниже приведены некоторые способы получения справки:
  
- [Разработка для Exchange Server на форуме MSDN](http://social.msdn.microsoft.com/Forums/en-US/home?category=exchangeserver) — задайте вопрос сообщества разработчиков MSDN Exchange Server. 
    
- [Сайт StackOverflow](http://stackoverflow.com/tags/ews) — задайте вопрос StackOverflow сообщества. Убедитесь, что тег сообщение с «веб-служб Exchange». 
    
- [Службы поддержки Майкрософт](http://support.microsoft.com/ph/730/en-us) , обратитесь за помощью к специалисту службы поддержки Майкрософт. 
    
## <a name="see-also"></a>См. также


Можно в следующих статьях:
  
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Трассировка запросы и ответы для устранения неполадок в приложениях управляемый API EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
    
- [Оборудование клиентских запросов для веб-служб Exchange и REST в Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
- [Веб-служб Exchange регулирования в Exchange](ews-throttling-in-exchange.md)
    
- [Обновление сведений о конфигурации с помощью службы автообнаружения](how-to-refresh-configuration-information-by-using-autodiscover.md)
    
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)
    
- [Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с синхронизации в веб-служб Exchange в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удаления в веб-служб Exchange в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
- [Настройка ведения журнала в службах IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [Устранение неполадок в неудачных запросов с помощью трассировку в IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Краткие сведения о: Log Parser Studio](http://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Параметры по умолчанию для виртуальных каталогов Exchange](http://technet.microsoft.com/en-us/library/gg247612%28v=exchg.150%29.aspx)
    
Загрузите следующее:
  
- [Сетевой монитор Microsoft 3.4](http://www.microsoft.com/en-us/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler);
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [Веб-служб Exchange управляемого интерфейса API](http://go.microsoft.com/fwlink/?LinkID=255472)
    

