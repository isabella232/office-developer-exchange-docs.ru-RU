---
title: IsMeetingResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsMeetingResponse
api_type:
- schema
ms.assetid: 85090943-81c6-4fbe-a2db-007dced6a4cf
description: Элемент IsMeetngResponsequest указывает, должны ли входящие сообщения быть ответом на собрания, чтобы применить условие или исключение.
ms.openlocfilehash: ff6008eef7ae5198738e68db62303b06a619e41d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532753"
---
# <a name="ismeetingresponse"></a>IsMeetingResponse

Элемент **IsMeetngResponsequest** указывает, должны ли входящие сообщения быть ответом на собрания, чтобы применить условие или исключение. 
  
```XML
<IsMeetingResponse/>true | false</IsMeetingResponse>
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
|[Условия](conditions.md) <br/> |Представляет условия, которые, если удовлетворены, запускают действия правила для правила.  <br/> |
|[Исключения](exceptions.md) <br/> |Представляет все доступные условия исключения правил для правила "Входящие".  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение текста указывает **на** то, что сообщение должно быть ответом собрания, чтобы применить условие или исключение. Ложное **текстовое** значение указывает на то, что сообщение не должно быть ответом собрания, чтобы применить условие или исключение. 
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

