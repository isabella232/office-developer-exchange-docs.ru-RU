---
title: Status (веб-служба единой системы обмена сообщениями — SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: Элемент Status определяет значение, которое будет использоваться в SetOofStatus операции (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 865152baf28c22578664e16db2dcd5f82a04af98
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459982"
---
# <a name="status-um-web-service---setoofstatus"></a>Status (веб-служба единой системы обмена сообщениями — SetOofStatus)

Элемент **Status** определяет значение, которое будет использоваться в [SetOofStatus операции (веб-служба единой системы обмена сообщениями)](setoofstatus-operation-um-web-service.md) . 
  
[SetOofStatus (веб-служба единой системы обмена сообщениями)](setoofstatus-um-web-service.md)
  
[Status (веб-служба единой системы обмена сообщениями — SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SetOofStatus (веб-служба единой системы обмена сообщениями)](setoofstatus-um-web-service.md) <br/> |Определяет запрос на установку состояния единой системы обмена сообщениями (отсутствие на работе) для пользователя, который выполняет запрос.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать логическое значение. Ниже перечислены возможные значения.
  
- Верно.
    
- False
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SetOofStatus (веб-служба единой системы обмена сообщениями)](setoofstatus-operation-um-web-service.md)

