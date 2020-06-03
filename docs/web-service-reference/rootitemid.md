---
title: рутитемид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootItemId
api_type:
- schema
ms.assetid: f613c705-17ce-48ce-aa64-4dc2cea25e31
description: Элемент Рутитемид определяет корневой элемент удаленного вложения.
ms.openlocfilehash: d8badd465fd5a93e1a6354d55ac5c4b080897152
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457097"
---
# <a name="rootitemid"></a>рутитемид

Элемент **рутитемид** определяет корневой элемент удаленного вложения. 
  
[делетеаттачментреспонсе](deleteattachmentresponse.md)
  
[респонсемессажес](responsemessages.md)
  
[делетеаттачментреспонсемессаже](deleteattachmentresponsemessage.md)
  
[рутитемид](rootitemid.md)
  
```xml
<RootItemId RootItemId="" RootItemChangeKey="" />
```

 **рутитемидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**рутитемид** <br/> |Определяет корневой элемент удаленного вложения.  <br/> |
|**рутитемчанжекэй** <br/> |Определяет новый ключ изменения корневого элемента удаленного вложения.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[делетеаттачментреспонсемессаже](deleteattachmentresponsemessage.md) <br/> |Содержит состояние и результат запроса DeleteAttachment.  <br/> |
   
## <a name="remarks"></a>Примечания

Элемент **рутитемид** используется только в ответах DeleteAttachment. Это определяет идентификатор корневого элемента и, что более важно, новый ключ изменения для родительского элемента. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[DeleteAttachment](deleteattachment.md)
  
[Операция DeleteAttachment](deleteattachment-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

