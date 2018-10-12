---
title: Справочник по управляемому API веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6ca36f4-a67c-4e3c-aae7-9ead7b704e15
description: Узнайте о пространствах имен, включенных в управляемый API веб-служб Exchange.
ms.openlocfilehash: 78797ba5124cb47da5430491d3be23bbaf0371a7
ms.sourcegitcommit: 25cbbc6707e4ec0621c5c46baf7fe49be42d3297
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/07/2018
ms.locfileid: "25440985"
---
# <a name="ews-managed-api-reference"></a>Справочник по управляемому API веб-служб Exchange

**Область применения**: управляемый API веб-служб Exchange | Exchange Online | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 | Office 365

В состав управляемого API веб-служб Exchange входят два API: Microsoft.Exchange.WebServices.dll и Microsoft.Exchange.WebServices.Auth.dll.

## <a name="ews-managed-api-namespaces"></a>Пространства имен управляемого API веб-служб Exchange

|Пространство имен |Описание |
|:---------|:-----------|
|[Microsoft.Exchange.WebServices.Auth.Validation](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.auth.validation?view=exchange-ews-api) |Содержит типы и методы, которые используются для проверки маркеров удостоверений пользователей, отправленных с сервера Exchange. Пространство имен Microsoft.Exchange.WebServices.Auth.Validation применимо к клиентам, предназначенным для работы с Exchange Online и Exchange, начиная с версии Exchange Server 2013. Это пространство имен включено в API Microsoft.Exchange.WebServices.Auth.dll.|
|[Microsoft.Exchange.WebServices.Autodiscover](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.autodiscover?view=exchange-ews-api)|Содержит типы, которые используются для обмена данными со службой автообнаружения, размещенной Exchange Server. Это пространство имен также используется для поиска объектов точек подключения службы в доменных службах Active Directory (AD DS). Служба автообнаружения предоставляет сведения о конфигурации клиентам веб-служб Exchange. Благодаря этому клиенты могут обращаться по URL-адресу соответствующей службы.<br/><br/>Функции пространства имен можно использовать для обращения к службе автообнаружения POX, впервые появившейся в Microsoft Exchange Server 2007, к функции поиска объекта точки подключения службы, если клиент присоединен к домену, или к конечной точке автообнаружения SOAP, впервые появившейся в Exchange Server 2010. Основной тип в этом пространстве имен — [класс AutodiscoverService](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.autodiscover.autodiscoverservice?view=exchange-ews-api). Это пространство имен включено в API Microsoft.Exchange.WebServices.dll.|
|[Microsoft.Exchange.WebServices.Data](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data?view=exchange-ews-api)| Содержит типы, которые используются для обмена данными с сервером Exchange через веб-службы Exchange. Это пространство имен предоставляет основные функции управляемого API веб-служб Exchange. Основной тип в этом пространстве имен — [класс ExchangeService](https://docs.microsoft.com/dotnet/api/microsoft.exchange.webservices.data.exchangeservice?view=exchange-ews-api).|

## <a name="see-also"></a>См. также

- [Справочник по веб-службам для Exchange](web-services-reference-for-exchange.md)
- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Новые возможности веб-служб Exchange и других веб-служб в Exchange](../exchange-web-services/whats-new-in-ews-and-other-web-services-in-exchange.md)
- [Начало работы с использованием веб-служб в Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Разработка клиентов веб-служб для Exchange](../exchange-web-services/develop-web-service-clients-for-exchange.md)

