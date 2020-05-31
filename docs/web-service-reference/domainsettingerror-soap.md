---
title: Домаинсеттинжеррор (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: Элемент Домаинсеттинжеррор представляет ошибку, возникшую при получении параметра домена. Представляет ошибку в запросе Жетдомаинсеттингс.
ms.openlocfilehash: 08b0a47acea8d35ec78efd701168a251771effac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762216"
---
# <a name="domainsettingerror-soap"></a>Домаинсеттинжеррор (SOAP)

Элемент **домаинсеттинжеррор** представляет ошибку, возникшую при получении параметра домена. Представляет ошибку в запросе **жетдомаинсеттингс** . 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 **домаинсеттинжеррор**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Определяет код ошибки, связанный с конкретным запросом.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Содержит сообщение об ошибке, связанное с конкретным запросом.  <br/> |
|[Свойства settingname (SOAP)](settingname-soap.md) <br/> |Представляет имя параметра.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домаинсеттинжеррорс (SOAP)](domainsettingerrors-soap.md) <br/> |Содержит сведения об ошибках для параметров, которые не удалось вернуть.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

