---
title: Ссылка веб-службы автооткрытия POX для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Найдите справочные сведения для службы автонаружия POX в Exchange.
ms.openlocfilehash: b28ea64a82960a84dee06c5055ee915614f4fde7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516421"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a>Ссылка веб-службы автооткрытия POX для Exchange

Найдите справочные сведения для службы автонаружия POX в Exchange.
  
Служба автооткрытия предоставляет сведения о конфигурации, которые приложение использует для создания подключения к Exchange серверу. Для отправки сообщений, состоящих только из полезной нагрузки XML без всяких конвертов SOAP, можно использовать службу автоматического обнаружения XML (POX), чтобы найти параметры, которые должны быть у клиентского приложения для подключения к Exchange.
  
> [!NOTE]
> Клиентам, целевым версиям Exchange начиная с Exchange Server 2010 г., рекомендуется использовать службу автооткрытия SOAP вместо службы автооткрытия POX. Клиенты, Exchange 2007 г., должны использовать службу автооткрытия POX. Мы рекомендуем клиентам, платформа .NET Framework использовать управляемый API EWS, так как он содержит надежный и хорошо протестированный клиент poX Autodiscover. Дополнительные сведения о управляемом API EWS см. в приложении [Get started with EWS Managed API client applications.](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx) 
  
В этом разделе приводится информация о элементах XML, которые отправляются между клиентом и сервером во время перенаправления запросов автонаружения POX, и параметры пользователя, возвращаемого в ответ. Ссылка на элемент XML содержит сводки о том, что представляют элементы, и описание потенциальных иерархий элементов, которые используют этот элемент. Эта документация охватывает экземпляры XML, отправленные между клиентом и сервером. Служба автооткрытия POX не имеет явной схемы.
  
В статьях в этом разделе описаны примеры и описания сообщений, используемых для получения сведений о конфигурации автооткрытия с помощью службы автооткрытия POX. 
  
## <a name="in-this-section"></a>В этом разделе:
<a name="bk_InThisSection"> </a>

- [Запрос автооткрытия POX для Exchange](pox-autodiscover-request-for-exchange.md)
    
- [Ответ автооткрытия POX для Exchange](pox-autodiscover-response-for-exchange.md)
    
- [Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a>См. также

- [Ссылка на веб-службу автооткрытия для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Автообнаружение в Exchange](../exchange-web-services/autodiscover-for-exchange.md)   
- [Ссылка веб-службы soap Autodiscover для Exchange](soap-autodiscover-web-service-reference-for-exchange.md)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

