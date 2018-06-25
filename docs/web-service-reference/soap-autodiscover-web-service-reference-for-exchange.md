---
title: SOAP ссылку веб-службы автообнаружения для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Найдите справочные сведения для службы автообнаружения SOAP в Exchange.
ms.openlocfilehash: 1cb24a8667c71028f3dead78d9fa533dc9547a64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835514"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a>SOAP ссылку веб-службы автообнаружения для Exchange

Найдите справочные сведения для службы автообнаружения SOAP в Exchange.
  
Служба автообнаружения предоставляет сведения о конфигурации, используемые приложением для создания подключения к серверу Exchange. Служба автообнаружения SOAP можно использовать для отправки сообщений между клиентским приложением и Exchange server, чтобы найти параметры приложения будет использоваться для подключения к Exchange. В отличие от службы автообнаружения POX служба автообнаружения SOAP обеспечивает пакетных запросах автообнаружения для параметров количество пользователей и более детальный контроль над тем, какие параметры возвращаются в ответе. 
  
> [!NOTE]
> Для клиентов, предназначенных для версии Exchange, начиная с Exchange Server 2010 мы рекомендуем использовать службы автообнаружения SOAP (вместо службы автообнаружения POX). Клиенты, предназначенных для Exchange 2007 необходимо использовать службу автообнаружения POX. Мы рекомендуем, что клиентов, использующих .NET Framework использовать управляемый API EWS, так как он содержит надежных и хорошо проверенные клиента автообнаружения SOAP. Дополнительные сведения о управляемый API EWS можно [приступить к работе с клиентскими приложениями, управляемый API веб-служб Exchange](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
В этом разделе приведены сведения об XML-элементы, отправленные между клиентом и сервером во время перенаправления запроса SOAP автообнаружения и параметров пользователя, которые возвращаются в ответе. Справочник по элементам XML содержит элементы представления сводки и описание возможных иерархии элементов, которые содержат элемент. 
  
В статьях этого раздела описывается экземпляры XML, отправленные между клиентом и сервером. Схема, описывающая этих элементов можно найти в виртуальном каталоге сервера, на котором размещается служба автообнаружения SOAP.
  
Операции WSDL, в этом разделе описываются что не обзор операций и примеры операция запроса и ответа. Можно использовать сведения о версии, для определения, доступны ли компоненты, которые вы хотите использовать в версию продукта, выполняется. Примеров в разделах операции помогут понять структуру XML, который включен в сообщения SOAP, и с сервера.
  
В этом разделе также приведены примеры и описания сообщений, которые используются для получения сведений о конфигурации автообнаружения с помощью службы автообнаружения SOAP. 
  
## <a name="in-this-section"></a>В этом разделе
<a name="bk_InThisSection"> </a>

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)
    
- [Операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)
    
- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
    
- [Операция GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)
    
- [Элементы XML автоматического обнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a>См. также


- [Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Автообнаружение для Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Использование службы автообнаружения для поиска точек подключения](http://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [Получить параметры пользователя из Exchange с помощью службы автообнаружения](http://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [Получение параметров домена с сервера Exchange](http://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

