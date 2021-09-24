---
title: MailboxSmtpAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: Элемент MailboxSmtpAddress представляет SMTP-адрес пользователя, правила которого должны быть извлечены или обновлены; или срок действия пароля, который должен быть извлечен.
ms.openlocfilehash: 86a39c416b9674e1f48f0a75508c003ad9d620f1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511133"
---
# <a name="mailboxsmtpaddress"></a>MailboxSmtpAddress

Элемент **MailboxSmtpAddress** представляет SMTP-адрес пользователя, правила которого должны быть извлечены или обновлены; или срок действия пароля, который должен быть извлечен. 
  
```XML
<MailboxSmtpAddress/>
```

**строка**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetInboxRules](getinboxrules.md) <br/> |Определяет запрос для получения правил входящие в почтовый ящик в серверном магазине.  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |Определяет запрос для получения даты истечения срока действия пароля учетной записи электронной почты.  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |Определяет запрос на обновление правил "Входящие" в почтовом ящике в серверном магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Элемент **MailboxSmtpAddress** является необязательным элементом. Если **элемент MailboxSmtpAddress** опущен, используется адрес зарегистрированного пользователя. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetInboxRules](getinboxrules-operation.md)
- [Операция GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Операция UpdateInboxRules](updateinboxrules-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

