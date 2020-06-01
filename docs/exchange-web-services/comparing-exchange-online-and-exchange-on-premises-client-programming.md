---
title: Сравнение программирования локальных клиентов Exchange Online и Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3c2eabe4-52bc-461e-a6dd-f65f22f16e50
description: Сведения о проектировании для создания управляемого API EWS или клиентского приложения EWS, работающего в локальной среде Exchange Online и Exchange.
ms.openlocfilehash: 8b4dbae5cadfed377aa3a7179144a7cea68bc35c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456166"
---
# <a name="comparing-exchange-online-and-exchange-on-premises-client-programming"></a>Сравнение программирования локальных клиентов Exchange Online и Exchange

Сведения о проектировании для создания управляемого API EWS или клиентского приложения EWS, работающего в локальной среде Exchange Online и Exchange.
  
В большинстве случаев клиенты и веб-службы в Exchange, для которых они предназначены, будут работать одинаково независимо от того, является ли целевой сервер Exchange Online, Exchange Online в составе Office 365 или локального сервера Exchange. Однако существуют некоторые исключения, и вы хотите убедиться, что приложение может их обработать. Сведения, приведенные в этой статье, помогут вам разрабатывать клиент для работы как в Exchange Online, так и в локальной среде Exchange.

<a name="autodiscover"> </a>

## <a name="autodiscover-client-programming-considerations"></a>Рекомендации по программированию клиента автообнаружения

Служба [автообнаружения](autodiscover-for-exchange.md) предоставляет сведения о конфигурации для клиентов Exchange. Клиентское приложение может обнаружить сведения о конфигурации одним из трех способов в зависимости от того, предназначен ли клиент для Exchange Online или Exchange локально. 
  
**Таблица 1. Типы службы автообнаружения и применимости Exchange**

|**Тип службы автообнаружения**|**Относится к**|
|:-----|:-----|
|[Служба автообнаружения SOAP](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online и версии локального Exchange, начиная с Exchange 2010  <br/> |
|[Служба автообнаружения POX](autodiscover-for-exchange.md#bk_Options) <br/> |Exchange Online и версии локального Exchange, начиная с Exchange 2007  <br/> |
|[Поиск точки подключения службы (SCP)](how-to-find-autodiscover-endpoints-by-using-scp-lookup-in-exchange.md) <br/> |Версии локального Exchange, начиная с Exchange 2007  <br/> |
   
В дополнение к сведениям о конфигурации клиента, что служба автообнаружения SOAP и POX также возвращает версию службы Exchange и указывает, размещена ли служба в Exchange Online. Эти сведения возвращаются в разных элементах в зависимости от типа используемого автообнаружения.
  
**Таблица 2. Элементы автообнаружения, возвращающие версию службы и сведения о размещении Exchange Online**

|**Тип службы автообнаружения**|**Элемент XML, который содержит версию службы**|**XML-элемент, указывающий наличие у пользователя учетной записи Exchange Online**|
|:-----|:-----|:-----|
|Автообнаружение SOAP  <br/> |Элемент [Setting (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) с текстовым значением **касверсион** .  <br/> |Элемент [Setting (SOAP)](https://msdn.microsoft.com/library/43db26e1-f7be-49fd-b26b-fc1b10bd3458%28Office.15%29.aspx) с текстовым значением **усермсонлине** .  <br/> |
|Автообнаружение POX  <br/> |[Серверверсион (POX)](https://msdn.microsoft.com/library/2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a%28Office.15%29.aspx) <br/> |**MicrosoftOnline** <br/> |
   
Убедитесь, что клиент захватывает эти сведения, чтобы он мог использовать [набор функций](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md) , доступный на сервере Exchange. Это может быть полезно, чтобы определить, может ли ваш клиент ожидать различных действий в зависимости от того, находится ли почтовый ящик пользователя в локальной организации Exchange Online или Exchange. 

<a name="testing"> </a>

## <a name="testing-and-log-files-in-applications-that-target-exchange-online"></a>Тестирование файлов и журналов в приложениях, предназначенных для Exchange Online

Exchange Online не предоставляет доступ к файлам журнала протокола EWS, счетчикам производительности EWS и событиям служб, связанным с EWS, которые доступны на локальных серверах Exchange. Тем не менее, доступ к ним полезен для обнаружения того, как ваше приложение работает при взаимодействии с EWS. Убедитесь, что приложение тестируется на локальном сервере Exchange, чтобы вы могли оптимизировать его производительность. Если это возможно, вы можете [изменить параметры регулирования](https://technet.microsoft.com/library/bb232205%28v=exchg.150%29.aspx#Policies) на тестовом сервере в соответствии с параметрами регулирования для Exchange Online, чтобы вы могли оценить, как приложение будет вести себя при подключении к Exchange Online. 
  
> [!TIP]
> С помощью средства [евсрелентлесс](https://ewsrelentless.codeplex.com/) можно выполнить нагрузочный тест EWS. Это средство можно использовать с тестовым сервером, журналами протокола EWS, счетчиками производительности EWS, событиями служб и настройками регулирования EWS, чтобы лучше понять, как работает служба EWS под нагрузкой. 

<a name="throttling"> </a>

## <a name="throttling-settings-and-exchange-online"></a>Параметры регулирования и Exchange Online

Значения по умолчанию для [параметров регулирования EWS](ews-throttling-in-exchange.md) для Exchange Online отличаются от значений по умолчанию для локальной службы Exchange. Кроме того, вы не можете изменить параметры регулирования Exchange Online. С помощью командлетов командной консоли Exchange можно определить параметры регулирования для локального сервера Exchange; Тем не менее, эти командлеты не включены для Exchange Online. 

<a name="ems"> </a>

## <a name="exchange-management-shell-cmdlets-and-configuration-settings"></a>Командлеты командной консоли Exchange и параметры конфигурации

Несколько командлетов могут напрямую или косвенно повлиять на API веб-служб в Exchange Online и в локальной среде Exchange. Командлеты недоступны для следующих компонентов в Exchange Online:
  
- Параметры регулирования 
    
- Параметры виртуального каталога 
    
- Параметры проверки подлинности
    
Для получения дополнительных сведений о командлетах, доступных для Exchange Online, обратитесь к [командлетам PowerShell в Exchange Online](http://help.outlook.com/140/dd575549.aspx). Дополнительные сведения о командлетах, доступных для локальной организации Exchange, можно найти в статье [командлеты exchange 2013](https://technet.microsoft.com/library/bb124413%28v=exchg.150%29.aspx).
  
## <a name="client-affinity-and-network-load-balancers"></a>Сходство клиентов и подсистемы балансировки нагрузки сети
<a name="affinity"> </a>

Для большей части взаимодействия EWS не требуется, чтобы клиент участвовал в обслуживании соответствия с Exchange. Для подписки на события почтовых ящиков необходимо, чтобы клиент предоставил файлы cookie и другие сведения для поддержки сходства с сервером Exchange Server, поддерживающим очередь событий почтовых ящиков для пользователя. Сервер Exchange Server 2010 использует ексчанжекукие для поддержания сходства клиентов между подсистемами балансировки нагрузки сети. Exchange Online и версии локального Exchange, начиная с Exchange 2013 [, используют заголовок x-AnchorMailbox, заголовок x-преферсервераффинити и файл cookie x-баккендоверридекукие](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md#bk_howmaintained) для сохранения сходства для уведомлений почтовых ящиков. 
  
## <a name="authentication"></a>Аутентификация
<a name="auth"> </a>

Клиенты могут проходить проверку подлинности в Exchange Online с помощью Basic или OAuth. Версии локального Exchange, начиная с Exchange 2013, используют NTLM по умолчанию; Тем не менее, для локальной проверки подлинности можно также настроить использование обычной проверки подлинности. 
  
## <a name="client-latency-diagnostics"></a>Диагностика задержки клиентов
<a name="diag"> </a>

Exchange Online собирает диагностические сведения о задержке клиентов, если они выдаются. Это помогает корпорации Майкрософт в поддержке проблем с подключением к Exchange Online. В локальной среде Exchange не выполняется сбор диагностических сведений о задержке клиентов. Если клиент ориентирован на локальную среду Exchange, клиент не может сообщать о задержке на сервере.
  
## <a name="functionality-in-the-ews-managed-api"></a>Функции в управляемом API EWS
<a name="ewsma"> </a>

Управляемый API EWS предоставляет некоторые функциональные возможности, характерные для локальной среды Exchange, например поиск подключения к точке обслуживания, а также некоторые функции, характерные для Exchange Online, например отчеты о задержке клиентов. Обратите внимание на то, что некоторые функции можно реализовать в Exchange Online, прежде чем она будет реализована в управляемом API EWS. 
  
Следующие функции управляемого API EWS относятся только к Exchange Online:
  
- Отчеты о задержке клиентов
    
- Базовая Предварительная проверка подлинности
    
- Возможность запросить возврат ИД запроса в ответах
    
## <a name="api-features-in-exchange-online-plans-and-exchange-server-editions"></a>Функции API в планах Exchange Online и Exchange Server Editions
<a name="exo"> </a>

Разные наборы функций могут быть доступны в разных планах Office 365 и Exchange Online, а также в стандартных и корпоративных версиях Exchange Server. Имейте в виду, что некоторые функции API могут быть недоступны для клиентского приложения в зависимости от плана Exchange Online или Exchange Server Edition, на котором размещается почтовый ящик пользователя. 
  
**Таблица 3. Варианты функций API в планах и выпусках**

|**Функция API**|**Рекомендации по планированию или выпуску**|
|:-----|:-----|

| Доступ к учетным записям с помощью EWS, кроме олицетворения Exchange  <br/> | Не разрешено в [Office 365 для бизнеса — планы киосков](https://office.microsoft.com/business/compare-office-365-kiosk-plans-FX103178917.aspx).  <br/> |


| Единая система обмена сообщениями (UM)  <br/> | Доступно только в планах Office 365 Enterprise (E3), Exchange Online (план 2) и Exchange Server 2013 Enterprise Editions.  <br/> | | Интеграция с доменными службами Active Directory (AD DS)  <br/> | Недоступно в плане Office 365 для малого бизнеса и Office 365 для малого бизнеса расширенный.  <br/> | | Управление правами на доступ к данным, Архивация и юридические удержания  <br/> | Доступно только в планах Office 365 Enterprise (E3 и E4).  <br/> | | Защита от потери данных  <br/> | Доступно только в планах Office 365 для предприятий, Exchange Online (план 2) и Exchange Server 2013 для корпоративных выпусков.  <br/> |
   
Так как доступность функций может измениться, рекомендуется проверить возможности планов Exchange Online и Exchange Server, чтобы оценить, как доступность функций может повлиять на ваш клиент. Вы также можете разработать свой клиент для проверки доступности функций с помощью [операции GetServiceConfiguration](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) или путем отправки тестовых запросов для операций, реализующих эти функции. Если функция недоступна, ответ сервера будет указываться таким образом. 
  
## <a name="other-considerations"></a>Другие особенности
<a name="other"> </a>

Вы можете выполнить следующие действия при нацелении на локальную систему Exchange, но не Exchange Online:
  
- Создайте клиент, установленный на сервере Exchange. 
    
- Установите [Настраиваемые агенты транспорта](../transport-agents/transport-agents-in-exchange-2013.md) , которые могут повлиять на доставку и содержимое сообщений, которые вы создаете и отправляете с помощью EWS и других клиентов. 
    
## <a name="see-also"></a>См. также

- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
- [Сравнение Exchange Online и Exchange Server 2013](https://blogs.technet.com/b/exchange/archive/2012/09/19/comparing-exchange-online-and-exchange-server-2013.aspx)  
- [Сравнение планов Office 365 для бизнеса](https://office.microsoft.com/business/compare-all-office-365-for-business-plans-FX104051403.aspx)
- [Евсрелентлесс — средство создания нагрузки EWS](https://ewsrelentless.codeplex.com/)
- [Доступность функции веб-службы API в Exchange и в Управляемом API EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)
- [EWS регулирование в Exchange](ews-throttling-in-exchange.md)
    

