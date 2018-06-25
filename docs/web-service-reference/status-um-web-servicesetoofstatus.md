---
title: Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)
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
description: Элемент Status определяет значение для использования в запросе SetOofStatus операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: 57b4f8fe1a64341b1c2ae0a06bc98f1c9cfd28c4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835583"
---
# <a name="status-um-web-service---setoofstatus"></a>Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)

Элемент **Status** определяет значение для использования в запросе [SetOofStatus операции (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setoofstatus-operation-um-web-service.md) . 
  
[SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setoofstatus-um-web-service.md)
  
[Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)](status-um-web-servicesetoofstatus.md)
  
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
|[SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setoofstatus-um-web-service.md) <br/> |Определяет запрос для задания состояния единой системы обмена сообщениями об отсутствии на работе Office (OOF) для пользователя, который выполняет запрос.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Логическое значение является обязательным. Ниже перечислены возможные значения.
  
- Истина
    
- Ложь
    
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setoofstatus-operation-um-web-service.md)

