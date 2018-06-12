---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: Элемент GetPasswordExpirationDate определяет запрос на получение срок действия пароля для учетной записи электронной почты. Этот элемент является базовый элемент для операции GetPasswordExpirationDate операции.
ms.openlocfilehash: a9e0955566372f7b99c48c56e62ce2c5025f9f95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762877"
---
# <a name="getpasswordexpirationdate"></a>GetPasswordExpirationDate

Элемент **GetPasswordExpirationDate** определяет запрос на получение срок действия пароля для учетной записи электронной почты. Этот элемент является базовый элемент для операции [GetPasswordExpirationDate операции](getpasswordexpirationdate-operation.md) . 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 **GetPasswordExpirationDateType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[MailboxSmtpAddress](mailboxsmtpaddress.md) <br/> |Представляет собой адрес электронной почты учетной записи электронной почты, для которого срок действия пароля — это должно быть возвращено.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

