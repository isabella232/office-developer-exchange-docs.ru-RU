---
title: деливермитингрекуестс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: Элемент Деливермитингрекуестс определяет способ обработки приглашений на собрание между представителем и участником. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 3998443613437bca2267678f7bc2c5584b779135
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463680"
---
# <a name="delivermeetingrequests"></a>деливермитингрекуестс

Элемент **деливермитингрекуестс** определяет способ обработки приглашений на собрание между представителем и участником. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 **деливермитингрекуестстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AddDelegate](adddelegate.md) <br/> |Определяет запрос на добавление делегатов в почтовый ящик. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Определяет запрос на обновление делегатов в почтовом ящике. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[жетделегатереспонсе](getdelegateresponse.md) <br/> |Содержит состояние и результат запроса делегата. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **деливермитингрекуестс** . 
  
**Значения элементов Деливермитингрекуестс**

|**Значение**|**Описание**|
|:-----|:-----|
|делегатесонли  <br/> |Приглашения на собрания пересылаются представителю и перемещаются в папку "Удаленные" в почтовом ящике субъекта.  <br/> |
|делегатесандме  <br/> |Приглашения на собрания пересылаются представителю и сохраняются в папке "Входящие" в почтовом ящике субъекта.  <br/> |
|делегатесандсендинформатионтоме  <br/> |Приглашения на собрания пересылаются представителю и хранятся в папке "Входящие" в почтовом ящике участника, но кнопки "принять", "под вопросом" и "отклонить" не отображаются в области чтения Microsoft Office Outlook.  <br/> |
|Не пересылать  <br/> |Приглашения на собрания не пересылаются представителю.  <br/> |
   
## <a name="remarks"></a>Примечания

Параметр **деливермитингрекуестс** влияет на всех делегатов в почтовом ящике участника. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция AddDelegate](adddelegate-operation.md)  
- [Операция UpdateDelegate](updatedelegate-operation.md)  
- [Операция GetDelegate](getdelegate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Добавление делегатов](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

