---
title: Ссылка веб-службы soap Autodiscover для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Найдите справочные сведения для службы автооткрытия SOAP в Exchange.
ms.openlocfilehash: 488862f5797abfd71d33c916fa96970ab300a2c0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521356"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>Ссылка веб-службы soap Autodiscover для Exchange

Найдите справочные сведения для службы автооткрытия SOAP в Exchange.
  
Служба автооткрытия предоставляет сведения о конфигурации, которые приложение использует для создания подключения к Exchange серверу. Вы можете использовать службу автоматического обнаружения SOAP для отправки сообщений между клиентом и сервером Exchange, чтобы найти параметры, которые приложение будет использовать для подключения к Exchange. В отличие от службы автооткрытия POX, служба автооткрытия SOAP позволяет пакетно запрашивать автонаруже для параметров многих пользователей и более подробно контролировать, какие параметры возвращаются в ответе. 
  
> [!NOTE]
> Клиентам, целевым версиям Exchange, начиная с Exchange Server 2010 г., рекомендуется использовать службу автооткрытия SOAP (вместо службы автооткрытия POX). Клиенты, Exchange 2007 г., должны использовать службу автооткрытия POX. Мы рекомендуем клиентам, платформа .NET Framework использовать управляемый API EWS, так как он содержит надежный и хорошо протестированный клиент SOAP Autodiscover. Дополнительные сведения о управляемом API EWS см. в приложении [Get started with EWS Managed API client applications.](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx) 
  
В этом разделе приводится информация о элементах XML, которые отправляются между клиентом и сервером во время перенаправления запросов автонаружения SOAP и параметров пользователя, возвращаемого в ответ. Ссылка на элемент XML содержит сводки о том, что представляют элементы, и описание потенциальных иерархий элементов, содержащих элемент. 
  
В статьях в этом разделе описываются экземпляры XML, отправленные между клиентом и сервером. Схему, описываемую этими элементами, можно найти в виртуальном каталоге сервера, на котором размещена служба автооткрытия SOAP.
  
Темы операций WSDL в этом разделе предоставляют обзор действий операции, а также примеров запросов и ответов на операции. Сведения о версии можно использовать, чтобы определить, доступны ли те функции, которые вы хотите использовать в запущенной версии продукта. Примеры в темах операции также помогают понять структуру XML, включенного в сообщения SOAP, которые отправляются на сервер и с него.
  
В этом разделе также приводится примеры и описания сообщений, используемых для получения сведений о конфигурации автооткрытия с помощью службы автооткрытия SOAP. 
  
## <a name="in-this-section"></a>В этом разделе:
<a name="bk_InThisSection"> </a>

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
    
- [Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
    
- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
    
- [Операция GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Элементы XML автооткрытия SOAP для Exchange 2013 г.](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>См. также


- [Ссылка на веб-службу автооткрытия для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Автообнаружение в Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Поиск точек соединения с помощью службы автообнаружения](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [Получение параметров пользователя из Exchange с помощью службы автообнаружения](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Получение параметров домена с сервера Exchange](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

