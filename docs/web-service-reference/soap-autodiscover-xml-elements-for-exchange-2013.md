---
title: Элементы XML автооткрытия SOAP для Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Найдите справочные сведения об элементах XML для веб-службы автооткрытия SOAP в Exchange.
ms.openlocfilehash: 5dcf4d6cd7a2b0b2987e59530dfbaae7b9993242
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539096"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>Элементы XML автооткрытия SOAP для Exchange 2013 г.

Найдите справочные сведения об элементах XML для веб-службы автооткрытия SOAP в Exchange.
  
Документация в этом разделе основана на экземплярах элементов XML-элементов soap Autodiscover, которые отправляются между клиентом и сервером. Эта документация XML-экземпляра основана на WSDL-файлах и файлах схем, расположенных в виртуальном каталоге, в котором размещена служба автооткрытия SOAP. Пользователи с проверкой подлинности могут просматривать файлы WSDL и схемы с помощью URL-адреса, аналогичного одному из следующих:
  
- Расположение файла WSDL: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` или `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- Расположение схемы сообщений: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` или `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
Расположение файлов WSDL и схемы мыла автооткрываемого оборудования зависит от Exchange установки.
  
В файле схемы messages.xsd описываются элементы XML, которые можно отправить в заголовке мыла автообнаружения и теле SOAP. В этом файле содержится общая дорожная карта структуры XML для данного взаимодействия сообщений с запросами и ответами. Фактическая структура XML, которая отправляется между клиентом и сервером, основана на параметрах и контексте, в котором она используется. Файлы схемы определяют возможности XML. Фактический диапазон XML, который отправляется по проводу, зависит от того, какая операция называется, запрашиваемая информация и параметры на стороне сервера. 
  
## <a name="related-sections"></a>Связанные разделы

- [Ссылка веб-службы soap Autodiscover для Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)    
- [Ссылка на веб-службу единой системы обмена сообщениями для Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>См. также

- [Ссылка на веб-службу автооткрытия для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Автообнаружение в Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

