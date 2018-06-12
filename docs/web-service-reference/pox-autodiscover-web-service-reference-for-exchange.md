---
title: Служба POX автоматического обнаружения веб-ссылки для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Найдите справочные сведения для службы автообнаружения POX в Exchange.
ms.openlocfilehash: a8797fe714fd23049094c3ec2475b93fec4282c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834867"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Служба POX автоматического обнаружения веб-ссылки для Exchange

Найдите справочные сведения для службы автообнаружения POX в Exchange.
  
Служба автообнаружения предоставляет сведения о конфигурации, используемые приложением для создания подключения к серверу Exchange. Можно использовать «Обычная старые XML» службы автообнаружения (POX) для отправки сообщений, которые состоят только из полезных данных XML, без любого заключающего конверты SOAP для обнаружения параметров, которые необходимо клиентское приложение для подключения к Exchange.
  
> [!NOTE]
> Для клиентов, предназначенных для версии Exchange, начиная с Exchange Server 2010 мы рекомендуем использовать службу автообнаружения SOAP вместо службы автообнаружения POX. Клиенты, предназначенных для Exchange 2007 необходимо использовать службу автообнаружения POX. Мы рекомендуем, что клиентов, использующих .NET Framework использовать управляемый API EWS, так как он содержит надежных и хорошо проверенные автообнаружения POX клиента. Дополнительные сведения о управляемый API EWS можно [приступить к работе с клиентскими приложениями, управляемый API веб-служб Exchange](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
В этом разделе приведены сведения об XML-элементы, отправленные между клиентом и сервером во время перенаправления запроса POX автообнаружения и параметров пользователя, которые возвращаются в ответе. Справочник по элементам XML содержит элементы представления сводки и описание возможных иерархии элементов, используйте элемент. В этой документации описываются экземпляры XML, отправленные между клиентом и сервером. Служба автообнаружения POX нет явных схемы.
  
В статьях в этом разделе приведены примеры и описания сообщений, которые используются для получения сведений о конфигурации автообнаружения с помощью службы автообнаружения POX. 
  
## <a name="in-this-section"></a>В этом разделе
<a name="bk_InThisSection"> </a>

- [Запрос автообнаружения POX для Exchange](pox-autodiscover-request-for-exchange.md)
    
- [POX ответа службы автообнаружения для Exchange](pox-autodiscover-response-for-exchange.md)
    
- [Элементы XML автоматического обнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>См. также

- [Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Автообнаружение для Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [SOAP ссылку веб-службы автообнаружения для Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

