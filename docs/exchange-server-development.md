---
title: Exchange Online и Exchange (en)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f33d1093-75ba-4ff2-8d15-b0bf73a401bf
description: Представляем подробную документацию для разработчиков Exchange Server (в том числе по Exchange Online как части Office 365), Exchange Online, Exchange 2013, Управляемый API EWS, Exchange 2010 и Exchange 2007.
ms.openlocfilehash: b933bd1bdc6dfcbe4941f23dbee9a587745c7bd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760935"
---
# <a name="exchange-online-and-exchange-development"></a>Exchange Online и Exchange (en)

Представляем подробную документацию для разработчиков Exchange Server (в том числе по Exchange Online как части Office 365), Exchange Online, Exchange 2013, Управляемый API EWS, Exchange 2010 и Exchange 2007. 

Можно использовать как, начало работы, новые функции и справочная документация по API для разработки средств для доступа к данным и управления ими почтовых ящиков из служб, веб-сайтов, настольных компьютеров и мобильных устройств и создания настраиваемых решений для электронной почты, календарь, контакты, и другие элементы, которые хранятся в Exchange Online или на сервере Exchange 2013. 

Вы можете использовать Веб-службы Exchange (EWS), автообнаружение, почтовые приложения для Office и другие API для разработки приложений. На этой странице поможет вам Выбор правильной технологии Exchange.

## <a name="exchange-developer-content"></a>Содержимое для разработчиков Exchange  

С помощью таблицы ниже определите технологию и соответствующее содержимое API, чтобы использовать их при разработке.  
  
|Что нужно создать|С чего следует начать|
|:-----|:-----|
|Приложение на основе REST для доступа к Exchange Online в составе Office 365|[API REST Office 365 для почту, календари и контакты](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md) |
|Контекстно-зависимое приложение для отображения информации в Outlook, Outlook Web App или OWA для устройств |[Приложения электронной почты для Outlook и EWS в Exchange](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) |
|Почтовый клиент, не размещенный на .NET Framework или Java |[Сведения об управляемом API EWS, EWS и веб-службах в Exchange](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) |
|Почтовый клиент, для доступа к веб-служб Exchange с помощью .NET Framework |[Начало работы с клиентскими приложениями, использующими управляемый API EWS](exchange-web-services/get-started-with-ews-managed-api-client-applications.md) |
|Почтовый клиент, который использует Java для доступа к веб-служб Exchange |[Java API для веб-служб Exchange на сайте GitHub](https://github.com/OfficeDev/ews-java-api) |
|Приложение, которое настраивает пользовательского интерфейса Outlook или опирается на бизнес-логику Outlook  |[Справочные материалы по VBA для Outlook](https://msdn.microsoft.com/en-us/VBA/VBA-Outlook) |
|Приложение, предназначенное для Exchange Online или Exchange 2013, который необходимо перенести из предыдущей версии сервера Exchange  |[Переход на технологии Exchange](migrating-to-exchange-online-and-exchange-2013-technologies.md) |
|Настраиваемое средство для управления, использующее Windows PowerShell из управляемого кода   |[Командная консоль Exchange](management/exchange-management-shell.md) |
|Решения для резервного копирования или восстановления данных Exchange  |[Резервное копирование и восстановление для Exchange](backup-restore/backup-and-restore-for-exchange-2013.md) |
|Расширение для поддержки доступа к сообщениям в конвейере транспорта   |[Агенты транспорта в Exchange](transport-agents/transport-agents-in-exchange-2013.md)  |
|Клиент для почтовых ящиков для мобильного устройства   |[Служба Exchange ActiveSync](https://technet.microsoft.com/en-us/library/aa998357.aspx) |
   
## <a name="exchange-interactions-with-custom-applications"></a>Взаимодействие Exchange с помощью пользовательских приложений

Некоторые из этих технологий позволяют приложениям работать с данными, хранящимися в Exchange, а другие используются для управления сервером Exchange. Часто выполнить задачу можно благодаря сразу нескольким технологиям или языкам программирования. Поэтому вы можете выбрать те, с которыми знакомы. Например, задать свойства элементов в хранилище Exchange можно с помощью API REST почтовой программы, веб-служб Exchange или Управляемый API EWS.
  
Существует несколько способов взаимодействия Exchange с пользовательскими приложениями в зависимости от их архитектуры и функций. По сути, Exchange обеспечивает не только транспорт сообщений, но и обслуживание почтовых ящиков, и запуск приложений на основе форм, а также многое другое.

|Способ взаимодействия Exchange|Описание|
|:-----|:-----|
|**Сообщения транспорта**|Exchange выполняет функции стандартного почтового сервера для приложений, отправляющих сообщения.<br/>Exchange включает несколько интерфейсов API для передачи сообщений, в том числе REST, EWS и Управляемый API EWS.<br/>Кроме того, приложения могут использовать агенты транспорта для отправки ответов по мере того, как Exchange обрабатывает и доставляет сообщения. |
|**Хранилища почтовых ящиков** |Exchange предоставляет иерархическую структуру папок, элементов и свойств для приложений, которые получают доступ к данным, хранящимся в почтовых ящиках.<br/>Вы можете получить этот доступ, совмещая работу с базой данных и COM-объектами.<br/>Когда вы запрашиваете данные, служба Exchange управляет доступом к хранящимся данным с учетом разрешений для пользователя и хранилища.<br/>Приложения, которые обрабатывают данные почтового ящика, обычно используют REST, EWS или Управляемый API EWS.|
|**Управляемые enterprise server** |Exchange выполняет функции управляемого сервера для приложений, которые управляют серверами и хранилищами Exchange.<br/>Приложения могут настраивать, контролировать и отслеживать текущую деятельность и работоспособность серверов Exchange в организации.<br/>Приложения управления Exchange используют Командная консоль Exchange для управления серверами Exchange. |
   
## <a name="see-also"></a>См. также

- [Справочник по API сервера для Exchange](https://msdn.microsoft.com/en-us/library/dn186243(v=exchg.150).aspx)
- [Материалы по Exchange в блогах Office](https://www.microsoft.com/en-us/microsoft-365/blog/) 
- [101 пример кода для Exchange 2013](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)
- [Получить управляемый API веб-служб Exchange (репозиториев)](https://github.com/OfficeDev/ews-managed-api/blob/master/README.md)
- [Поддержка для Exchange Server](https://support.microsoft.com/en-us/getsupport?oaspworkflow=start_1.0.0.0&wf=0&wfname=productselection&gprid=730&x=13&y=7&st=1&wfxredirect=1&sd=gn&ccsid=635890984021344661&forceorigin=esmc)


