---
title: Граупингинформатион (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d8a007f-d79c-43c8-90e3-2c6d883f3a7c
description: Элемент Граупингинформатион содержит значение, используемое для группировки почтового ящика пользователя при подписке на уведомления через несколько почтовых ящиков.
ms.openlocfilehash: 7cab5d68f7dd5ec1f6caded5b9da6cfee03f3a67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530080"
---
# <a name="groupinginformation-pox"></a>Граупингинформатион (POX)

Элемент **граупингинформатион** содержит значение, используемое для группировки почтового ящика [пользователя при](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx) подписке на уведомления через несколько почтовых ящиков. 
  
[Служба автообнаружения (POX)](autodiscover-pox.md)
  
[Ответ (POX)](response-pox.md)
  
[Учетная запись (POX)](account-pox.md)
  
[Протокол (POX)](protocol-pox.md)
  
[Граупингинформатион (POX)](groupinginformation-pox.md)
  
```XML
<GroupingInformation/>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Протокол (POX)](protocol-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу Exchange Server.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение сравнивается со значением элемента **граупингинформатион** для других почтовых ящиков. Почтовые ящики, имеющие одинаковое значение и использующие одну конечную точку веб-служб Exchange (EWS), можно объединять для поддержания сходства. Более подробную информацию можно узнать [в статье поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx).
  
## <a name="remarks"></a>Примечания

Элемент **граупингинформатион** применяется только к элементам **протокола** , имеющим дочерний элемент [Type (POX)](type-pox.md) со значением "expr". 
  
## <a name="see-also"></a>См. также

- [XML-элементы автообнаружения POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)
- [Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange](https://msdn.microsoft.com/library/1bda4094-88c3-4f61-9219-6ee70f6e81cf%28Office.15%29.aspx)

