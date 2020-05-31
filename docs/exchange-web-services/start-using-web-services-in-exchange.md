---
title: Начать работу с использованием веб-служб Exchange
manager: sethgros
ms.date: 2/27/2017
ms.audience: Developer
localization_priority: Normal
ms.assetid: e1b07a92-0595-4bf1-bd6b-c07e66a8c923
description: Здесь вы найдете информацию, которая поможет вам начать работу с веб-службами EWS и другими веб-службами в Exchange.
ms.openlocfilehash: 2f203c5634c29105feb39220c3ebdd9624bb49ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761243"
---
# <a name="start-using-web-services-in-exchange"></a>Начать работу с использованием веб-служб Exchange

Здесь вы найдете информацию, которая поможет вам начать работу с веб-службами EWS и другими веб-службами в Exchange.
  
[Веб-службы в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)предоставляют доступ к данным почтовых ящиков, хранящимся в Exchange Online, Exchange Online в составе Office 365, и локальным версиям Exchange, начиная с Exchange Server 2007, и позволяя создавать настраиваемые приложения, которые можно использовать для управления этими сведениями в соответствии с требованиями Организации. Несмотря на то, что диапазон создаваемых приложений EWS и веб-служб практически бесконечно, некоторые фундаментальные концепции применяются для любого типа приложений. В этом разделе представлены сведения об основных понятиях, с которыми необходимо ознакомиться, чтобы начать использовать веб-службы EWS и другие веб-службы в Exchange. 
  
## <a name="build-your-knowledge"></a>Создание базы знаний
<a name="bk_Knowledge"> </a>

Если вы используете .NET Framework или другую платформу для разработки приложения веб-службы, вам будет необходимо изучить некоторые важные понятия, прежде чем приступать к проекту разработки. 
  
**Таблица 1. Концепции веб-служб**

|**Концепция**|**Сводка**|
|:-----|:-----|
|[Архитектура](ews-applications-and-the-exchange-architecture.md) <br/> |Узнайте, как работает служба EWS в архитектуре Exchange и используемых ею протоколах.  <br/> |
|[Типы приложений EWS](ews-application-types.md) <br/> |Сведения о наиболее распространенных типах приложений, которые можно создать с помощью EWS в Exchange.  <br/> |
|[Доступ к EWS](controlling-client-application-access-to-ews-in-exchange.md) <br/> |Администраторы Exchange могут полностью ограничить доступ к службам EWS для всей Организации, отдельных пользователей и отдельных приложений. Узнайте, какой уровень доступа подходит вам.  <br/> |
|[Установка](setting-up-your-ews-application.md) <br/> |Найдите сведения о задачах, которые необходимо выполнить для создания приложений, использующих управляемый API EWS или EWS для связи с Exchange.  <br/> |
|[Проверка подлинности](authentication-and-ews-in-exchange.md) <br/> |Сведения о параметрах проверки подлинности для подключения к Exchange Online и локальной среде Exchange.  <br/> |
|[Автообнаружение](autodiscover-for-exchange.md) <br/> |Узнайте о наборе служб, которые можно использовать для обнаружения конечной точки URL-адреса, в которой учетная запись пользователя может получать доступ к информации с помощью EWS.  <br/> |
|[Сервер почтовых ящиков](http://technet.microsoft.com/en-us/library/jj150491%28v=exchg.150%29.aspx) <br/> |Узнайте о основном репозитории сведений, доступных клиенту EWS. Служба EWS имеет доступ к ограниченному набору сведений, хранящихся в доменных службах Active Directory (AD DS).  <br/> |
|[Почтовые приложения для Outlook и EWS](mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Найдите сведения о почтовых приложениях для Outlook и их работе с EWS в Exchange.  <br/> |
|[API REST Office 365 для почту, календари и контакты](office-365-rest-apis-for-mail-calendars-and-contacts.md) <br/> |Сведения об интерфейсах API Office 365, которые можно использовать для доступа к электронной почте, календарям и контактам в Exchange Online в составе Office 365.  <br/> |
|[управляемый API EWS;](get-started-with-ews-managed-api-client-applications.md) <br/> |Здесь вы найдете сведения о предпочтительном клиенте API для разработчиков .NET Framework.  <br/> |
|[EWS](get-started-with-ews-client-applications.md) <br/> |Сведения о создании первого приложения с помощью запросов и ответов по веб-службам EWS.  <br/> |
|[Функции EWS в версиях продуктов Exchange](ews-functionality-in-exchange-product-versions.md) <br/> |Узнайте, какие функции EWS доступны в версии Exchange.  <br/> |
|[Трассировка и устранение неполадок](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) <br/> |Сведения о том, как отслеживать запросы и ответы EWS для устранения ошибок в приложении управляемого API EWS.  <br/> |
   
## <a name="create-your-first-application"></a>Создание первого приложения
<a name="create"> </a>

Если вы готовы приступить к написанию вашего первого клиентского приложения .NET Framework или EWS, ознакомьтесь со [статьей начало работы с клиентскими приложениями с управляемым API EWS](get-started-with-ews-managed-api-client-applications.md) или [Начало работы с клиентскими приложениями EWS](get-started-with-ews-client-applications.md).
  
## <a name="get-code-samples"></a>Получение примеров кода
<a name="samples"> </a>

Чтобы найти примеры кода и примеры, показывающие, как работать с веб-службами EWS и другими веб-службами в Exchange, ознакомьтесь со следующими материалами:
  
- [Примеры кода Exchange](http://code.msdn.microsoft.com/exchange)
    
- [CodePlex](http://www.codeplex.com/)
    
- [Документация по API Exchange](develop-web-service-clients-for-exchange.md)
    
- [Форум по разработке Exchange](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment)
    
Многие другие примеры доступны в блогах, демонстрационных сайтах и форумах. Кроме того, рекомендуется скачать [евседитор](http://ewseditor.codeplex.com/). Этот проект реализует большинство функций EWS; Здесь вы можете найти примеры всех основных функций EWS.
  
Если вы не являетесь разработчиком .NET Framework, вы можете найти многие клиентские библиотеки для разработки EWS, которые используют Java, Python, PHP и другие языки. 
  
## <a name="ask-questions-and-solve-problems"></a>Задавайте вопросы и разрешите проблемы
<a name="questions"> </a>

Нужна помощь по выполнению задач и невозможности найти ответы? Вы можете выполнить поиск в [форуме по разработке Exchange](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) , чтобы узнать, встречается ли кто-то другой, и устранить эту проблему. Сообщество участников ответило сотни вопросов о разработке Exchange. Вы также можете найти сторонние сайты, форумы и блоги, посвященные разработке Exchange, а также найти решение, которое вы ищете. 
  
Если вам нужна дополнительная помощь, обратитесь в [службу поддержки Майкрософт](https://support.microsoft.com/) . Сотрудники группы поддержки разработчиков Exchange отвечают за ваши специалисты, которые могут помочь вам ответить на вопросы о разработке Exchange. 
  
## <a name="see-also"></a>См. также

- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md) 
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md) 
- [Справочник по веб-службам для Exchange](../web-service-reference/web-services-reference-for-exchange.md)
    

