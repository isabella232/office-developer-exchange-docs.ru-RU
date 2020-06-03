---
title: Элементы XML веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Справочные сведения о XML-элементах EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 29b90ad137141e30484ef804b6fcb6bb049ef3e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526118"
---
# <a name="ews-xml-elements-in-exchange"></a>Элементы XML веб-служб Exchange в Exchange

Справочные сведения о XML-элементах EWS в Exchange.
  
Веб-службы Exchange (EWS) — это веб-служба на основе SOAP, которая означает, что сообщения запроса и ответа, которые передаются между клиентом и сервером, состоят из XML-элементов. Документация в этом разделе основана на экземплярах XML, которые передаются между клиентом и сервером. Экземпляры XML определяются в файлах WSDL и Schema, расположенных в виртуальном каталоге, на котором размещается EWS. Если вы прошедший проверку подлинности пользователя, вы можете перейти к файлам WSDL и Schema, используя следующие URL-адреса, где \<yourclientaccessserver\> — имя сервера клиентского доступа:
  
- http:// \<yourclientaccessserver\> . com/EWS/Services. WSDL — расположение WSDL-файла.
    
- http:// \<yourclientaccessserver\> . com/EWS/messages. xsd — расположение схемы messages.
    
- http:// \<yourclientaccessserver\> . com/EWS/Types. xsd — расположение схемы типов.
    
Файлы схемы, описывающие элементы XML EWS, предоставляют общий план структуры XML, который можно использовать для взаимодействия с сообщениями request-response. Реальная структура XML, которая передается между клиентом и сервером, зависит от вызываемой операции, запрашиваемых сведений и параметров на стороне сервера.
  
WSDL-файл EWS, Services. WSDL, не полностью соответствует стандарту WSDL, так как он не включает определение службы WSDL. Это вызвано тем, что веб-сервер EWS не предназначен для размещения на компьютере с предварительно определенным адресом. Вы можете использовать службу автообнаружения, чтобы получить адрес конечной точки EWS. Некоторые генераторы объектной модели на стороне клиента анализируют WSDL и могут возникать из-за ошибки, потому что WSDL-файл не содержит определения службы WSDL. Если генератор объектной модели обнаруживает ошибку, вы можете вставить заполнитель для определения службы WSDL.
  
> [!TIP]
> Если вы используете .NET Framework для разработки приложения, мы рекомендуем использовать [управляемый API EWS](http://aka.ms/ews-managed-api-readme), а не генератор объектной модели. Управляемый API EWS предоставляет простую в использовании объектную модель для обработки сериализации и десериализации XML-кода EWS. Дополнительные сведения см. в статье [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx). 
  
Файл схемы messages. XSD содержит определения элементов для элементов верхнего уровня в теле SOAP. За исключением кодов отклика об ошибках, большинство определений в messages. xsd характерны для операции. Схема Types. XSD содержит определения для заголовков SOAP и все общие определения, которые используются совместно несколькими операциями.
  
## <a name="see-also"></a>См. также

- [Справка по службам EWS для Exchange](ews-reference-for-exchange.md)
- [Операции EWS в Exchange](ews-operations-in-exchange.md)
- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Автообнаружение для Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

