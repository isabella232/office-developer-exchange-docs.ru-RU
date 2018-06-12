---
title: SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: Элемент SetPlayOnPhoneDialString определяет запрос на присвоение строке звонка по умолчанию для операции PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ) и запросы PlayOnPhoneGreeting операции (веб-служба единой системы обмена СООБЩЕНИЯМИ).
ms.openlocfilehash: fd82dc6ef0dd90a2318da93191f657005b7a5c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835450"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)

Элемент **SetPlayOnPhoneDialString** определяет запрос для установки строке звонка по умолчанию для запросов [PlayOnPhone операция (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphone-operation-um-web-service.md) , а [операция PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ)](playonphonegreeting-operation-um-web-service.md) . 
  
[SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setplayonphonedialstring-um-web-service.md)
  
```xml
<SetPlayOnPhoneDialString>
  <dialString>   </dialString>
</SetPlayOnPhoneDialString>
```

 **complexType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[dialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)](dialstring-um-web-service.md) <br/> |Номер телефона, чтобы установить в качестве строке звонка по умолчанию.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена СООБЩЕНИЯМИ)](setplayonphonedialstring-operation-um-web-service.md)

