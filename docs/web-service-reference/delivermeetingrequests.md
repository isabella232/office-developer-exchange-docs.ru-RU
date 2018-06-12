---
title: DeliverMeetingRequests
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
description: Элемент DeliverMeetingRequests определяет порядок обработки приглашений на собрания между делегата и участника. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 803bd2da72bdb21b507a59cc11635a40d4431acf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762063"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

Элемент **DeliverMeetingRequests** определяет порядок обработки приглашений на собрания между делегата и участника. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```XML
<DeliverMeetingRequests>DelegatesOnly or DelegatesAndMe or DelegatesAndSendInformationToMe or NoForward</DeliverMeetingRequests>
```

 **DeliverMeetingRequestsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Метод AddDelegate](adddelegate.md) <br/> |Определяет запрос на Добавление делегатов к почтовому ящику. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Определяет запрос на обновление делегаты в почтовом ящике. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Содержит состояние и результат запроса GetDelegate. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **DeliverMeetingRequests** . 
  
**Значения элементов DeliverMeetingRequests**

|**Значение**|**Описание**|
|:-----|:-----|
|DelegatesOnly  <br/> |Приглашения на собрания пересылку делегата и перемещено в папку «Удаленные» в почтовом ящике участника.  <br/> |
|DelegatesAndMe  <br/> |Приглашения на собрания, пересылаются на делегат и оставаться в папке "Входящие" в почтовом ящике участника.  <br/> |
|DelegatesAndSendInformationToMe  <br/> |Приглашения на собрания, пересылаются на делегат и оставаться в папке "Входящие" в почтовом ящике участника, но кнопки принять, под вопросом и отклонить не отображаются в области чтения Microsoft Office Outlook.  <br/> |
|NoForward  <br/> |Приглашения на собрания не перенаправляются на делегат.  <br/> |
   
## <a name="remarks"></a>Замечания

Параметр **DeliverMeetingRequests** влияет на все делегаты в почтовом ящике участника. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция AddDelegate](adddelegate-operation.md)  
- [Операция UpdateDelegate](updatedelegate-operation.md)  
- [Операция GetDelegate](getdelegate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Добавление делегатов](http://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

