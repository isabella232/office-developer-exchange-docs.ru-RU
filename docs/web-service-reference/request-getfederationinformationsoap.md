---
title: Request (Жетфедератионинформатион) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: Элемент request представляет запрос Жетфедератионинформатионрекуест (SOAP).
ms.openlocfilehash: dbd88537d03f6325cf0025d08c63ae486544d705
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459583"
---
# <a name="request-getfederationinformation-soap"></a>Request (Жетфедератионинформатион) (SOAP)

Элемент **request** представляет запрос [жетфедератионинформатионрекуест (SOAP)](getfederationinformationrequest-soap.md) . 
  
```XML
<Request>
   <Domain/>
</Request>
```

 **жетфедератионинформатионрекуест**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домен (Жетфедератионинформатион) (SOAP)](domain-getfederationinformationsoap.md) <br/> |Определяет домен, который имеет доверие федерации.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Жетфедератионинформатионрекуестмессаже (SOAP)](getfederationinformationrequestmessage-soap.md) <br/> |Подготавливает вызов к серверу для запроса данных конфигурации для службы маркеров безопасности (STS).  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Работа со службой автообнаружения](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

