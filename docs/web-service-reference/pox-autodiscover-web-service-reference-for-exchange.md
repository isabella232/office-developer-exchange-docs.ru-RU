---
title: Справочник по веб-службе автообнаружения POX для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Найдите справочные сведения о службе автообнаружения POX в Exchange.
ms.openlocfilehash: 3c0ca368f4427be7759e2db58fb418b4822dea8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465655"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Справочник по веб-службе автообнаружения POX для Exchange

Найдите справочные сведения о службе автообнаружения POX в Exchange.
  
Служба автообнаружения предоставляет сведения о конфигурации, которые приложение использует для создания подключения к серверу Exchange. Службу автообнаружения "Plain Old XML" (POX) можно использовать для отправки сообщений, состоящих только из полезных данных XML, без почтовых конвертов SOAP, чтобы определить параметры, которые должны быть у клиентского приложения для подключения к Exchange.
  
> [!NOTE]
> Для клиентов, использующих версии Exchange, начиная с Exchange Server 2010, рекомендуется использовать службу автообнаружения SOAP вместо службы автообнаружения POX. Клиентам, которые нацелены на Exchange 2007, необходимо использовать службу автообнаружения POX. Мы рекомендуем использовать для клиентов, использующих платформу .NET Framework, управляемый API EWS, так как он содержит надежный и хорошо протестированный клиент автообнаружения POX. Дополнительные сведения об управляемом API EWS можно найти в статье Начало [работы с клиентскими приложениями для управляемого API EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
В этом разделе представлены сведения об элементах XML, которые передаются между клиентом и сервером во время перенаправлений запросов автообнаружения POX, и пользовательских параметров, возвращаемых в ответе. Справочник по XML-элементам содержит сводки элементов, которые представляют элементы, и описание потенциальных иерархий элементов, использующих этот элемент. В этой документации описываются экземпляры XML, которые передаются между клиентом и сервером. Служба автообнаружения POX не имеет явной схемы.
  
В статьях этого раздела приводятся примеры и описания сообщений, которые используются для получения сведений о конфигурации автообнаружения с помощью службы автообнаружения POX. 
  
## <a name="in-this-section"></a>В этой статье
<a name="bk_InThisSection"> </a>

- [Запрос автообнаружения POX для Exchange](pox-autodiscover-request-for-exchange.md)
    
- [Отклик автообнаружения POX для Exchange](pox-autodiscover-response-for-exchange.md)
    
- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>См. также

- [Справочные материалы по веб-службе автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Автообнаружение в Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [Справочник по веб-службе автообнаружения SOAP для Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Начало работы с веб-службами Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

