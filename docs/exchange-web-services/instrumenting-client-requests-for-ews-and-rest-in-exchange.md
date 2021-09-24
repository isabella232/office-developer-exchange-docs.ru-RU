---
title: Инструментирование запросов клиентов для EWS и REST в Exchange
manager: sethgros
ms.date: 4/13/2016
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 330de503-498d-447e-b4a9-c20fc1699fd1
description: Узнайте о загонах HTTP в запросах и ответах EWS и REST, которые помогут вам отслеживать и устранять Exchange приложение.
ms.openlocfilehash: f32a164436a1f8ab06192e71a287f5092fe9a6c4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520992"
---
# <a name="instrumenting-client-requests-for-ews-and-rest-in-exchange"></a>Инструментирование запросов клиентов для EWS и REST в Exchange

Узнайте о загонах HTTP в запросах и ответах EWS и REST, которые помогут вам отслеживать и устранять Exchange приложение.
  
С вами такое случалось? Пользователь приложения сообщает о неожиданной ошибке. Вы хотите исследовать, но вы не можете воспроизвести его. Ошибка исчезла для пользователя, и у вас осталось очень мало действий данных. Разочарование, не так ли? Давайте рассмотрим, как можно активно подготовиться к этому сценарию и, надеюсь, избежать разочарований в будущем.
  
## <a name="add-instrumentation-to-requests"></a>Добавление инструментов в запросы

Мы рекомендуем добавить дополнительные http-заготки в запросы для облегчения устранения неполадок. Вы должны хранить запись этой информации где-то (например, в файле журнала), чтобы вы могли получить ее позже, если это необходимо. Это полезно при анализе сетевого трафика, а также полезно, если вы обратитесь за помощью в службу поддержки Майкрософт.
  
**Таблица 1. Запрос заглавных заглавок для устранения неполадок**

|**Http header (EWS)**|**Эквивалент управляемого API EWS**|**Примечания**.|
|:-----|:-----|:-----|
|User-Agent  <br/> |[ExchangeService.UserAgent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.useragent%28v=exchg.80%29.aspx) <br/> |Установите это уникальное значение, которое идентифицирует клиентскую заявку.<br/><br/> Использование одинакового значения для всех запросов, которые отправляет приложение, позволяет Корпорации Майкрософт в случае их возникновения помочь устранить сбои вызовов.  <br/> |
|client-request-id  <br/> |[ExchangeService.ClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.clientrequestid%28v=exchg.80%29.aspx) <br/> |Установите для каждого запроса, который отправляет приложение, другое уникальное значение.<br/><br/> Рекомендуется использовать GUID. Этот уникальный идентификатор предназначен для сопоставления действий между двумя системами в случае, если что-то пойдет не так.  <br/> |
|return-client-request-id  <br/> |[ExchangeService.ReturnClientRequestId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.returnclientrequestid%28v=exchg.80%29.aspx) <br/> |Установите значение **true,** чтобы сигнализировать Exchange серверу о том, что в соответствующем ответе оно должно возвращать значение вашего клиента-запроса.<br/><br/> Это можно использовать для сопоставления запросов и ответов в сетевых трассировок или трассировок управляемого API EWS.  <br/> |
|X-ClientStatistics  <br/> |[ExchangeService.SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) <br/> |Используется для сообщения о задержках [EWS](#bk_ReportLatency) в Корпорации Майкрософт, если приложение Exchange Online или Exchange Online в Office 365.  <br/> |
   
## <a name="log-information-from-responses"></a>Сведения о журнале из ответов

Так же, как клиент может добавить дополнительную аппаратуру к отправляемым запросам, Exchange добавляет дополнительные инструменты в ответы в виде http headers. Клиент должен зафиксировать эти сведения, чтобы получить сведения об инструментах запроса.
  
> [!NOTE]
> Если вы используете управляемый API EWS, нет прямого эквивалента для http-заглав. Однако все заголовок ответов HTTP можно получить через свойство [ExchangeService.HttpResponseHeaders.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.httpresponseheaders%28v=exchg.80%29.aspx) 
  
**Таблица 2. Http response headers**

|**Http header**|**Описание**|
|:-----|:-----|
|request-id  <br/> |Созданный сервером ID для запроса, соответствующего этому ответу.  <br/> |
|client-request-id  <br/> |Значение заглавного руководителя клиента-запроса в запросе.<br/><br/> Этот заглавный заготок присутствует только в том случае, если запрос содержит заглавную ссылку return-client-request-id со значением **true**.  <br/> |
|X-FEServer  <br/> |FQDN сервера клиентского доступа, обрабатываемого запросом.  <br/> |
|X-TargetBEServer  <br/> |FQDN сервера почтовых ящиков, обрабатываемого запросом.  <br/> |
|X-DiagInfo  <br/> |Дополнительные диагностические сведения в зависимости от запроса.  <br/> |
|x-ms-diagnostics  <br/> | Этот заголовок применим только в том случае, если в запросе используется проверка подлинности OAuth.<br/><br/> Он содержит явный код ошибки, который указывает причины сбой проверки подлинности OAuth.<br/><br/> Требуется следующий формат: `errorId;reason="reason"error_type="error type"`<br/><br/> Поле **причины** — это понятное человеку описание ошибки.<br/><br/> Поле **errorId** — это рядное, **\_** а поле типа ошибки представляет строковую репрезентативность этого integer следующим образом:<ul><li>2000000: недействительный \_ подписи</li><li>2000001: недействительный \_ маркер</li><li>  2000002: срок \_ действия маркера истек</li><li>2000003: недействительный \_ ресурс</li><li>2000004: недействительный \_ клиент  </li><li>2000005: недействительный \_ пользователь</li><li>2000006: недействительный \_ клиент</li><li>2000007: внутренняя \_ ошибка</li><li>2000008: недействительный \_ грант</li></ul> |
   
## <a name="report-ews-latency-to-microsoft"></a>Отчет о задержке EWS в Корпорации Майкрософт
<a name="bk_ReportLatency"> </a>

Если ваше приложение использует управляемый API EWS или EWS для подключения к Exchange Online, вы можете сообщить о задержке в запросах EWS непосредственно в Корпорацию Майкрософт. Информация передается через заглавную заглавную запроса X-ClientStatistics. Если вы используете управляемый API EWS, все, что вам нужно сделать, это установить свойство [ExchangeService.SendClientLatencies](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.sendclientlatencies%28v=exchg.80%29.aspx) к **true**. Если вы используете EWS, необходимо измерить время между выдачей запроса и получением ответа, а затем добавить заглавную головку X-ClientStatistics в следующий запрос EWS, который отправляет ваше приложение, используя следующий формат.
  
`X-ClientStatistics: MessageId=<value of request-id header>,ResponseTime=<time in milliseconds>,SoapAction=<EWS operation>`
  
Мы поддерживаем отчеты об этих задержках и используем их для непрерывного улучшения служб EWS в Exchange Online.
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_ReportLatency"> </a>

После того как в приложение добавлена клиентская аппаратура, вы будете лучше подготовлены, если что-то пойдет не так. Если это произойдет, вы можете использовать данные приборов для [устранения неполадок в приложении.](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
  
## <a name="see-also"></a>См. также

- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
- [Трассировка запросов и ответов для устранения неполадок в приложениях управляемого API EWS](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md)
- [Инструменты и ресурсы для устранения неполадок приложений EWS для Exchange](tools-and-resources-for-troubleshooting-ews-applications-for-exchange.md)
    

