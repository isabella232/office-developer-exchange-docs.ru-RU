---
title: Начать работу с использованием веб-служб Exchange
manager: sethgros
ms.date: 2/27/2017
ms.audience: Developer
localization_priority: Normal
ms.assetid: e1b07a92-0595-4bf1-bd6b-c07e66a8c923
description: Найдите сведения, которые помогут вам начать работу с веб-служб Exchange и других веб-служб Exchange.
ms.openlocfilehash: 2f203c5634c29105feb39220c3ebdd9624bb49ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761243"
---
# <a name="start-using-web-services-in-exchange"></a>Начать работу с использованием веб-служб Exchange

Найдите сведения, которые помогут вам начать работу с веб-служб Exchange и других веб-служб Exchange.
  
[Веб-службы Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)предоставляют доступ к данным почтового ящика хранятся в Exchange Online, Exchange Online как часть Office 365 и локальной версии Exchange, начиная с Exchange Server 2007 и позволяют создавать пользовательские приложения, которые вы можете Используйте для управления эти сведения в соответствии с требованиями вашей организации. Несмотря на то, диапазон веб-служб Exchange и веб-приложений-служб, которые можно создать практически не ограничен, некоторые основные понятия, применяются для любого типа приложения. В этом разделе представлены сведения о основные понятия, должны быть знакомы с, чтобы начать работу с веб-служб Exchange и другие веб-службы в Exchange. 
  
## <a name="build-your-knowledge"></a>Построение вашей базы знаний
<a name="bk_Knowledge"> </a>

При использовании .NET Framework или другой платформы для разработки веб-приложения службы необходимо понять некоторые важные понятия, прежде чем начать проекта разработки. 
  
**В таблице 1. Веб-служб концепции**

|**Концепция**|**Сводка**|
|:-----|:-----|
|[Архитектура](ews-applications-and-the-exchange-architecture.md) <br/> |Сведения о работе в рамках архитектуры Exchange и протоколы, которые используются веб-служб Exchange.  <br/> |
|[Типы приложений веб-служб Exchange](ews-application-types.md) <br/> |Узнайте о наиболее распространенные типы приложений, которые можно создать с помощью веб-служб Exchange в Exchange.  <br/> |
|[Доступа к веб-служб Exchange](controlling-client-application-access-to-ews-in-exchange.md) <br/> |Администраторы Exchange можно ограничить доступ к веб-служб Exchange для всей организации, для отдельных пользователей, а также для отдельных приложений. Узнайте, какой уровень доступа к необходимой вам.  <br/> |
|[Установка](setting-up-your-ews-application.md) <br/> |Найдите сведения о задачах, необходимо выполнить для создания приложений, использующих управляемый API EWS или веб-служб Exchange для взаимодействия с сервером Exchange.  <br/> |
|[Проверка подлинности](authentication-and-ews-in-exchange.md) <br/> |Сведения о параметрах проверки подлинности для подключения к Exchange Online и локальную систему Exchange.  <br/> |
|[Службы автообнаружения](autodiscover-for-exchange.md) <br/> |Сведения о наборе служб, которые можно использовать для обнаружения URL-адрес конечной точки где учетной записи пользователя можно получить доступ к информации с помощью веб-служб Exchange.  <br/> |
|[Сервер почтовых ящиков](http://technet.microsoft.com/en-us/library/jj150491%28v=exchg.150%29.aspx) <br/> |Ознакомьтесь с хранилищем данных, доступной для клиентов веб-служб Exchange. Веб-служб Exchange имеет права на ограниченный набор информацию, содержащуюся в доменных службах Active Directory (AD DS).  <br/> |
|[Почтовые приложения для Outlook и веб-служб Exchange](mail-apps-for-outlook-and-ews-in-exchange.md) <br/> |Найдите сведения о почтовых приложений для Outlook и работы с веб-служб Exchange в Exchange.  <br/> |
|[API REST Office 365 для почту, календари и контакты](office-365-rest-apis-for-mail-calendars-and-contacts.md) <br/> |Сведения об Office 365 API-интерфейсы, которые можно использовать для доступа к почту, календари и контакты в Exchange Online в составе Office 365.  <br/> |
|[Управляемый API веб-служб Exchange](get-started-with-ews-managed-api-client-applications.md) <br/> |Найдите сведения о предпочитаемого клиентского интерфейса API для разработчиков .NET Framework.  <br/> |
|[Службы EWS](get-started-with-ews-client-applications.md) <br/> |Найдите сведения о создании первого приложения с помощью XML веб-служб Exchange запросы и ответы.  <br/> |
|[Функциональные возможности веб-служб Exchange в Exchange версии продуктов](ews-functionality-in-exchange-product-versions.md) <br/> |Узнайте, какие функциональные возможности веб-служб Exchange доступна в версии Exchange.  <br/> |
|[Отслеживание и устранение неполадок](how-to-trace-requests-responses-to-troubleshoot-ews-managed-api-applications.md) <br/> |Узнайте, как для трассировки запросов веб-служб Exchange и ответы для устранения ошибок в приложении управляемый API веб-служб Exchange.  <br/> |
   
## <a name="create-your-first-application"></a>Создание первого приложения
<a name="create"> </a>

Если вы хотите получить business создания первого .NET Framework или клиентское приложение веб-служб Exchange, отображаться [приступить к работе с клиентскими приложениями, управляемый API EWS](get-started-with-ews-managed-api-client-applications.md) или [приступить к работе с клиентскими приложениями, веб-служб Exchange](get-started-with-ews-client-applications.md).
  
## <a name="get-code-samples"></a>Образцы кода
<a name="samples"> </a>

Чтобы найти образцы кода и примеры, показывающие, как для работы с веб-служб Exchange и других веб-служб Exchange, воспользуйтесь следующими ресурсами:
  
- [Примеры кода Exchange](http://code.msdn.microsoft.com/exchange)
    
- [CodePlex (en)](http://www.codeplex.com/)
    
- [Документация по Exchange API](develop-web-service-clients-for-exchange.md)
    
- [Форум разработчиков Exchange](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment)
    
Другие примеры доступны в блоги, код для демонстрации сайты и форумы. Мы также рекомендуем, что вы загрузили [EWSEditor](http://ewseditor.codeplex.com/). Этот проект реализует большую часть функциональных возможностей веб-служб Exchange; Примеры все основные функциональные возможности веб-служб Exchange, здесь можно найти.
  
Если вы не разработчика .NET Framework, многие библиотеки клиента можно найти, для разработки веб-служб Exchange, используйте Java, Python, PHP и других языках. 
  
## <a name="ask-questions-and-solve-problems"></a>Задайте вопросы и решения проблем
<a name="questions"> </a>

Нужна помощь по началу приемы работы и в случае не удалось найти ответы? [Форум разработчиков Exchange](http://social.technet.microsoft.com/Forums/exchange/en-US/home?forum=exchangesvrdevelopment) для получения сведений ли кто-либо сталкивались и разрешить этой проблеме можно найти. Сообщество участники ответили сотни вопросы о разработке Exchange. Кроме того, можно найти узлы третьих сторон, форумы и блоги, охватывающие Exchange (en), может оказаться решения, которые вы ищете. 
  
Если требуется дополнительная помощь в службу [поддержки Майкрософт](https://support.microsoft.com/) . Группа поддержки разработчиков Exchange службы с помощью опытных специалистов, которые могут помочь ответы на вопросы о разработке Exchange. 
  
## <a name="see-also"></a>См. также

- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md) 
- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md) 
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md) 
- [Справочник по веб-службам для Exchange](../web-service-reference/web-services-reference-for-exchange.md)
    

