---
title: Настройка параметров для EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: Сведения о параметрах конфигурации, доступ к которым имеет клиент EWS, а также настраиваемые параметры Exchange, которые могут повлиять на клиента EWS.
ms.openlocfilehash: 55f927b7b301bdfaa298bcd254b18a00cf1692d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456159"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Настройка параметров для EWS в Exchange

Сведения о параметрах конфигурации, доступ к которым имеет клиент EWS, а также настраиваемые параметры Exchange, которые могут повлиять на клиента EWS. 
  
Многие параметры конфигурации могут влиять на то, что может выполнять клиентское приложение EWS. Эти параметры конфигурации могут быть следующими: 
  
- Только для чтения или для чтения и записи из клиента.
    
- Доступ к серверу Exchange Server, на котором размещается служба EWS.
    
Клиент может получить доступ к параметрам в Exchange Online, Exchange Online в составе Office 365 и локальном сервере Exchange Server. Все локальные параметры Exchange Server доступны администраторам Exchange; Однако не все эти параметры доступны администраторам клиентов Exchange Online. В этой статье описывается, какие параметры конфигурации клиенты, администраторы Exchange Server и Администраторы клиентов Exchange Online могут получать доступ.
  
## <a name="configuration-settings-that-clients-can-access"></a>Параметры конфигурации, доступные клиентам

Клиентское приложение может получать и задавать ряд параметров конфигурации на сервере Exchange. Параметры конфигурации, необходимые для всех приложений EWS, предоставляются службой автообнаружения. Другие параметры конфигурации используются для конкретных сценариев приложений. 
  
**Таблица 1. Функции веб-служб, предоставляющие параметры конфигурации для клиентов EWS**

|**Функция**|**Описание**|
|:-----|:-----|
|Служба автообнаружения  <br/> |[Служба автообнаружения](autodiscover-for-exchange.md) предоставляет клиентским приложениям сведения о конфигурации, чтобы клиент мог автоматически настраивать себя для общения с EWS.  <br/> |
|Настраиваемые сведения о конфигурации, хранящиеся в почтовом ящике  <br/> |Вы можете использовать один из нескольких вариантов [хранения настраиваемых сведений о конфигурации](persistent-application-settings-in-ews-in-exchange.md) в почтовом ящике: объекты конфигурации пользователя, настраиваемые элементы или расширенные свойства.  <br/> |
|Управление делегированием  <br/> | EWS предоставляет операции CRUD для управления делегированным доступом к почтовому ящику. Представители — это пользователи, которым предоставлено разрешение на доступ к почтовому ящику другого пользователя.<br/><br/>  Вы можете использовать [операции управления делегированием](https://msdn.microsoft.com/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management) , чтобы включить управление делегированием с помощью EWS, или, если вы используете управляемый API EWS, вы можете использовать следующие методы:<br/><br/>- [ExchangeService. Аддделегатес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. Делегаты](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. Упдатеделегатес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService. Ремоведелегатес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|Конфигурация поиска eDiscovery  <br/> |клиентские приложения обнаружения электронных [данных могут получать сведения о конфигурации поиска](https://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) , включающие поисковый запрос обнаружения электронных данных, список почтовых ящиков, доступных для поиска, и идентификатор почтовых ящиков на месте.  <br/> |
|Разрешения для папок  <br/> |Разрешения на доступ к папкам ограничивают то, что делает пользователь в общедоступной папке, а также о том, как представитель может выполнять действия делегата в папке другого пользователя. Для доступа к набору разрешений каждой папки, включая общедоступные папки, общие частные папки или папки, к которым пользователи имеют доступ для делегирования, можно использовать как метод [Folder. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) , так и [операцию с папкой](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) .  <br/> |
|Советы по работе с почтой, единая система обмена сообщениями или правила защиты  <br/> |[Операция GetServiceConfiguration](https://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) предоставляет [сведения о конфигурации службы](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) , предназначенной только для чтения, для почтовых подсказок, единой системы обмена сообщениями и правил защиты.  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Параметры конфигурации, доступные администраторам на сервере Exchange Server

Большинство сценариев клиентского приложения не требуют изменений параметров конфигурации сервера; Тем не менее, некоторые сценарии выполняются. Например, чтобы включить приложение среднего уровня в качестве пользователя, необходимо задать олицетворение Exchange на сервере. Обратите внимание на то, что доступ к некоторым параметрам возможен только на локальных серверах Exchange. Если вы нацелены на Exchange Online, клиентскому приложению может потребоваться работать с параметрами по умолчанию.
  
**Таблица 2. Параметры конфигурации Exchange Server, которые влияют на клиентов EWS**

|**Функция**|**Доступны в Exchange Online?**|**Для получения дополнительных сведений см.**|
|:-----|:-----|:-----|
|Параметры виртуального каталога (включая проверку подлинности)  <br/> |Нет  <br/> |[Get — Webservicesvirtualdirectory используется](https://technet.microsoft.com/library/aa998810%28v=exchg.150%29.aspx) <br/> [Set — Webservicesvirtualdirectory используется](https://technet.microsoft.com/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|Autodiscover  <br/> |Нет  <br/> |[Get — AutodiscoverVirtualDirectory используется](https://technet.microsoft.com/library/aa996819%28v=exchg.150%29.aspx) <br/> [Set — AutodiscoverVirtualDirectory используется](https://technet.microsoft.com/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|Соответствие требованиям  <br/> |Да  <br/> |[Архивация](https://technet.microsoft.com/library/dd979800%28v=exchg.150%29.aspx) <br/> [Обнаружение электронных данных](https://technet.microsoft.com/library/dd298021%28v=exchg.150%29.aspx) <br/> [Удержание хранения](https://technet.microsoft.com/library/dd335168%28v=exchg.150%29.aspx) <br/> [Защита от потери данных](https://technet.microsoft.com/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|Управление делегированием  <br/> |Да  <br/> |[Manage Permissions for Recipients](https://technet.microsoft.com/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Олицетворение Exchange  <br/> |Да  <br/> |[Настройка олицетворения Exchange](https://msdn.microsoft.com/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|Советы по работе с почтой, единая система обмена сообщениями или правила защиты  <br/> |Да  <br/> |[Подсказки](https://technet.microsoft.com/library/jj649091%28v=exchg.150%29.aspx) <br/> [Командлеты единой системы обмена сообщениями](https://technet.microsoft.com/library/aa997665%28v=exchg.150%29.aspx) <br/> [Правила защиты Outlook](https://technet.microsoft.com/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|Регулирование  <br/> |Нет  <br/> |[Параметры регулирования](ews-throttling-in-exchange.md) <br/> |
|Фильтрация агентов пользователей  <br/> |Да  <br/> |[Фильтрация агентов пользователей](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>См. также

- [Получение сведений о конфигурации службы с помощью EWS в Exchange](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)   
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

