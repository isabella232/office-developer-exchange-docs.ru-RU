---
title: Data (base64Binary)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Data
api_type:
- schema
ms.assetid: 26d8c2d0-bed2-4aed-b381-20e2ace6892f
description: Элемент Data содержит данные одного экспортированного элемента или элемента для отправки в почтовый ящик.
ms.openlocfilehash: 43ee16ca7caf634756ca00a88715d9834adad92b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526972"
---
# <a name="data-base64binary"></a>Data (base64Binary)

Элемент **Data** содержит данные одного экспортированного элемента или элемента для отправки в почтовый ящик. 
  
```XML
<Data/>
```

**xs: base64Binary**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[експортитемсреспонсемессаже](exportitemsresponsemessage.md) <br/> |Содержит состояние и результаты запроса на экспорт одного элемента почтового ящика.  <br/> |
|[Элемент (Уплоадитемтипе)](item-uploaditemtype.md) <br/> |Представляет отдельный элемент для отправки в почтовый ящик.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Элемент **Data** содержит имена и значения свойств для экспортированного элемента или элемента, которые будут отправлены в почтовый ящик. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ExportItems](exportitems-operation.md)
- [Операция UploadItems](uploaditems-operation.md)

