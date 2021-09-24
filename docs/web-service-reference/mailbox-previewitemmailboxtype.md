---
title: Mailbox (PreviewItemMailboxType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: e898d737-b6e4-4403-9c2c-aec52a48a83d
description: Элемент почтовых ящиков содержит идентификатор почтового ящика и основной адрес простого протокола передачи почты пользователя (SMTP).
ms.openlocfilehash: 1a2dcc08d3e1595aede21e6982b36a60e6efafb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514300"
---
# <a name="mailbox-previewitemmailboxtype"></a>Mailbox (PreviewItemMailboxType)

Элемент **почтовых ящиков** содержит идентификатор почтового ящика и основной адрес простого протокола передачи почты пользователя (SMTP). 
  
```XML
<Mailbox>
   <MailboxId/>
   <PrimarySmtpAddress/>
</Mailbox>
```

**PreviewItemMailboxType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Почтовый ящикId](mailboxid.md)  |  [PrimarySmtpAddress (string)](primarysmtpaddress-string.md)
  
### <a name="parent-elements"></a>Родительские элементы

[SearchPreviewItem](searchpreviewitem.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   

