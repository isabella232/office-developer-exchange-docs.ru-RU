---
title: Домаинсеттинжеррорс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a4ce19de-f560-4984-8047-ecbbc86c9b91
description: Элемент Домаинсеттингсеррорс содержит сведения об ошибке для параметров, которые не могут быть возвращены.
ms.openlocfilehash: 4e7ee29c2bc680a1938b75189c2ac3c214f7d2b5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530707"
---
# <a name="domainsettingerrors-soap"></a>Домаинсеттинжеррорс (SOAP)

Элемент **домаинсеттингсеррорс** содержит сведения об ошибке для параметров, которые не могут быть возвращены. 
  
```XML
<DomainSettingsErrors>
   <DomainSettingsError/>
</DomainSettingsErrors>
```

 **домаинсеттингсеррорс**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домаинсеттинжеррор (SOAP)](domainsettingerror-soap.md) <br/> |Представляет ошибку, возникшую при получении параметра домена. Представляет ошибку в запросе операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домаинреспонсе (SOAP)](domainresponse-soap.md) <br/> |Содержит запрошенные параметры для указанного домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

