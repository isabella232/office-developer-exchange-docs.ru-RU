---
title: Status (веб-служба единой системы обмена сообщениями — SetOofStatus)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- Status
api_type:
- schema
ms.assetid: 893bcff1-ccdc-493f-b366-ce8a68c813bd
description: Элемент Status определяет значение, используемого в запросе операции SetOofStatus (веб-служба um).
ms.openlocfilehash: fc4806e4978ae51ec6113ff8fd45da7db223a071
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546940"
---
# <a name="status-um-web-service---setoofstatus"></a>Status (веб-служба единой системы обмена сообщениями — SetOofStatus)

Элемент **Status** определяет значение, используемого в запросе [операции SetOofStatus (веб-служба um).](setoofstatus-operation-um-web-service.md) 
  
[SetOofStatus (веб-служба единой системы обмена сообщениями)](setoofstatus-um-web-service.md)
  
[Status (веб-служба единой системы обмена сообщениями — SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
```xml
<SetOofStatus>
  <status/>
</SetOofStatus>
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
|[SetOofStatus (веб-служба единой системы обмена сообщениями)](setoofstatus-um-web-service.md) <br/> |Определяет запрос на определение состояния единой системы обмена сообщениями Office (OOF) для пользователя, который делает запрос.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется значение Boolean. Ниже перечислены возможные значения.
  
- Верно
    
- Неверно
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SetOofStatus (веб-служба единой системы обмена сообщениями)](setoofstatus-operation-um-web-service.md)

