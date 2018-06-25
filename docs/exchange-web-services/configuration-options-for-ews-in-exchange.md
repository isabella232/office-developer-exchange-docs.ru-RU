---
title: Параметры конфигурации для веб-службах Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f6562639-9366-4a13-9fdb-2fa737833329
description: Сведения о параметрах конфигурации, которые можно получить доступ к вашей клиентского веб-служб Exchange и настраиваемые параметры Exchange, которые могут повлиять на ваш клиент веб-служб Exchange.
ms.openlocfilehash: d6c2866abf3dc16c77d84355afb9d86b0a9934c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760940"
---
# <a name="configuration-options-for-ews-in-exchange"></a>Параметры конфигурации для веб-службах Exchange

Сведения о параметрах конфигурации, которые можно получить доступ к вашей клиентского веб-служб Exchange и настраиваемые параметры Exchange, которые могут повлиять на ваш клиент веб-служб Exchange. 
  
Множество параметров конфигурации может повлиять на клиентское приложение веб-служб Exchange, которые можно выполнить. Эти параметры конфигурации являются: 
  
- Только для чтения или для чтения и записи из клиента.
    
- Доступ к на сервере Exchange, на котором размещается служба веб-служб Exchange.
    
Клиент для доступа к параметрам в Exchange Online, Exchange Online в составе Office 365 и Exchange server на месте. Все параметры сервера Exchange на месте, доступны для администраторов Exchange; Однако не все эти параметры доступны в Exchange Online Администраторы клиента. В этой статье описывается, какие клиенты параметры конфигурации, администраторы сервера Exchange и клиентом Exchange Online администраторы могут получить доступ к.
  
## <a name="configuration-settings-that-clients-can-access"></a>Параметры конфигурации, которые клиенты могут получить доступ к

Клиентское приложение можно получить и задать параметры конфигурации с сервера Exchange. Параметры конфигурации, которые необходимы для всех приложений веб-служб Exchange предоставляются службы автообнаружения. Другие параметры конфигурации используются для конкретного приложения сценариев. 
  
**В таблице 1. Функции веб-служб, которые обеспечивают параметры конфигурации для клиентов веб-служб Exchange**

|**Функция**|**Описание**|
|:-----|:-----|
|Службы автообнаружения  <br/> |[Службы автообнаружения](autodiscover-for-exchange.md) предоставляет вашей клиентских приложений с помощью сведений о конфигурации, чтобы клиент автоматически можно настроить так, чтобы взаимодействовать с веб-служб Exchange.  <br/> |
|Данные настраиваемой конфигурации, которые хранятся в почтовом ящике  <br/> |Можно использовать один из нескольких параметров для [хранения сведений о конфигурации](persistent-application-settings-in-ews-in-exchange.md) в почтовом ящике пользователя: Конфигурация объектов-пользователей, настраиваемые элементы или расширенные свойства.  <br/> |
|Делегирование управления  <br/> | Веб-служб Exchange предоставляет операций CRUD для управления делегированный доступ к почтовому ящику. Делегаты — это пользователи, у которых есть разрешение на доступ к почтовому ящику другого пользователя.<br/><br/>  [Операции управления делегат](http://msdn.microsoft.com/en-us/library/bb409286%28v=exchg.150%29.aspx#bk_delegate_management) можно использовать для включения делегирование управления с помощью веб-служб Exchange или, если вы используете управляемый API веб-служб Exchange, можно использовать следующие методы:<br/><br/>- [ExchangeService.AddDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.GetDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getdelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.UpdateDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.updatedelegates%28v=exchg.80%29.aspx) <br/>- [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |
|Конфигурация поиска обнаружения электронных данных  <br/> |[Поиск сведений о конфигурации](http://msdn.microsoft.com/library/8a54a6dc-110c-4972-a8bc-5ddb43c4b857%28Office.15%29.aspx) , которая включает в себя запрос поиска обнаружения электронных данных список доступен для поиска почтовых ящиков можно получить eDiscovery клиентских приложений и хранит идентификатор почтового ящика на месте.  <br/> |
|Разрешения для папки  <br/> |Ограничение разрешений для папки пользователь может выполнить в общей папке и в случае делегированный доступ, что делегат может сделать в папки другого пользователя. Для доступа к набору разрешений каждой папки, включая общие папки, личных папок или папки, к которым пользователи имеют делегированный доступ, можно использовать метод [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) или [GetFolder операции](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) .  <br/> |
|Почтовые подсказки, единой системы обмена сообщениями или правила защиты  <br/> |[Операция GetServiceConfiguration](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx) содержит только для чтения [сведений о конфигурации службы](how-to-get-service-configuration-information-by-using-ews-in-exchange.md) для почтовые подсказки, единой системы обмена сообщениями и правила защиты.  <br/> |
   
## <a name="configuration-settings-that-administrators-can-access-on-the-exchange-server"></a>Параметры конфигурации, которые администраторы могут получить доступ к на сервере Exchange

Большинству сценариев клиентского приложения не требуется изменений в параметры конфигурации сервера; Тем не менее выполните некоторые сценарии. Например чтобы приложения среднего уровня в качестве пользователя, необходимо установить уровень олицетворения Exchange на сервере. Обратите внимание на то, что некоторые параметры доступен только на серверах Exchange на месте. Если вы используете Exchange Online, клиентское приложение может потребоваться работа с параметрами по умолчанию.
  
**В таблице 2. Параметры конфигурации сервера Exchange, которые влияют на клиентов веб-служб Exchange**

|**Функция**|**Доступ из Exchange Online?**|**Для получения дополнительных сведений см.**|
|:-----|:-----|:-----|
|Параметры виртуального каталога (в том числе проверка подлинности)  <br/> |Нет  <br/> |[Get-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa998810%28v=exchg.150%29.aspx) <br/> [SET-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) <br/> |
|Автообнаружение  <br/> |Нет  <br/> |[Get-AutodiscoverVirtualDirectory](http://technet.microsoft.com/en-us/library/aa996819%28v=exchg.150%29.aspx) <br/> [SET-AutodiscoverVirtualDirectory](http://technet.microsoft.com/en-us/library/aa998601%28v=exchg.150%29.aspx) <br/> |
|Соответствие требованиям  <br/> |Да  <br/> |[Архивации](http://technet.microsoft.com/en-us/library/dd979800%28v=exchg.150%29.aspx) <br/> [обнаружение электронных данных](http://technet.microsoft.com/en-us/library/dd298021%28v=exchg.150%29.aspx) <br/> [Удержание хранения](http://technet.microsoft.com/en-us/library/dd335168%28v=exchg.150%29.aspx) <br/> [Защита от потери данных](http://technet.microsoft.com/en-us/library/jj150527%28v=exchg.150%29.aspx) <br/> |
|Делегирование управления  <br/> |Да  <br/> |[Управление разрешениями для получателей](http://technet.microsoft.com/en-us/library/jj919240%28v=exchg.150%29.aspx) <br/> |
|Олицетворение Exchange  <br/> |Да  <br/> |[Настройка олицетворения Exchange](http://msdn.microsoft.com/en-us/library/bb204095%28EXCHG.140%29.aspx) <br/> |
|Почтовые подсказки, единой системы обмена сообщениями или правила защиты  <br/> |Да  <br/> |[Почтовые подсказки](http://technet.microsoft.com/en-us/library/jj649091%28v=exchg.150%29.aspx) <br/> [Единая система обмена сообщениями командлеты](http://technet.microsoft.com/en-us/library/aa997665%28v=exchg.150%29.aspx) <br/> [Правила защиты Outlook](http://technet.microsoft.com/en-us/library/dd638178%28v=exchg.150%29.aspx) <br/> |
|Регулирование  <br/> |Нет  <br/> |[Параметры регулирования](ews-throttling-in-exchange.md) <br/> |
|Фильтрация агента пользователя  <br/> |Да  <br/> |[Фильтрация агента пользователя](how-to-control-access-to-ews-in-exchange.md) <br/> |
   
## <a name="see-also"></a>См. также

- [Получение сведений о конфигурации службы с помощью веб-служб Exchange в Exchange](how-to-get-service-configuration-information-by-using-ews-in-exchange.md)
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)   
- [Начать работу с использованием веб-служб Exchange](start-using-web-services-in-exchange.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

