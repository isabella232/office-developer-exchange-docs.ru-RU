---
title: Оборудование клиентских запросов для веб-служб Exchange и REST в Exchange
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
localization_priority: Normal
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Сведения о заголовках HTTP в веб-служб Exchange и REST запросы и ответы, которые помогут вам мониторинг и устранение неполадок Exchange приложения.
ms.openlocfilehash: bcf362952c29956729c44397043a56bf3603d0af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761142"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Оборудование клиентских запросов для веб-служб Exchange и REST в Exchange

Сведения о заголовках HTTP в веб-служб Exchange и REST запросы и ответы, которые помогут вам мониторинг и устранение неполадок Exchange приложения.
  
Это никогда не произошло вам? Пользователь приложения отчетов произошла непредвиденная ошибка. Необходимо рассмотреть, но не удается воспроизвести его. Ошибка исчезла для пользователя, и вы получили очень маленьким другие необходимые сведения. Раздражающим, правда? Давайте рассмотрим, как заранее подготовить для этого сценария и надеюсь избежать проблему в будущем.
  
## <a name="add-instrumentation-to-requests"></a>Добавление инструментирования для запросов

Рекомендуется добавлять дополнительные заголовки HTTP для ваших запросов для облегчения устранения неполадок. Следует вести запись эти сведения, где-нибудь (например, в файл журнала), чтобы его можно получить более поздней версии, если необходимо. Функция полезна, если анализ сетевого трафика, а также полезна, если вы обратиться в службу поддержки корпорации Майкрософт для получения помощи.
  
**В таблице 1. Заголовки запроса для устранения неполадок**

|**Заголовок HTTP (EWS)**|**Управляемый API EWS эквивалент**|**Примечания**|
|:-----|:-----|:-----|
|Агент пользователя  <br/> |[ExchangeService.UserAgent](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |Значение уникальное значение, определяющее клиентского приложения.<br/><br/> Для всех запросов, которые приложение отправляет позволяет корпорации Майкрософт в устранении сбоями вызовов с использованием такого же значения, следует их возникновения.  <br/> |
|код запроса клиента  <br/> |[ExchangeService.ClientRequestId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |Значение разных уникальное значение приложение отправляет запрос.<br/><br/> Мы рекомендуем использовать GUID. Этот уникальный идентификатор предназначен для использования для соотнесения мероприятий между двумя системами в случае, если возникновения непредвиденных обстоятельств.  <br/> |
|Return-client--код запроса  <br/> |[ExchangeService.ReturnClientRequestId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |Задайте **значение true** для оповещения на сервере Exchange, что он должен возвращать значение запрос идентификатором клиента в соответствующем ответ.<br/><br/> Это можно использовать для соотнесения запросов и ответов в трассировку сети или трассировки управляемый API веб-служб Exchange.  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService.SendClientLatencies](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |Используется для [задержки EWS отчета](#bk_ReportLatency) в корпорацию Майкрософт, если приложение является доступа к Exchange Online или Exchange Online в составе Office 365.  <br/> |
   
## <a name="log-information-from-responses"></a>Сведения журнала из ответов на отчеты

Так же, как вашего клиента можно добавить дополнительные инструментария запросы, отправляемые им, Exchange добавляет дополнительные инструментария ответы в формате заголовки HTTP. Клиент должен сохранить эти сведения, чтобы перейти наряду со сведениями о инструментария запроса.
  
> [!NOTE]
> Если используется управляемый API EWS не имеет эквивалента прямое для заголовков HTTP. Тем не менее все заголовки HTTP-ответа осуществляется через свойство [ExchangeService.HttpResponseHeaders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) . 
  
**В таблице 2. Заголовки HTTP-ответа**

|**Заголовок HTTP**|**Описание**|
|:-----|:-----|
|код запроса  <br/> |Созданные сервером код запроса, соответствующий этой ответа.  <br/> |
|код запроса клиента  <br/> |Значение заголовка запроса идентификатор клиента в запросе.<br/><br/> В этом заголовке присутствует только в том случае, если запрос содержит заголовок return-client--код запроса, значение **true**.  <br/> |
|X-feserver.  <br/> |Полное доменное имя сервера клиентского доступа, обработку запроса.  <br/> |
|X-TargetBEServer  <br/> |Полное доменное имя сервера почтовых ящиков, обработку запроса.  <br/> |
|X-diaginfo.  <br/> |Дополнительную информацию, в зависимости от запроса.  <br/> |
|x-ms-diagnostics  <br/> | Этот заголовок применима только в том случае, если используется проверка подлинности OAuth в запросе.<br/><br/> Он содержит код явные ошибки, которая указывает причины сбоя проверки подлинности OAuth.<br/><br/> Она имеет следующий формат:`errorId;reason="reason"error_type="error type"`<br/><br/> Поле **Причина** — это понятное описание ошибки.<br/><br/> В поле **код ошибки** — целое число и **Ошибка\_тип** поле является строковое представление целого числа, как показано ниже:<ul><li>2000000: недопустимый\_подписи</li><li>2000001: недопустимый\_маркеров</li><li>  2000002: маркеров\_срока действия</li><li>2000003: недопустимый\_ресурсов</li><li>2000004: недопустимый\_клиента  </li><li>2000005: недопустимый\_пользователя</li><li>2000006: недопустимый\_клиента</li><li>2000007: внутренний\_об ошибках</li><li>2000008: недопустимый\_предоставить</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Отчет о задержке веб-служб Exchange в корпорацию Майкрософт
<a name="bk_ReportLatency"> </a>

Если приложение использует управляемый API EWS или веб-служб Exchange для подключения к Exchange Online, можно сообщить о задержке запросов веб-служб Exchange в непосредственно в корпорацию Майкрософт. Сведения передаются через заголовка X-ClientStatistics запроса. При использовании управляемого интерфейса API веб-служб Exchange все, что вам потребуется выполнить присвоено свойству [ExchangeService.SendClientLatencies](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) **значение true**. Если вы используете веб-служб Exchange, необходимо оценить с момента отправки запроса и ответа, а затем добавить заголовок X-ClientStatistics следующего запроса веб-служб Exchange, которые приложение отправляет в следующем формате.
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Мы Ведение отчетов для этих задержек и использовать их для постоянно повышать службы веб-служб Exchange в Exchange Online.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_ReportLatency"> </a>

После добавления инструментария клиентского приложения лучше подготовиться к Если возникновения непредвиденных обстоятельств. В этом случае можно использовать данные инструментирования для [устранения неполадок приложения](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md).
  
## <a name="see-also"></a>См. также

- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
- [Трассировка запросы и ответы для устранения неполадок в приложениях управляемый API EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

