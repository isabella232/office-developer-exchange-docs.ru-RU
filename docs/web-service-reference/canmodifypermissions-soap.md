---
title: CanModifyPermissions (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9693de1a-0c76-4898-8f4d-a8693fb005b3
description: Элемент CanModifyPermissions указывает, может ли пользователь изменить разрешения на доступ к документу, расположение для обмена.
ms.openlocfilehash: 16526cb79eeca591af6e009e67959a1c3b58a5d7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761666"
---
# <a name="canmodifypermissions-soap"></a>CanModifyPermissions (SOAP)

Элемент **CanModifyPermissions** указывает, может ли пользователь изменить разрешения на доступ к документу, расположение для обмена. 
  
```XML
<CanModifyPermissions /> 
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DocumentSharingLocation (SOAP)](documentsharinglocation-soap.md) <br/> |Представляет сведения о расположении и метаданных для документа расположение для обмена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Логическое значение элемента **CanModifyPermissions** указывает, будет ли пользователи смогут изменять разрешения на доступ к месту общего доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)


[Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
  
[Элементы XML автоматического обнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

