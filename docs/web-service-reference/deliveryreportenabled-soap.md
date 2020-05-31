---
title: Деливерирепортенаблед (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: Элемент Деливерирепортенаблед представляет флаг Деливерирепортенаблед (). Элемент Деливерирепортенаблед предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 089256a5f75ad92a4f11c5aaf3d175382eeee456
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762065"
---
# <a name="deliveryreportenabled-soap"></a>Деливерирепортенаблед (SOAP)

Элемент **деливерирепортенаблед** представляет флаг **деливерирепортенаблед ()** . Элемент **деливерирепортенаблед** предназначен только для внутреннего использования. Этот элемент не используется клиентами. 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Организатионрелатионшипсеттингс (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Представляет список отношений Организации для одной организации.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение true для элемента Деливерирепортенаблед указывает на то, что можно использовать отчеты о доставке от пользователей в Организации. Значение false указывает, что отчеты о доставке должны подавляться.
  
## <a name="remarks"></a>Примечания

Используйте этот элемент, чтобы разрешить или запретить отправку отчетов о доставке с сервера.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция Жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

