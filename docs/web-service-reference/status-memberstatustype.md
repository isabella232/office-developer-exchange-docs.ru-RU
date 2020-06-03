---
title: Состояние (Мемберстатустипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: Элемент Status предоставляет сведения о состоянии члена списка рассылки на сервере.
ms.openlocfilehash: bfa0c349d6af51c1b2238c9749d2656541d31906
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465466"
---
# <a name="status-memberstatustype"></a>Состояние (Мемберстатустипе)

Элемент **Status** предоставляет сведения о состоянии члена списка рассылки на сервере. 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 **мемберстатустипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент](member-ex15websvcsotherref.md) <br/> |Представляет члена списка рассылки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **Status** . 
  
**Значения элементов Status**

|**Значение**|**Описание**|
|:-----|:-----|
|Нераспознанный  <br/> |Сведения об участниках являются недопустимыми или неопознанными.  <br/> |
|Normal  <br/> |Сведения об участниках в списке рассылки синхронизируются с объектом, на который указывает ссылка.  <br/> |
|Понижения  <br/> |Объект, на который указывает ссылка, недоступен.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

