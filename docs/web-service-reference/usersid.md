---
title: О.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UserSid
api_type:
- schema
ms.assetid: f8a0dcd9-8564-4e35-b307-c5d2761b48d8
description: Элемент "код возврата" представляет форму SDDL идентификатора безопасности пользователя в заголовке SOAP сериализованного контекста безопасности. Сериализация маркеров не поддерживается.
ms.openlocfilehash: b8ee51b1998546fc4ab14bd3666192ae63c8dba8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462019"
---
# <a name="usersid"></a>О.

Элемент **"код возврата" представляет** форму SDDL идентификатора безопасности пользователя в заголовке SOAP сериализованного контекста безопасности. Сериализация маркеров не поддерживается. 
  
```xml
<UserSid/>
```

 **String**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[сериализедсекуритиконтекст](serializedsecuritycontext.md) <br/> |Используется в заголовке SOAP для сериализации маркеров при проверке подлинности "сервер — сервер".  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет идентификатор безопасности пользователя.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

