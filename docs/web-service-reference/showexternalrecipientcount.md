---
title: ShowExternalRecipientCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ShowExternalRecipientCount
api_type:
- schema
ms.assetid: db28dbcb-d051-4e5c-a9c2-4b8d5149b4e1
description: Элемент ShowExternalRecipientCount указывает, должны ли пользователи операции GetMailTips показывать советы по почте, которые указывают количество внешних получателей, к которым адресовано сообщение.
ms.openlocfilehash: 30615dcb1091dff01cf13679e3e1ed68c8b25af9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539102"
---
# <a name="showexternalrecipientcount"></a>ShowExternalRecipientCount

Элемент **ShowExternalRecipientCount** указывает, должны ли пользователи операции [GetMailTips](getmailtips-operation.md) показывать советы по почте, которые указывают количество внешних получателей, к которым адресовано сообщение. 
  
```XML
<ShowExternalRecipientCount>true | false</ShowExternalRecipientCount>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MailTipsConfiguration (MailTipsServiceConfiguration)](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |Содержит сведения о конфигурации службы для службы советов почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Значение текста этого элемента  верно, если пользователи операции [GetMailTips](getmailtips-operation.md) должны показывать советы по почте, указывающие количество внешних получателей, к которым адресовано сообщение. Значение является **ложным,** если пользователям операции [GetMailTips](getmailtips-operation.md) не нужно показывать советы по почте, которые указывают количество внешних получателей, к которым адресовано сообщение. 
  
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



[Операция GetMailTips](getmailtips-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

