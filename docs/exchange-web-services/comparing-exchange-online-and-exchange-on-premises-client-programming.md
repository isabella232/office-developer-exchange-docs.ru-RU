---
title: Сравнение Exchange Online и Exchange локальным клиентом для программирования
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Узнайте о вопросы проектирования для создания управляемый API EWS или клиентское приложение веб-служб Exchange, работающим с Exchange Online и локальную систему Exchange.
ms.openlocfilehash: 87c6ee476e06b50c339901bf61020b0fc98f8486
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760963"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Сравнение Exchange Online и Exchange локальным клиентом для программирования

Узнайте о вопросы проектирования для создания управляемый API EWS или клиентское приложение веб-служб Exchange, работающим с Exchange Online и локальную систему Exchange.
  
Для большей части, клиенты и веб-службы в Exchange, предназначенных для они будут работать так же, как независимо от того, является ли целевой объект является Exchange Online, Exchange Online в составе Office 365 или Exchange на локальном сервере. Существуют, однако некоторые исключения, и вы наверняка хотели бы убедитесь в том, что приложение может обрабатывать их. Используйте сведения в этой статье по проектированию вашего клиента для обоих Exchange Online и локальную систему Exchange.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Вопросы программирования клиента службы автообнаружения

[Автообнаружение](autodiscover-for-exchange.md) предоставляет сведения о конфигурации для клиентов Exchange. Клиентское приложение может получить сведения о конфигурации в одном из трех следующих способов в зависимости от того, является ли ориентация клиента Exchange Online или локальную систему Exchange. 
  
**В таблице 1. Типы службы автообнаружения и применимость Exchange**

|**Тип службы автообнаружения**|**Применимо к**|
|:-----|:-----|
|[Служба автообнаружения SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online и версии Exchange локальных начиная с Exchange 2010  <br/> |
|[Служба автообнаружения POX](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online и версии Exchange локальных начиная с Exchange 2007  <br/> |
|[Точка подключения службы поиска](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Версии Exchange локальных начиная с Exchange 2007  <br/> |
   
В дополнение к клиента сведения о конфигурации, что SOAP автообнаружения POX вернуть версию обновления Exchange и указывает, размещается ли служба с Exchange Online. Эти сведения возвращаются в различных элементов, в зависимости от типа использовании службы автообнаружения.
  
**В таблице 2. Элементы автоматического обнаружения, которые возвращают версию обновления и Exchange Online, информацию о размещении**

|**Тип службы автообнаружения**|**Элемент XML, который содержит версию обновления**|**Элемент XML, которое указывает, имеет ли пользователь учетную запись Exchange Online**|
|:-----|:-----|:-----|
|Автообнаружение SOAP  <br/> |[Параметр (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) в элемент Текстовое значение **CasVersion** .  <br/> |[Параметр (SOAP)](http://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) в элемент Текстовое значение **UserMSOnline** .  <br/> |
|Автообнаружение POX  <br/> |[ServerVersion (POX)](http://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Убедитесь, что ваш клиент позволяет получить сведения, чтобы его можно распределять [набор функций](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) , который доступен на сервере Exchange. Это может быть полезно для определения, является ли ваш клиент может предполагать по-разному зависимости от того, находится ли почтовый ящик пользователя в Exchange Online или Exchange в локальной организации. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Тестирование и файлов журналов в приложениях, предназначенных для Exchange Online

Exchange Online не предоставляет доступ к файлов журнала протокола веб-служб Exchange, счетчики производительности веб-служб Exchange и событий службы, связанные с веб-служб Exchange, доступных на локальных серверах Exchange. Доступ к ним полезен, однако в обнаружение как приложение выполняет при взаимодействии с веб-служб Exchange. Убедитесь, что тестирование приложения для тестирования на локальном сервере Exchange, таким образом, можно оптимизировать производительность. Если это возможно можно [Изменить параметры регулирования](http://technet.microsoft.com/en-us/library/bb232205%28v=exchg.150%29.aspx#Policies) на тестовом сервере для сопоставления параметры регулирования для Exchange Online, поэтому можно оценить поведение приложения при подключении к Exchange Online. 
  
> [!TIP]
> Средство [EWSRelentless](https://ewsrelentless.codeplex.com/) можно использовать для выполнения теста нагрузки веб-служб Exchange. Чтобы лучше понять, как веб-служб Exchange выполняется под нагрузкой можно использовать это средство с к тестовому серверу, журналы протоколов веб-служб Exchange, счетчики производительности веб-служб Exchange, службы событий и параметрами регулирования веб-служб Exchange. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Параметры регулирования и Exchange Online

Значения по умолчанию [Параметры регулирования веб-служб Exchange](ews-throttling-in-exchange.md) для разных для Exchange Online, чем для локальную систему Exchange. Кроме того нельзя изменить в Exchange Online, параметрами регулирования. Можно использовать командлеты командной консоли Exchange для обнаружения параметры регулирования для локальную систему Exchange; Тем не менее эти командлеты для Exchange Online не включены. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Командная консоль Exchange командлетов и параметров конфигурации

Число командлеты можно прямо или косвенно повлиять на API веб-службы в Exchange Online и Exchange локальной. Командлеты, недоступны для следующего в Exchange Online:
  
- Параметры регулирования 
    
- Параметры виртуального каталога 
    
- Параметры проверки подлинности
    
Для получения дополнительных сведений о командлетах, которые доступны для Exchange Online видеть [командлеты PowerShell в Exchange Online](http://help.outlook.com/en-us/140/dd575549.aspx). Дополнительные сведения о командлетах, которые доступны для локальную систему Exchange в разделе [командлеты Exchange 2013](http://technet.microsoft.com/en-us/library/bb124413%28v=exchg.150%29.aspx).
  
## <a name="client-affinity-and-network-load-balancers"></a>Сходства клиентов и сетевой подсистемы балансировки нагрузки
<a name="affinity"> </a>

Большинство связи веб-служб Exchange не требуется, что клиент участвовать в обслуживание сходства с сервером Exchange. Подписки на события почтового ящика требуется предоставить, что клиент файлы cookie и другие сведения на обслуживание сходства с Exchange server, который поддерживает очереди событий почтового ящика для пользователя. Exchange Server 2010 использует exchangecookie для поддержания сходства клиентов между балансировки сетевой нагрузки. Exchange Online и версии Exchange локальных начиная с Exchange 2013 используйте [заголовок X-AnchorMailbox, заголовок X-PreferServerAffinity и X BackEndOverrideCookie файл cookie](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) для обеспечения соответствия для уведомления почтового ящика. 
  
## <a name="authentication"></a>Аутентификация
<a name="auth"> </a>

Клиенты могут проходить проверку подлинности с Exchange Online с помощью Basic или OAuth. Версии Exchange в локальной начиная с Exchange 2013 используют NTLM по умолчанию; Тем не менее можно настроить локальную систему Exchange для использования обычной проверки подлинности также. 
  
## <a name="client-latency-diagnostics"></a>Диагностика задержка клиента
<a name="diag"> </a>

Exchange Online собирает диагностику задержка клиента, если они отображаются. Это помогает устранения неполадок подключения к с Exchange Online службы поддержки Майкрософт. Локальную систему Exchange не собирает диагностику задержка клиента. Если ваш клиент относится локальную систему Exchange, клиент не может сообщить о диагностики задержки на сервере.
  
## <a name="functionality-in-the-ews-managed-api"></a>Управляемый API функции в веб-служб Exchange
<a name="ewsma"> </a>

Управляемый API веб-служб Exchange предоставляет некоторые функциональные возможности, характерные для локальную систему Exchange, например подстановки точки подключения службы и некоторые функциональные возможности, необходимые для Exchange Online, таких как reporting задержка клиента. Обратите внимание на то, что существует возможность некоторые функциональные возможности для реализации в Exchange Online перед реализована в управляемый API веб-служб Exchange. 
  
Следующие функциональные возможности управляемый API EWS применима только к Exchange Online:
  
- Отчеты задержка клиента
    
- Базовая предварительной проверки подлинности
    
- Возможность запроса, что RequestId возвращаться в ответы
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Функции API в Exchange Online планы и версии Exchange Server
<a name="exo"> </a>

Наборы различных компонентов могут быть доступны в различных планов Office 365 и Exchange Online или в стандартный и корпоративных версий Exchange Server. Обратите внимание, что некоторые функциональные возможности API могут быть недоступны для клиентского приложения в зависимости от Exchange Online — план или версии Exchange Server, на котором размещен почтовый ящик пользователя. 
  
**В таблице 3. Функция вариантов API через планы и выпуски**

|**Функции API**|**Сведения о выполнении плана или выпуска**|
|:-----|:-----|
|Веб-служб Exchange получить доступ к учетным записям, за исключением через олицетворения Exchange  <br/> |Не допускается в [Office 365 для бизнеса, планы киоска](http://office.microsoft.com/en-us/business/compare-office-365-kiosk-plans-FX103178917.aspx).  <br/> |
|Единая система обмена сообщениями  <br/> |Доступны только в план, Exchange Online план 2 и Exchange Server 2013 корпоративных версий Office 365 корпоративный (E3).  <br/> |
|Интеграция с Active Directory доменных служб (AD DS)  <br/> |Недоступно, с помощью Office 365 для малого бизнеса и Office 365 для малого бизнеса расширенный плана.  <br/> |
|Управление правами на доступ, архивации и юридических удержаний  <br/> |Доступны только в планах Office 365 корпоративный (E3 и E4).  <br/> |
|Защита от потери данных  <br/> |Доступны только в планах Office 365 для предприятия, Exchange Online (план 2) и Exchange Server 2013 корпоративных версий.  <br/> |
   
Доступность функций можно изменить, поэтому рекомендуется установить Exchange Online планы и версиях Exchange Server, чтобы оценить, как доступность функций может повлиять на клиенте. Можно также создать клиента для проверки доступности функций с помощью [операции GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) или отправлять запросы тестирования для операций, которые реализуют функции. Если компонент недоступен, ответ от сервера указывает таким образом. 
  
## <a name="other-considerations"></a>Другие рекомендации
<a name="other"> </a>

Вы можете выполнять следующие действия при определении Exchange в локальной, но не в Exchange Online:
  
- Создание клиента, установленные на сервере Exchange. 
    
- Установка [настраиваемых транспортных агентов](../transport-agents/transport-agents-in-exchange-2013.md) , которые могут влиять на доставки и содержимого сообщений, создание и отправка с помощью веб-служб Exchange и других клиентских программах. 
    
## <a name="see-also"></a>См. также

- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
- [Сравнение Exchange Online и Exchange Server 2013](http://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Сравнение всех планов Office 365 для бизнес-планы](http://office.microsoft.com/en-us/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [EwsRelentless - средства создания нагрузки веб-служб Exchange](https://ewsrelentless.codeplex.com/)
- [Доступность функций API службы Web в Exchange и управляемый API веб-служб Exchange](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [Веб-служб Exchange регулирования в Exchange](ews-throttling-in-exchange.md)
    

