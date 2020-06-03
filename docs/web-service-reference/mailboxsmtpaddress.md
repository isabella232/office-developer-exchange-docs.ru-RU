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
ms.openlocfilehash: 613e8098210257280bec47f2b22a2d29d04fa07c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530546"
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

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
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
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetInboxRules](getinboxrules-operation.md)
- [Операция GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Операция UpdateInboxRules](updateinboxrules-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

