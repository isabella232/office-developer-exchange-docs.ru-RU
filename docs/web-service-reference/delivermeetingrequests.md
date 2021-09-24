---
title: DeliverMeetingRequests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeliverMeetingRequests
api_type:
- schema
ms.assetid: 04b999af-0b27-4e6d-a8b1-400955a1afaa
description: Элемент DeliverMeetingRequests определяет, как обрабатываются запросы на собрания между делегатом и директором. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 8e61af87337cb1fc8936b4de7753fca2d6c1161e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519830"
---
# <a name="delivermeetingrequests"></a>DeliverMeetingRequests

Элемент **DeliverMeetingRequests** определяет, как обрабатываются запросы на собрания между делегатом и директором. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
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
|[AddDelegate](adddelegate.md) <br/> |Определяет запрос на добавление делегатов в почтовый ящик. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UpdateDelegate](updatedelegate.md) <br/> |Определяет запрос на обновление делегатов в почтовом ящике. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[GetDelegateResponse](getdelegateresponse.md) <br/> |Содержит состояние и результат запроса GetDelegate. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **DeliverMeetingRequests.** 
  
**Значения элементов DeliverMeetingRequests**

|**Значение**|**Описание**|
|:-----|:-----|
|DelegatesOnly  <br/> |Запросы на собрание перенакладыются делегату и перемещаются в папку "Удаленные элементы" в почтовом ящике директора.  <br/> |
|DelegatesAndMe  <br/> |Запросы на собрание перенакладыются делегату и остаются в папке "Входящие" в почтовом ящике директора.  <br/> |
|DelegatesAndSendInformationToMe  <br/> |Запросы на собрание пересылаются делегату и остаются в папке "Входящие" в почтовом ящике директора, но кнопки Accept, Tentative и Decline не отображаются в области Microsoft Office Outlook чтения.  <br/> |
|NoForward  <br/> |Запросы на собрание не переадад- ются делегату.  <br/> |
   
## <a name="remarks"></a>Заметки

Параметр **DeliverMeetingRequests затрагивает** всех делегатов в почтовом ящике директора. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция AddDelegate](adddelegate-operation.md)  
- [Операция UpdateDelegate](updatedelegate-operation.md)  
- [Операция GetDelegate](getdelegate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Добавление делегатов](https://msdn.microsoft.com/library/3a744150-66a3-4a13-9433-793603ba5038%28Office.15%29.aspx)

