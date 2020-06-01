---
title: Получатели (Аррайофсмтпаддресстипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recipients
api_type:
- schema
ms.assetid: cf68417d-85cf-49e0-857a-f987d3675344
description: Элемент Recipients указывает массив получателей сообщения.
ms.openlocfilehash: 4c2478a81836c2e52baad9c928d112108679b837
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465508"
---
# <a name="recipients-arrayofsmtpaddresstype"></a>Получатели (Аррайофсмтпаддресстипе)

Элемент **Recipients** указывает массив получателей сообщения. 
  
```xml
<Recipients>   <SmtpAddress/></Recipients>
```

 **аррайофсмтпаддресстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SmtpAddress](smtpaddress.md) <br/> |Представляет адрес получателя протокола SMTP для запроса на общий доступ к календарю или контакту.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetSharingMetadata](getsharingmetadata.md) <br/> |Определяет запрос на получение непрозрачного маркера проверки подлинности, который определяет приглашение к совместному использованию.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, на котором размещены веб-службы Exchange компьютера, на котором установлен сервер Microsoft Exchange, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetSharingMetadata](getsharingmetadata-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

