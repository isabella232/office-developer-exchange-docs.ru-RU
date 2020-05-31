---
title: маилбокссмтпаддресс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailboxSmtpAddress
api_type:
- schema
ms.assetid: de7c9035-ebbc-4473-ac14-3b22ce62768c
description: Элемент Маилбокссмтпаддресс представляет SMTP-адрес пользователя, чьи правила папки "Входящие" извлекаются или обновляются; или Дата окончания срока действия пароля, который необходимо получить.
ms.openlocfilehash: 60b2c018f2a05e9630e92e28de1054a421b41e52
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834303"
---
# <a name="mailboxsmtpaddress"></a>маилбокссмтпаддресс

Элемент **маилбокссмтпаддресс** представляет SMTP-адрес пользователя, чьи правила папки "Входящие" извлекаются или обновляются; или Дата окончания срока действия пароля, который необходимо получить. 
  
```XML
<MailboxSmtpAddress/>
```

**строка**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetInboxRules](getinboxrules.md) <br/> |Определяет запрос на получение правил для папки "Входящие" для почтового ящика в хранилище сервера.  <br/> |
|[GetPasswordExpirationDate](getpasswordexpirationdate.md) <br/> |Определяет запрос на получение даты истечения срока действия пароля учетной записи электронной почты.  <br/> |
|[UpdateInboxRules](updateinboxrules.md) <br/> |Определяет запрос на обновление правил папки "Входящие" в почтовом ящике в хранилище сервера.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Элемент **маилбокссмтпаддресс** является необязательным элементом. Если элемент **маилбокссмтпаддресс** опущен, используется адрес пользователя, выполнившего вход в систему. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetInboxRules](getinboxrules-operation.md)
- [Операция GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Операция UpdateInboxRules](updateinboxrules-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

