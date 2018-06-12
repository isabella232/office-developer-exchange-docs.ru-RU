---
title: DocumentSharingLocationCollectionSetting (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e3346f9-7a55-4e87-b121-9b1ee7f227f4
description: Элемент DocumentSharingLocationCollectionSetting — это пользователь, то есть параметр коллекцию документации, совместное использование расположения и метаданных.
ms.openlocfilehash: 9871e3fccdcce95fc275768d99159c70f57a07af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762197"
---
# <a name="documentsharinglocationcollectionsetting-soap"></a>DocumentSharingLocationCollectionSetting (SOAP)

Элемент **DocumentSharingLocationCollectionSetting** — это пользователь, то есть параметр коллекцию документации, совместное использование расположения и метаданных. 
  
[DocumentSharingLocationCollectionSetting (SOAP)](documentsharinglocationcollectionsetting-soap.md)
  
```XML
<DocumentSharingLocationCollectionSetting>
    <DocumentSharingLocations />
</DocumentSharingLocationCollectionSetting>
```

 **DocumentSharingLocationCollectionSetting**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |Представляет расположение и метаданных в список расположения общих документов.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Параметры пользователя (SOAP)](usersettings-soap.md) <br/> |Представляет коллекцию параметров пользователя.  <br/> |
   
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

