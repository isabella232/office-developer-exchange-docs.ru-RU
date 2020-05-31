---
title: Рекуестедверсион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: Элемент Рекуестедверсион Указывает минимальную версию службы, на которую клиент хочет обработать запрос.
ms.openlocfilehash: 0d8682c33790d2d26001512ad9e2191ae52074d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835134"
---
# <a name="requestedversion-soap"></a>Рекуестедверсион (SOAP)

Элемент **рекуестедверсион** Указывает минимальную версию службы, на которую клиент хочет обработать запрос. 
  
```XML
<RequestedVersion/>
```

 **ексчанжеверсион**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Запрос (SOAP)](request-soap.md) <br/> |Содержит запрошенные параметры конфигурации и конечных пользователей.  <br/> |
|[Request (Жетдомаинсеттингс) (SOAP)](request-getdomainsettingssoap.md) <br/> |Представляет запрос на получение параметров домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение для элемента **рекуестедверсион** может быть Exchange2010, Exchange2010_SP1, Exchange2010_SP2 или Exchange2013.
  
## <a name="remarks"></a>Примечания

Если этот элемент не указан, используется последняя версия службы.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

