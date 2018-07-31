---
title: Элементы XML автоматического обнаружения SOAP для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Найдите XML элемент справочные сведения для веб-службы автообнаружения SOAP в Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353394"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Элементы XML автоматического обнаружения SOAP для Exchange 2013

Найдите XML элемент справочные сведения для веб-службы автообнаружения SOAP в Exchange.
  
В этом разделе документации основано на экземпляры элемент XML автоматического обнаружения SOAP, отправленные между клиентом и сервером. В этой документации экземпляр XML основано на WSDL и схеме файлы, расположенные в виртуальном каталоге, на котором размещается служба автообнаружения SOAP. Прошедшего проверку подлинности пользователи могут просматривать файлы WSDL и схемы с помощью URL-адреса, который похож на один из следующих:
  
- Расположение WSDL-файла: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` или`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- Расположение схемы сообщений: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` или`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
Расположение службы автообнаружения WSDL SOAP и схеме файлов зависит от установки Exchange.
  
Файл схемы messages.xsd описывает XML-элементы, которые могут быть отправлены в SOAP автообнаружения заголовок и тело SOAP. Этот файл предоставляет общая схема XML-структура может быть для диалога сообщения заданного запросов и ответов. Фактические XML-структура, пересылаемые между клиентом и сервером на основе параметров и контекст, в котором она используется. Файлы схемы определения возможности возможные XML. Фактический диапазон XML, отправляемые по сети основано на какие операция называется запрошенные данные и параметры на сервере. 
  
## <a name="related-sections"></a>Связанные разделы

- [SOAP ссылку веб-службы автообнаружения для Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)    
- [Единой системы обмена сообщениями веб-службы ссылки для Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>См. также

- [Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Автообнаружение для Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

