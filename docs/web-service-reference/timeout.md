---
title: Timeout
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Timeout
api_type:
- schema
ms.assetid: c2e1ca5a-6667-4f6f-aac4-89de33bddc54
description: Элемент timeout представляет продолжительность в минутах, в течение которого подписка может быть бездействовать без запроса на получение событий от клиента.
ms.openlocfilehash: 6f3228cd480bf0eaf259c4f321bc74d0845b9bba
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459898"
---
# <a name="timeout"></a>Timeout

Элемент **timeout** представляет продолжительность в минутах, в течение которого подписка может быть бездействовать без запроса на получение событий от клиента. 
  
```xml
<Timeout/>
```

 **int**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[пуллсубскриптионрекуест](pullsubscriptionrequest.md) <br/> |Представляет подписку на подписку на уведомления о событиях по запросу.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

При использовании этого элемента необходимо указать текстовое значение, представляющее целое число. Возможные значения для этого элемента — от 1 до 1440 включительно. Этот элемент обязательный.
  
## <a name="remarks"></a>Примечания

Таймер времени ожидания для подписки сбрасывается из-за успешных запросов на получение событий.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

