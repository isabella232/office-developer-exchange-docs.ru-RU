---
title: Данные
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
ms.assetid: f875e6c2-be18-439a-a7b1-bb49a149b538
description: Элемент Data содержит зашифрованные данные, представляющие общие данные.
ms.openlocfilehash: cd13d68afcd0f40486865887676d2b5669c276f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529219"
---
# <a name="data"></a>Данные

Элемент **Data** содержит зашифрованные данные, представляющие общие данные. 
  
- [енкриптедшаредфолдердата](encryptedsharedfolderdata.md)  
- [Data](data.md)
  
```xml
<Data/>
```

**енкриптеддатаконтаинертипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[енкриптедшаредфолдердата](encryptedsharedfolderdata.md) <br/> |Содержит зашифрованные данные, которые клиент может использовать для авторизации общего доступа к данным календаря или контактных данных с другими клиентами.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetSharingMetadata](getsharingmetadata-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

