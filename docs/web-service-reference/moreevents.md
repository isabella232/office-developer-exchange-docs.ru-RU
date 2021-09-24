---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: Элемент MoreEvents указывает, есть ли в очереди больше событий, которые будут доставлены клиенту.
ms.openlocfilehash: 7a19349e406a7e55e52c8a8cf0c3febba0a7301b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521811"
---
# <a name="moreevents"></a>MoreEvents

Элемент **MoreEvents** указывает, есть ли в очереди больше событий, которые будут доставлены клиенту. 
  
```xml
<MoreEvents/>
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
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет значение Boolean. Значение true **указывает** на то, что в очереди больше событий. Значение false **указывает,** что в очереди больше нет событий. Это свойство доступно только для чтения. 
  
## <a name="remarks"></a>Заметки

В случае уведомлений Pull  истинное значение этого элемента указывает клиенту, что для получения оставшихся событий должен быть выдан другой запрос GetEvents. Предполагая, что спецификации клиента требуют минимальной задержки для уведомлений о событиях, запросы GetEvents должны продолжаться непрерывно, пока не будет возвращено ложное значение  **MoreEvents.** 
  
В случае push-уведомлений  истинное значение **для MoreEvents** указывает клиенту, что для доставки оставшихся событий клиенту будет отправлен другой запрос на уведомление. Подобно уведомлениям Pull, эти последующие запросы будут непрерывно выполняться до тех пор, пока очередь событий на сервере клиентского доступа не будет пуста. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция Unsubscribe](unsubscribe-operation.md)

