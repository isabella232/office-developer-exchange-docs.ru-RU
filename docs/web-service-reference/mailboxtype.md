---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: Элемент MailboxType представляет тип почтового ящика, представленного адресом электронной почты.
ms.openlocfilehash: d7232377951e8d9c8f191ac856058bc28467cadd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834305"
---
# <a name="mailboxtype"></a>MailboxType

Элемент **MailboxType** представляет тип почтового ящика, представленного адресом электронной почты. 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

**маилбокстипетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет полностью разрешенный адрес электронной почты.  <br/> |
|[RoomList](roomlist.md) <br/> |Определяет список комнат для собраний.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **MailboxType** . 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Почтовый ящик  <br/> |Представляет объект Active Directory с включенной поддержкой почты.  <br/> |
|PublicDL  <br/> |Представляет общедоступный список рассылки.  <br/> |
|PrivateDL  <br/> |Представляет частный список рассылки в почтовом ящике пользователя.  <br/> |
|Контакт  <br/> |Представляет контакт в почтовом ящике пользователя.  <br/> |
|PublicFolder  <br/> |Представляет общедоступную папку.  <br/> |
|Unknown  <br/> |Представляет неизвестный тип почтового ящика.  <br/> |
|OneOff  <br/> |Представляет одноразовый участник личного списка рассылки.  <br/> |
|граупмаилбокс  <br/> |Представляет группу почтового ящика.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

