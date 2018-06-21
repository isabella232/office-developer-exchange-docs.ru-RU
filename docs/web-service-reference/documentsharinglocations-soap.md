---
title: DocumentSharingLocations (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 394f6015-721b-4800-9286-039d430f09b3
description: Элемент DocumentSharingLocations содержит список местоположения и сведения о метаданных для общего доступа к расположение документа.
ms.openlocfilehash: 72d1ae9f01ad45441b4e255f2fb6353be2dc8d28
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/21/2018
ms.locfileid: "19762202"
---
# <a name="documentsharinglocations-soap"></a>DocumentSharingLocations (SOAP)

Элемент **DocumentSharingLocations** содержит список местоположения и сведения о метаданных для общего доступа к расположение документа. 
  
```XML
<DocumentSharingLocations>
   <DocumentSharingLocation />
</DocumentSharingLocations>
```

 **DocumentSharingLocations**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Содержит расположение и метаданных для общего доступа к расположение документа.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DocumentSharingLocationCollectionSetting (SOAP)](documentsharinglocationcollectionsetting-soap.md) <br/> |Представляет пользователя, то есть параметр коллекцию документации, совместное использование расположения и метаданных.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Элементы XML автоматического обнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

