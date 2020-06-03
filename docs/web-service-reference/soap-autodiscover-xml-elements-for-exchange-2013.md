---
title: XML-элементы автообнаружения SOAP для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Найдите справочные сведения о XML-элементе для веб-службы автообнаружения SOAP в Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465186"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a>XML-элементы автообнаружения SOAP для Exchange 2013

Найдите справочные сведения о XML-элементе для веб-службы автообнаружения SOAP в Exchange.
  
Документация в этом разделе основана на экземплярах XML-элементов автообнаружения SOAP, которые передаются между клиентом и сервером. Эта документация по экземпляру XML основана на файлах WSDL и Schema, расположенных в виртуальном каталоге, где размещается служба автообнаружения SOAP. Пользователи, прошедшие проверку подлинности, могут перейти к файлам WSDL и Schema, используя URL-адрес, подобный одному из следующих:
  
- Расположение WSDL-файла: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` или`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`
    
- Расположение схемы messages: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` или`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd` 
    
Расположение WSDL и файлов схемы автообнаружения SOAP зависит от установки Exchange.
  
В файле схемы messages. xsd описываются элементы XML, которые можно отправить в заголовке SOAP автообнаружения и теле SOAP. В этом файле представлен общий обзор структуры XML, которую можно использовать для взаимодействия с сообщением о ответе на запрос. Фактическая структура XML, которая передается между клиентом и сервером, основана на параметрах и контексте, в котором они используются. Файлы схемы определяют, какой возможен XML-файл. Фактический диапазон XML-данных, передаваемых по сети, зависит от того, какая операция вызывается, запрашиваемые сведения и параметры на стороне сервера. 
  
## <a name="related-sections"></a>Связанные разделы

- [Справочник по веб-службе автообнаружения SOAP для Exchange](soap-autodiscover-web-service-reference-for-exchange.md)    
- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)    
- [Справочные материалы по веб-службе единой системы обмена сообщениями для Exchange](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a>См. также

- [Справочные материалы по веб-службе автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Автообнаружение в Exchange](../exchange-web-services/autodiscover-for-exchange.md)
- [Начало работы с веб-службами Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
    

