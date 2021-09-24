---
title: Настройка параметров для EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: Сведения о параметрах конфигурации, к которые может получить доступ клиент EWS, и настраиваемых параметрах Exchange, которые могут повлиять на клиента EWS.
ms.openlocfilehash: ed7667086b36897fd07031526e5a4657a120d505
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522287"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Настройка параметров для EWS в Exchange

Сведения о параметрах конфигурации, к которые может получить доступ клиент EWS, и настраиваемых параметрах Exchange, которые могут повлиять на клиента EWS. 
  
Многие параметры конфигурации могут повлиять на работу клиентского приложения EWS. Эти параметры конфигурации: 
  
- Только для чтения или для чтения с клиентом.
    
- Доступ на сервере Exchange, на котором размещена служба EWS.
    
Клиент может получить доступ к Exchange Online, Exchange Online как часть Office 365, так и локальному Exchange серверу. Все локальное Exchange серверов доступны Exchange администраторам; однако не все эти параметры доступны администраторам Exchange Online клиентов. В этой статье описывается, какие параметры конфигурации могут получить Exchange Server, администраторы и Exchange Online клиенты.
  
## <a name="configuration-settings-that-clients-can-access"></a>Параметры конфигурации, к которые клиенты могут получить доступ

Клиентские приложения могут получить и установить ряд параметров конфигурации с Exchange сервера. Параметры конфигурации, необходимые всем приложениям EWS, предоставляются службой автооткрытия. Другие параметры конфигурации используются для определенных сценариев приложений. 
  
**Таблица 1. Функции веб-служб, которые предоставляют параметры конфигурации для клиентов EWS**

|**Функция**|**Описание**|
|:-----|:-----|
|Служба автообнаружения  <br/> |Служба [автообнаружия](autodiscover-for-exchange.md) предоставляет клиентские приложения сведения о конфигурации, чтобы клиент мог автоматически настраивать себя для связи с EWS.  <br/> |
|Сведения о настраиваемой конфигурации, хранимые в почтовом ящике  <br/> |Для хранения пользовательских сведений о конфигурации в почтовом ящике можно использовать один из нескольких вариантов: объекты конфигурации пользователей, настраиваемые элементы или расширенные свойства. [](persistent-application-settings-in-ews-in-exchange.md)  <br/> |
|Управление делегированием  <br/> | EWS предоставляет операции CRUD для управления доступом делегатов к почтовому ящику. Делегаты — это пользователи, которым было предоставлено разрешение на доступ к почтовому ящику другого пользователя.<br/><br/>  Вы можете [](https://msdn.microsoft.com/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management) использовать операции управления делегатами, чтобы включить управление делегированием с помощью EWS, или, если вы используете управляемый API EWS, вы можете использовать следующие методы:<br/><br/>- [ExchangeService.AddDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.GetDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.UpdateDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.RemoveDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|Конфигурация поиска по обнаружению электронных обнаружений  <br/> |Клиентские приложения eDiscovery [](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) могут получать сведения о конфигурации поиска, включаемые в поисковый запрос eDiscovery, список поисковых почтовых ящиков и идентификатор на месте, в котором хранится почтовый ящик.  <br/> |
|Разрешения для папок  <br/> |Разрешения папок ограничивают действия пользователя в общедоступных папках, а в случае делегирования доступа делегат может делать в папке другого пользователя. Вы можете использовать метод [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) или [операцию GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) для доступа к набору разрешений каждой папки, включая общедоступные папки, общие частные папки или папки, к которым пользователи могут делегировать доступ.  <br/> |
|Советы по почте, единой системы обмена сообщениями или правила защиты  <br/> |Операция [GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) предоставляет сведения [](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) о конфигурации служб только для чтения для советов по почте, правил единой системы обмена сообщениями и защиты.  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Параметры конфигурации, к которые администраторы могут получить доступ на Exchange сервере

Большинство сценариев клиентских приложений не требуют изменений параметров конфигурации сервера; однако некоторые сценарии это делают. Например, чтобы позволить приложению среднего уровня действовать в качестве пользователя, необходимо Exchange на сервере. Обратите внимание, что доступ к некоторым настройкам можно получить только на локальном Exchange серверах. Если вы нацелены на Exchange Online, вашему клиенту может потребоваться работать с настройками по умолчанию.
  
**Таблица 2. Exchange конфигурации сервера, влияющие на клиентов EWS**

|**Функция**|**Доступно из Exchange Online?**|**Дополнительные сведения см. в...**|
|:-----|:-----|:-----|
|Параметры виртуального каталога (включая проверку подлинности)  <br/> |Нет  <br/> |[Get-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa998810%28v=exchg.150%29.aspx) <br/> [Set-WebServicesVirtualDirectory](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|Автообнаружение  <br/> |Нет  <br/> |[Get-AutodiscoverVirtualDirectory](https://technet.microsoft.com/library/aa996819%28v=exchg.150%29.aspx) <br/> [Set-AutodiscoverVirtualDirectory](https://technet.microsoft.com/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|Соответствие требованиям  <br/> |Да  <br/> |[Архивация](https://technet.microsoft.com/library/dd979800%28v=exchg.150%29.aspx) <br/> [Обнаружение электронных данных](https://technet.microsoft.com/library/dd298021%28v=exchg.150%29.aspx) <br/> [Удержание хранения](https://technet.microsoft.com/library/dd335168%28v=exchg.150%29.aspx) <br/> [Защита от потери данных](https://technet.microsoft.com/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|Управление делегированием  <br/> |Да  <br/> |[Manage Permissions for Recipients](https://technet.microsoft.com/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Exchange Impersonation  <br/> |Да  <br/> |[Настройка Exchange обезличения](https://msdn.microsoft.com/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|Советы по почте, единой системы обмена сообщениями или правила защиты  <br/> |Да  <br/> |[Подсказки](https://technet.microsoft.com/library/jj649091%28v=exchg.150%29.aspx) <br/> [Комлеты единой системы обмена сообщениями](https://technet.microsoft.com/library/aa997665%28v=exchg.150%29.aspx) <br/> [Правила защиты Outlook](https://technet.microsoft.com/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|Регулирование  <br/> |Нет  <br/> |[Параметры регулирования](ews-throttling-in-exchange.md) <br/> |
|Фильтрация агента пользователя  <br/> |Да  <br/> |[Фильтрация агента пользователя](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>См. также

- [Получите сведения о конфигурации службы с помощью EWS в Exchange](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)   
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

