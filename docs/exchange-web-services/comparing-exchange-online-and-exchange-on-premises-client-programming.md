---
title: Сравнение программирования локальных клиентов Exchange Online и Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Узнайте о соображениях разработки для создания клиентского приложения EWS Managed API или EWS, которое работает Exchange Online и Exchange локально.
ms.openlocfilehash: 438965656e31eca586d06a5e0b6794c0eda87621
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512290"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Сравнение программирования локальных клиентов Exchange Online и Exchange

Узнайте о соображениях разработки для создания клиентского приложения EWS Managed API или EWS, которое работает Exchange Online и Exchange локально.
  
По большей части клиенты и веб-службы в Exchange, на которые они нацелены, будут работать одинаково независимо от того, является ли целевой объект Exchange Online, Exchange Online частью Office 365 или Exchange локального сервера. Однако существуют некоторые исключения, и необходимо убедиться, что ваше приложение может с ними справиться. Используйте сведения в этой статье, чтобы помочь вам спроектировать клиента, чтобы Exchange Online и Exchange локально.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Соображения программирования клиентов с автооткрытием

[Автооткрывка](autodiscover-for-exchange.md) предоставляет сведения о конфигурации для Exchange клиентов. Клиентские приложения могут обнаружить сведения о своей конфигурации одним из трех способов, в зависимости от того, Exchange Online или Exchange локального клиента. 
  
**Таблица 1. Типы и применимость служб автооткрытия Exchange**

|**Тип службы автооткрытия**|**Область применения**|
|:-----|:-----|
|[Служба автообнаружения SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online и версии Exchange локальной версии начиная с Exchange 2010 г.  <br/> |
|[Служба автообнаружения POX](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online и версии Exchange, начиная с Exchange 2007 г.  <br/> |
|[Точки подключения к службе (SCP)](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Версии Exchange, начиная с Exchange 2007 г.  <br/> |
   
Помимо сведений о конфигурации клиента, мыло и автооткрывка POX также возвращают версию Exchange службы и указывают, является ли эта служба Exchange Online. Эти сведения возвращаются в различных элементах в зависимости от типа используемого автонаружия.
  
**Таблица 2. Элементы автооткрытия, возвращающие версию службы и Exchange Online размещение информации**

|**Тип службы автооткрытия**|**Элемент XML, содержащий версию службы**|**Элемент XML, который указывает, есть ли у пользователя Exchange Online учетная запись**|
|:-----|:-----|:-----|
|Автообнаружение SOAP  <br/> |[Параметр (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) с текстовым **значением CasVersion.**  <br/> |[Параметр (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) с текстовым **значением UserMSOnline.**  <br/> |
|Автообнаружение POX  <br/> |[ServerVersion (POX)](https://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Убедитесь, что клиент получает эти сведения, [](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) чтобы он был нацелен на набор функций, доступный на Exchange сервере. Это может быть полезно для определения того, может ли клиент ожидать другого поведения в зависимости от того, находится ли почтовый ящик пользователя в локальной Exchange Online или Exchange локальной организации. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Тестирование и журнал файлов в приложениях, которые нацелены на Exchange Online

Exchange Online не предоставляет доступ к файлам журналов протоколов EWS, счетчикам производительности EWS и событиям службы, связанным с EWS, которые доступны на локальном Exchange серверах. Однако доступ к ним полезен при обнаружении работы приложения при взаимодействии с EWS. Убедитесь, что вы протестировали приложение на Exchange локальном сервере, чтобы оптимизировать его производительность. По возможности можно [](https://technet.microsoft.com/library/bb232205%28v=exchg.150%29.aspx#Policies) изменить параметры регулирования на тестовом сервере, чтобы соответствовать параметрам регулирования для Exchange Online, чтобы вы могли оценить, как будет вести себя ваше приложение при подключении к Exchange Online. 
  
> [!TIP]
> Вы можете использовать [средство EWSRelentless](https://ewsrelentless.codeplex.com/) для выполнения теста нагрузки EWS. Этот инструмент можно использовать с помощью тестового сервера, журналов протоколов EWS, счетчиков производительности EWS, событий службы и параметров регулирования EWS, чтобы лучше понять, как работает EWS при нагрузке. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Регулирование параметров и Exchange Online

Значения по умолчанию для параметров регулирования [EWS](ews-throttling-in-exchange.md) отличаются для Exchange Online, чем для Exchange локальной. Кроме того, невозможно изменить Exchange Online параметров регулирования. Для обнаружения параметров регулирования для Exchange локальной системы можно использовать Exchange management Shell. однако эти cmdlets не включены для Exchange Online. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Exchange Команды и параметры конфигурации управленческой оболочки

Ряд cmdlets может прямо или косвенно повлиять на API веб-службы в Exchange Online и Exchange локальном. Cmdlets не доступны для следующих в Exchange Online:
  
- Параметры регулирования 
    
- Параметры виртуального каталога 
    
- Параметры проверки подлинности
    
Подробные сведения о комлетах, доступных для Exchange Online, см. в [Exchange Online.](http://help.outlook.com/140/dd575549.aspx) Дополнительные данные о cmdlets, доступных Exchange локальной области, см. в Exchange [2013.](https://technet.microsoft.com/library/bb124413%28v=exchg.150%29.aspx)
  
## <a name="client-affinity-and-network-load-balancers"></a>Сродство клиентов и балансиры сетевых нагрузок
<a name="affinity"> </a>

Большинство сообщений EWS не требуют, чтобы клиент участвовал в сохранении сродства с Exchange. Подписки на события почтовых ящиков требуют, чтобы клиент предоставил файлы cookie и другие сведения для поддержания сродства с сервером Exchange, который поддерживает очередь событий почтовых ящиков для пользователя. Exchange Server 2010 г. с помощью exchangecookie поддерживается сродство клиентов в сетевых балансилях нагрузки. Exchange Online и версии Exchange, начиная с Exchange 2013 г., используют заголовку [X-AnchorMailbox, заголовку X-PreferServerAffinity и cookie X-BackEndOverrideCookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) для поддержания близости к уведомлениям почтовых ящиков. 
  
## <a name="authentication"></a>Проверка подлинности
<a name="auth"> </a>

Клиенты могут проверить подлинность Exchange Online с помощью Basic или OAuth. Версии локального Exchange, начиная с 2013 Exchange 2013 г., по умолчанию используют NTLM; однако можно настроить Exchange для использования базовой проверки подлинности. 
  
## <a name="client-latency-diagnostics"></a>Диагностика задержки клиента
<a name="diag"> </a>

Exchange Online собирает диагностику задержки клиента, если они сообщаются. Это помогает Корпорации Майкрософт поддерживать устранение проблем с подключением с помощью Exchange Online. Exchange не собирает диагностику задержки клиента. Если клиент нацелен Exchange локально, клиент не может сообщить серверу о диагностике задержки.
  
## <a name="functionality-in-the-ews-managed-api"></a>Функциональные возможности управляемого API EWS
<a name="ewsma"> </a>

Управляемый API EWS предоставляет некоторые функциональные возможности, которые специфичен для Exchange локального подключения, такие как просмотр точки подключения службы, а также некоторые функции, которые специфичен для Exchange Online, например отчеты о задержке клиента. Обратите внимание, что некоторые функции можно реализовать в Exchange Online, прежде чем они будут реализованы в управляемом API EWS. 
  
Следующие функции управляемого API EWS применимы только к Exchange Online:
  
- Отчеты о задержке клиента
    
- Базовая предварительная проверка подлинности
    
- Возможность запроса на возвращение RequestId в ответах
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Функции API в Exchange Online и Exchange Server выпусках
<a name="exo"> </a>

Различные наборы функций могут быть доступны в различных Office 365 и Exchange Online планах или в стандартных и корпоративных версиях Exchange Server. Следует помнить, что некоторые функции API могут быть недоступны для клиентского приложения в зависимости от Exchange Online или Exchange Server, в котором размещен почтовый ящик пользователя. 
   
Поскольку доступность функций может меняться, рекомендуется проверить Exchange Online и Exchange Server, чтобы оценить, как доступность функций может повлиять на клиента. Вы также можете создать клиента для проверки доступности компонентов с помощью [операции GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) или отправив тестовые запросы для операций, реализуя функции. Если функция недодоступна, ответ с сервера будет указан как таковой. 
  
## <a name="other-considerations"></a>Другие особенности
<a name="other"> </a>

Вы можете сделать следующее при Exchange локальном, но не Exchange Online:
  
- Создание клиента, установленного на Exchange сервере. 
    
- Установите [настраиваемые транспортные агенты,](../transport-agents/transport-agents-in-exchange-2013.md) которые могут повлиять на доставку и содержимое сообщений, которые вы создаете и отправляете с помощью EWS и других клиентов. 
    
## <a name="see-also"></a>См. также

- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
- [Сравнение Exchange Online и Exchange Server 2013 г.](https://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Сравнение всех Office 365 бизнес-планов](https://office.microsoft.com/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless — средство создания нагрузки EWS](https://ewsrelentless.codeplex.com/)
- [Доступность функции веб-службы API в Exchange и в Управляемом API EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [EWS регулирование в Exchange](ews-throttling-in-exchange.md)
    

