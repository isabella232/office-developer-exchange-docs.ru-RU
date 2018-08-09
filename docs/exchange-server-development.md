---
title: Разработки для Exchange Online и Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: f33d1093-75ba-4ff2-8d15-b0bf73a401bf
description: Представляем подробную документацию для разработчиков Exchange Server (в том числе по Exchange Online как части Office 365), Exchange Online, Exchange 2013, Управляемый API EWS, Exchange 2010 и Exchange 2007.
ms.openlocfilehash: 2af9e52c3f7cf03d7571d1640ef7bfa45b5e97be
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353247"
---
# <a name="exchange-online-and-exchange-development"></a>Разработки для Exchange Online и Exchange

Представляем подробную документацию для разработчиков Exchange Server (в том числе по Exchange Online как части Office 365), Exchange Online, Exchange 2013, Управляемый API EWS, Exchange 2010 и Exchange 2007.

Вы можете использовать справочную документацию как практическое руководство, документацию для начала работ, материалы с описанием новых характеристик и API для разработки средств доступа и управления данными почтовых ящиков со служб, веб-сайтов, настольных компьютеров и мобильных устройств, а также создавать пользовательские решения для электронной почты, календаря, контактов и других элементов, которые хранятся в Exchange Online или на сервере Exchange 2013.

Вы можете использовать Веб-службы Exchange (EWS), Автообнаружение, Надстройки Outlook или другие API для разработки приложений. С помощью это страницы вы сможете выбрать подходящую технологию Exchange.

## <a name="exchange-developer-content"></a>Материалы для разработчиков Exchange

Используйте приведенную ниже таблицу для определения технологии и связанных материалов API, которые помогут вам в достижении поставленных целей разработки.

> [!IMPORTANT]
> Microsoft Graph является API, рекомендуемым для доступа к данным Exchange Online. Новые приложения, разработанные для доступа к данным в Exchange Online, должны использовать Microsoft Graph.

|Что нужно создать...|С чего начать|
|:-----|:-----|
|REST-приложение для доступа к Exchange Online в составе Office 365|[Приложения Microsoft Graph REST API для почты, календаря и контактов](exchange-web-services/office-365-rest-apis-for-mail-calendars-and-contacts.md) |
|Контекстно-зависимое приложение для отображения информации в Outlook, Outlook Web App или OWA для устройств |[Надстройки для Outlook и EWS в Exchange](exchange-web-services/mail-apps-for-outlook-and-ews-in-exchange.md) |
|Клиент почтовых ящиков, не созданный на платформе .NET Framework или Java |[Сведения об управляемом API EWS, EWS и веб-службах в Exchange](exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) |
|Клиент почтовых ящиков, использующий .NET Framework для доступа к веб-службам Exchange |[Начало работы с клиентскими приложениями, использующими управляемый API EWS](exchange-web-services/get-started-with-ews-managed-api-client-applications.md) |
|Клиент почтовых ящиков, использующий Java для доступа к EWS |[API Java EWS на GitHub](https://github.com/OfficeDev/ews-java-api) |
|Приложение, которое настраивает пользовательский интерфейс Outlook или использует бизнес-логику Outlook  |[Справочник по VBA для Outlook](https://msdn.microsoft.com/ru-RU/VBA/VBA-Outlook) |
|Приложение, которое предназначено для Exchange Online или Exchange 2013, на которое необходимо перейти с более ранней версии Exchange  |[Переход на технологии Exchange](migrating-to-exchange-online-and-exchange-2013-technologies.md) |
|Пользовательское средство управления, использующее Windows PowerShell из управляемого кода   |[Командная консоль Exchange](management/exchange-management-shell.md) |
|Решение для резервного копирования или восстановления данных Exchange  |[Резервное копирование и восстановление для Exchange](backup-restore/backup-and-restore-for-exchange-2013.md) |
|Расширение для поддержки доступа к сообщениям в конвейере транспорта   |[Агенты транспорта в Exchange](transport-agents/transport-agents-in-exchange-2013.md)  |
|Клиент почтовых ящиков для мобильного устройства   |[Exchange ActiveSync](https://technet.microsoft.com/ru-RU/library/aa998357.aspx) |

## <a name="exchange-interactions-with-custom-applications"></a>Exchange взаимодействует с пользовательскими приложениями

Некоторые из этих технологий позволяют приложениям работать с данными, хранящимися в Exchange, а другие используются для управления сервером Exchange. Часто выполнить задачу можно благодаря сразу нескольким технологиям или языкам программирования. Поэтому вы можете выбрать те, с которыми знакомы. Например, задать свойства элементов в хранилище Exchange можно с помощью API REST почтовой программы, веб-служб Exchange или Управляемый API EWS.

Существует несколько способов взаимодействия Exchange с пользовательскими приложениями в зависимости от их архитектуры и функций. По сути, Exchange обеспечивает не только транспорт сообщений, но и обслуживание почтовых ящиков, и запуск приложений на основе форм, а также многое другое.

|Взаимодействие Exchange|Описание|
|:-----|:-----|
|**Передача сообщений**|Exchange подходит для использования в качестве стандартного почтового сервера для приложений, которые отправляют сообщения.<br/>Exchange включает несколько интерфейсов API для передачи сообщений, в том числе REST, EWS и Управляемый API EWS.<br/>Кроме того, приложения могут использовать агенты транспорта для ответа по мере обработки сообщений и доставки посредством Exchange. |
|**Хранилище почтового ящика** |Exchange обеспечивает иерархическую структуру папок, элементов и свойств для приложений, чей доступ к данным хранится в почтовых ящиках.<br/>Вы можете получить этот доступ, совмещая работу с базой данных и COM-объектами.<br/>Когда вы запрашиваете данные, служба Exchange управляет доступом к хранящимся данным с учетом разрешений для пользователя и хранилища.<br/>Приложения, которые обрабатывают данные почтовых ящиков, обычно используют REST, EWS или управляемое API EWS.|
|**Управляемый корпоративный сервер** |Exchange работает как управляемый сервер для приложений, которые управляют серверами и хранилищами Exchange.<br/>Приложения могут настраивать, контролировать и отслеживать текущую деятельность и работоспособность серверов Exchange в организации.<br/>Приложения управления Exchange используют командную консоль Exchange для управления серверами Exchange. |

## <a name="see-also"></a>См. также

- 
  [Справочные материалы по серверному API для Exchange](https://msdn.microsoft.com/en-us/library/dn186243(v=exchg.150).aspx)
- [Узнайте об Exchange в блогах Office](https://www.microsoft.com/ru-RU/microsoft-365/blog/)
- [Скачайте 101 пример кодов для Exchange 2013](https://code.msdn.microsoft.com/office/Exchange-2013-101-Code-3c38582c)
- [Получите управляемый API EWS (GitHub)](https://github.com/OfficeDev/ews-managed-api/blob/master/README.md)
- [Получите поддержку для сервера Exchange](https://support.microsoft.com/en-us/getsupport?oaspworkflow=start_1.0.0.0&wf=0&wfname=productselection&gprid=730&x=13&y=7&st=1&wfxredirect=1&sd=gn&ccsid=635890984021344661&forceorigin=esmc)
