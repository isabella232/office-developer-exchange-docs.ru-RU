---
title: SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: 513a5072-c3ac-405f-98c2-0ab982d0a360
description: Элемент SetPlayOnPhoneDialString определяет запрос на задание строки набора по умолчанию для операций PlayOnPhone (веб-служба um) и операций PlayOnPhoneGreeting (веб-служба UM).
ms.openlocfilehash: e485fd092da29a3f54b1acc2b7e50167084e13fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540505"
---
# <a name="setplayonphonedialstring-um-web-service"></a>SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)

Элемент **SetPlayOnPhoneDialString** определяет запрос на задание строки набора по умолчанию для операций [PlayOnPhone (веб-служба um)](playonphone-operation-um-web-service.md) и [операций PlayOnPhoneGreeting](playonphonegreeting-operation-um-web-service.md) (веб-служба UM). 
  
[SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)](setplayonphonedialstring-um-web-service.md)
  
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
|[dialString (веб-служба единой системы обмена сообщениями)](dialstring-um-web-service.md) <br/> |Телефонный номер для набора в качестве строки набора по умолчанию.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)](setplayonphonedialstring-operation-um-web-service.md)

