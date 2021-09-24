---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: Элемент RequestedVersion указывает минимальную версию службы, в которую клиент хочет, чтобы запрос был обработан.
ms.openlocfilehash: 390dee362bf2e6c2bdeac4e0e5564ecbd59b7319
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513334"
---
# <a name="requestedversion-soap"></a>RequestedVersion (SOAP)

Элемент **RequestedVersion** указывает минимальную версию службы, в которую клиент хочет, чтобы запрос был обработан. 
  
```XML
<RequestedVersion/>
```

 **ExchangeVersion**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Request (SOAP)](request-soap.md) <br/> |Содержит запрашиваемую конфигурацию параметров и целевых пользователей.  <br/> |
|[Request (GetDomainSettings) (SOAP)](request-getdomainsettingssoap.md) <br/> |Представляет запрос на получения параметров домена.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **RequestedVersion** может быть Exchange2010, Exchange2010_SP1, Exchange2010_SP2 Или Exchange2013.
  
## <a name="remarks"></a>Заметки

Если этого элемента нет, используется последняя версия службы.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
  
[Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

