---
title: Документшаринглокатионколлектионсеттинг (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 0e3346f9-7a55-4e87-b121-9b1ee7f227f4
description: Элемент Документшаринглокатионколлектионсеттинг представляет параметр пользователя, который представляет собой коллекцию местоположений и метаданных общего доступа к документации.
ms.openlocfilehash: 2a52f639a1f1bf638aacc78666c58aed1fae0fa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457055"
---
# <a name="documentsharinglocationcollectionsetting-soap"></a>Документшаринглокатионколлектионсеттинг (SOAP)

Элемент **документшаринглокатионколлектионсеттинг** представляет параметр пользователя, который представляет собой коллекцию местоположений и метаданных общего доступа к документации. 
  
[Документшаринглокатионколлектионсеттинг (SOAP)](documentsharinglocationcollectionsetting-soap.md)
  
```XML
<DocumentSharingLocationCollectionSetting>
    <DocumentSharingLocations />
</DocumentSharingLocationCollectionSetting>
```

 **документшаринглокатионколлектионсеттинг**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Документшаринглокатионс (SOAP)](documentsharinglocations-soap.md) <br/> |Представляет расположение и метаданные для списка расположений общего доступа к документам.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Усерсеттингс (SOAP)](usersettings-soap.md) <br/> |Представляет коллекцию параметров пользователя.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Справочные материалы по веб-службе автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [XML-элементы автообнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

