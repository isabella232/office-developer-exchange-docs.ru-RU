---
title: Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: ee7fcd05-35d7-47bf-bac4-e719c49c11fe
description: Найдите ресурсы, которые помогут устранить неполадки в управляемом API EWS или приложении EWS.
localization_priority: Priority
ms.openlocfilehash: 8a65b06cf911cd033d7fe5fe1b4566a7496de784
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542584"
---
# <a name="tools-and-resources-for-troubleshooting-ews-applications-for-exchange"></a>Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange

Найдите ресурсы, которые помогут устранить неполадки в управляемом API EWS или приложении EWS.
  
Не всегда все идет по плану. Иногда запросы EWS терпят сбой или дают неожиданные результаты. Это может быть неприятно, особенно если причина не очевидна. Надеюсь, с вами этого никогда не случится, но если это произойдет, в этой статье содержатся сведения об инструментах и ресурсах, которые можно использовать для устранения неполадок.
  
> [!NOTE]
> В этой статье представлены общие советы по устранению неполадок и источники информации по устранению неполадок. К сожалению, невозможно предоставить подробные действия по устранению неполадок. Подробнее о помощи в устранении конкретной ошибки см. в разделе [Дальнейшие действия](#bk_NextSteps). 
  
## <a name="examine-the-soap-requests-and-responses"></a>Изучение запросов и ответов SOAP

Если что-то работает неправильно, это помогает понять, что происходит. Первая линия запроса при исследовании проблемы с EWS или управляемым API EWS — это проверка запросов, которые приложение отправляет по сети, и ответов, которые сервер отправляет обратно.
  
Управляемый API EWS упрощает изучение запросов и ответов SOAP с помощью [встроенных функций трассировки](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md). Если вы используете EWS, у вас может быть или не быть доступа к аналогичным функциям трассировки, в зависимости от того, какую платформу или классы вы используете для отправки запросов. Однако вы всегда можете использовать средство трассировки сети, такой как [сетевой монитор](https://www.microsoft.com/download/details.aspx?id=4865) или[Fiddler](http://www.telerik.com/fiddler), для проверки сетевого трафика и просмотра полезных данных запроса и ответа. 
  
Кроме того, вы можете [инструментировать клиентские запросы](instrumenting-client-requests-for-ews-and-rest-in-exchange.md) для улучшения сведений, доступных в запросах и ответах. 
  
После получения запросов и ответов, задайте себе следующий вопрос: правильно ли они выглядят? Ожидаются ли значения, которые отправляет ваше приложение? Есть ли смысл в ответах?
  
## <a name="examine-error-codes"></a>Проверка кодов ошибок

Иногда код ошибки может иметь большое значение для определения проблемы, даже если на первый взгляд это не имеет смысла. Указывает ли ошибка на то, что ваш клиент [отрегулирован](ews-throttling-in-exchange.md)? Возможно, следует обратиться в автообнаружение для [обновления сведений о конфигурации](how-to-refresh-configuration-information-by-using-autodiscover.md)? 
  
Дополнительные сведения об обработке определенных ошибок см. в перечисленных ниже статьях.
  
- [Обработка сообщений об ошибках службы автообнаружения](handling-autodiscover-error-messages.md)
    
- [Обработка ошибок, связанных с уведомлениями, в EWS в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с синхронизацией, в EWS в Exchange](handling-synchronization-related-errors-in-ews-in-exchange.md)
    
- [Обработка ошибок, связанных с удалением, в EWS в Exchange](handling-deletion-related-errors-in-ews-in-exchange.md)
    
## <a name="verify-versions"></a>Проверка версий

В операциях EWS участвует ряд различных компонентов, и версии этих компонентов могут влиять на результаты.
  
**Таблица 1. Компоненты с поддержкой версий, которые могут влиять на процессы EWS**

|**Компонент**|**Управляемый API EWS**|**EWS**|**Примечания**|
|:-----|:-----|:-----|:-----|
|Запрашиваемая версия сервера  <br/> |Свойство [ExchangeServiceBase.RequestedServerVersion](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx)  <br/> |Элемент [RequestServerVersion](https://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx)  <br/> |Это значение определяет, какая версия схемы EWS используется для обработки запроса EWS. Убедитесь, что указанная здесь версия схемы подходит для отправляемого запроса. Некоторые свойства и операции недоступны в более ранних версиях схемы.  <br/> |
|Версия сервера  <br/> |Свойство [ExchangeServiceBase.ServerInfo](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.serverinfo%28v=exchg.80%29.aspx)  <br/> |Элемент [ServerVersionInfo](https://msdn.microsoft.com/library/c04a6872-ca27-432b-aac2-36b023d0afc6%28Office.15%29.aspx)  <br/> |Это значение возвращается сервером в ответах EWS и указывает версию сервера, обработавшего ответ. Убедитесь, что это значение соответствует вашим ожиданиям. По возможности убедитесь, что на сервере Exchange установлено самое последнее обновление для основной версии Exchange.  <br/> |
|Версия управляемого API EWS  <br/> |Свойство версии продукта файла Microsoft.Exchange.WebServices.dll.  <br/> |Неприменимо  <br/> |Если вы используете управляемый API EWS, убедитесь, что вы используете [самую последнюю версию](https://aka.ms/ews-managed-api-readme).  <br/> |
   
## <a name="verify-access"></a>Проверка доступа

EWS включен по умолчанию, но [значения по умолчанию можно изменить](how-to-control-access-to-ews-in-exchange.md). Используйте командлет [Get-OrganizationConfig](https://technet.microsoft.com/library/bb124754.aspx), чтобы убедиться, что EWS включен на сервере, и командлет [Get-CASMailbox](https://technet.microsoft.com/library/aa997571.aspx), чтобы убедиться, что EWS включен для почтового ящика пользователя. Также проверьте оба ответа командлета на наличие разрешенного или заблокированного списка EWS и убедитесь, что ваше приложение не заблокировано для использования EWS. 
  
Необходимо также убедиться, что [параметры проверки подлинности по умолчанию](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx) в виртуальном каталоге EWS не были изменены. 
  
## <a name="try-another-ews-client"></a>Попробуйте другой клиент EWS

Иногда полезно попробовать тот же запрос от другого клиента и сравнить результаты. Если другой клиент получает другие результаты, что изменится? Выявление различий между успешным и неудачным запросом может помочь объяснить, почему конкретный запрос не выполняется.
  
Конечно, вы можете написать другого клиента для проверки, но это не обязательно! [EWSEditor](http://ewseditor.codeplex.com/) — это пример клиента, который использует управляемый API EWS и EWS. Вы можете загрузить клиент (включая исходный код) и использовать его для выполнения тех же запросов, которые не работают в вашем приложении. 
  
## <a name="examine-iis-logs"></a>Изучение журналов IIS

Если у вас есть доступ к серверу Exchange, функция ведения журнала, предоставляемая службами IIS на серверах клиентского доступа, могут предоставлять дополнительные сведения о сбоях. Однако имейте в виду, что журналы IIS будут полезны только при получении ошибки HTTP.
  
IIS предоставляет два различных метода ведения журнала: [ведение журнала IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis) и [отслеживание неудачных запросов](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis). Для работы с журналами IIS можно использовать [Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx), которая включает ряд встроенных запросов EWS.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_NextSteps"> </a>

Теперь, когда вы узнали об инструментах и ресурсах, которые можно использовать для устранения неполадок, вам может потребоваться помощь в понимании информации, предоставляемой этими средствами. Ниже приведены некоторые варианты получения справки:
  
- [Форум разработчиков Exchange Server в MSDN](https://social.msdn.microsoft.com/Forums/home?category=exchangeserver) — задайте вопрос сообществу разработчиков Exchange Server MSDN. 
    
- [StackOverflow](http://stackoverflow.com/tags/ews) — задайте вопрос сообществу StackOverflow. Обязательно пометьте свой пост "EWS". 
    
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
    
- [Настройка журнала в IIS](http://www.iis.net/learn/manage/provisioning-and-managing-iis/configure-logging-in-iis)
    
- [Устранение неполадок с невыполненными запросами с помощью трассировки в IIS 7](http://www.iis.net/learn/troubleshoot/using-failed-request-tracing/troubleshooting-failed-requests-using-tracing-in-iis)
    
- [Введение: Log Parser Studio](https://blogs.technet.com/b/exchange/archive/2012/03/07/introducing-log-parser-studio.aspx)
    
- [Параметры по умолчанию для виртуальных каталогов Exchange](https://technet.microsoft.com/library/gg247612%28v=exchg.150%29.aspx)
    
Скачайте следующее:
  
- [Сетевой монитор Microsoft 3.4](https://www.microsoft.com/download/details.aspx?id=4865)
    
- [Fiddler](http://www.telerik.com/fiddler)
    
- [EWSEditor](http://ewseditor.codeplex.com/)
    
- [Управляемый API веб-служб Exchange](https://www.nuget.org/packages/Microsoft.Exchange.WebServices/)
