---
title: MailboxType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxType
api_type:
- schema
ms.assetid: 696e5fdb-d8c5-40f0-9e79-885eae65dfa4
description: Элемент MailboxType представляет тип почтового ящика, который представлен адресом электронной почты.
ms.openlocfilehash: f7605bf0e90851352efaaabed09e878be0925581
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524051"
---
# <a name="mailboxtype"></a>MailboxType

Элемент **MailboxType** представляет тип почтового ящика, который представлен адресом электронной почты. 
  
```XML
<MailboxType>Mailbox | PublicDL | PrivateDL | Contact | PublicFolder | Unknown | OneOff | GroupMailbox</MailboxType>
```

**MailboxTypeType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет полностью разрешенный адрес электронной почты.  <br/> |
|[RoomList](roomlist.md) <br/> |Определяет список комнат собраний.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **MailboxType.** 
  
|**Значение**|**Описание**|
|:-----|:-----|
|Почтовый ящик  <br/> |Представляет объект Active Directory с поддержкой почты.  <br/> |
|PublicDL  <br/> |Представляет общедоступный список рассылки.  <br/> |
|PrivateDL  <br/> |Представляет частный список рассылки в почтовом ящике пользователя.  <br/> |
|Контакт  <br/> |Представляет контакт в почтовом ящике пользователя.  <br/> |
|PublicFolder  <br/> |Представляет общедоступные папки.  <br/> |
|Unknown  <br/> |Представляет неизвестный тип почтового ящика.  <br/> |
|OneOff  <br/> |Представляет разовую часть личного списка рассылки.  <br/> |
|GroupMailbox  <br/> |Представляет почтовый ящик группы.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

