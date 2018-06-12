---
title: Элементы XML веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Найдите справочные сведения для веб-служб Exchange XML элементы в Exchange.
ms.openlocfilehash: 046a985ae4696616d28a0891ffe0aa8cc0552307
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762412"
---
# <a name="ews-xml-elements-in-exchange"></a>Элементы XML веб-служб Exchange в Exchange

Найдите справочные сведения для веб-служб Exchange XML элементы в Exchange.
  
Веб-служб Exchange (EWS) — это служба веб-SOAP, что означает, что запрос и ответ сообщения, отправленные между клиентом и сервером состоят из XML-элементы. В этом разделе документации основано на экземпляры XML, отправленные между клиентом и сервером. Экземпляры XML определяются в файлах WSDL и схемы, которые расположены в виртуальном каталоге, на котором размещается веб-служб Exchange. Пользователям, прошедшим проверку подлинности пользователя могут просматривать файлы WSDL и схемы с помощью следующие URL-адреса, где \<yourclientaccessserver\> — это имя сервера клиентского доступа:
  
- http://\<yourclientaccessserver\>.com/ews/services.wsdl — расположение WSDL-файла.
    
- http://\<yourclientaccessserver\>.com/ews/messages.xsd — расположение схемы сообщений.
    
- http://\<yourclientaccessserver\>.com/ews/types.xsd — расположение схемы типов.
    
Файлы схемы, которые описывают элементы XML веб-служб Exchange предоставляют общие схема XML структуры, возможно, для взаимодействия сообщения запросов и ответов. Фактические XML-структура, пересылаемые между клиентом и сервером изменяется в зависимости от операции, который будет вызываться, нужные данные и параметры на сервере.
  
Веб-служб Exchange WSDL-файла, services.wsdl, не соответствует полностью стандартный WSDL-ФАЙЛУ, так как он не включает определение WSDL службы. Это так, как веб-служб Exchange не может быть размещены на компьютере с предварительно заданных адресов. Можно использовать службу автообнаружения для получения адреса конечной точки веб-служб Exchange. Некоторые генераторы клиентскую объектную модель анализа WSDL-файла и могут возникнуть ошибки, так как WSDL-файла не содержит определение WSDL службы. Если генератор объектной модели возникают ошибки, можно вставить заполнитель определения службы WSDL.
  
> [!TIP]
> Если вы используете .NET Framework для разработки приложения, рекомендуется использовать [Управляемый API веб-служб Exchange](http://aka.ms/ews-managed-api-readme), а не генератор объектной модели. Управляемый API веб-служб Exchange предоставляет простой в использовании объектную модель для обработки сериализации и десериализации XML веб-служб Exchange. Дополнительные сведения можно [приступить к работе с клиентскими приложениями, управляемый API веб-служб Exchange](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Файл схемы messages.xsd содержит определения элементов для элементов верхнего уровня в тексте запроса SOAP. За исключением коды ответа об ошибках большая часть определения в messages.xsd относятся только к операции. Схема types.xsd содержит определения для заголовков SOAP и общие определения, которые являются общими для операций.
  
## <a name="see-also"></a>См. также

- [Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)
- [Операции EWS в Exchange](ews-operations-in-exchange.md)
- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Автообнаружение для Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

