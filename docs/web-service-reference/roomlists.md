---
title: румлистс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RoomLists
api_type:
- schema
ms.assetid: 2b190823-b11e-4635-97e4-3aba5865fd05
description: Элемент Румлистс — это список из одного или нескольких адресов, которые представляют список комнат для собраний.
ms.openlocfilehash: eb03c34aeb5d80c4a9c6c92471e4094c63f04c87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835252"
---
# <a name="roomlists"></a>румлистс

Элемент **румлистс** — это список из одного или нескольких адресов, которые представляют список комнат для собраний. 
  
[жетрумлистсреспонсе](getroomlistsresponse.md)
  
[румлистс](roomlists.md)
  
```xml
<RoomLists>   <Address/></RoomLists>
```

 **аррайофемаиладдрессестипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Адрес (EmailAddressType)](address-emailaddresstype.md) <br/> |Определяет адрес электронной почты и отображаемое имя, представляющее список помещений. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетрумлистсреспонсе](getroomlistsresponse.md) <br/> |Содержит состояние и результат запроса [операции GetRoomLists](getroomlists-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetRoomLists](getroomlists-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

