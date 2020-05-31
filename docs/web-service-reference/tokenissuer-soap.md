---
title: Токениссуер (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: Элемент Токениссуер указывает URI (SOAP) и конечную точку (SOAP) для службы маркеров безопасности.
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840196"
---
# <a name="tokenissuer-soap"></a>Токениссуер (SOAP)

Элемент **токениссуер** указывает [URI (SOAP)](uri-soap.md) и [конечную точку (SOAP)](endpoint-soap.md) для службы маркеров безопасности. 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 **токениссуер**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[URI (SOAP)](uri-soap.md) <br/> |Универсальный код ресурса (URI) службы маркеров безопасности, который выдал маркер безопасности.  <br/> |
|[Конечная точка (SOAP)](endpoint-soap.md) <br/> |URI конечной точки веб-службы.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Токениссуерс (SOAP)](tokenissuers-soap.md) <br/> |Представляет коллекцию URI-кодов службы маркеров безопасности [(SOAP)](uri-soap.md) и [КОНЕЧНОЙ точки (SOAP)](endpoint-soap.md).  <br/> |
   
## <a name="remarks"></a>Примечания

Используйте элемент **токениссуер** для указания службы маркеров безопасности при использовании маркеров безопасности. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Справочные материалы по веб-службе автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[XML-элементы автообнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

