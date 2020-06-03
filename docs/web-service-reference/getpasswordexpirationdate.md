---
title: GetPasswordExpirationDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f4f958ed-9cf4-4ebf-9b01-e2df9a7cbd63
description: Элемент GetPasswordExpirationDate определяет запрос на получение даты истечения срока действия пароля для учетной записи электронной почты. Этот элемент является базовым элементом для операции GetPasswordExpirationDate.
ms.openlocfilehash: ececbf51f71c7d87705d727229fce2314d922efb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456495"
---
# <a name="getpasswordexpirationdate"></a>GetPasswordExpirationDate

Элемент **GetPasswordExpirationDate** определяет запрос на получение даты истечения срока действия пароля для учетной записи электронной почты. Этот элемент является базовым элементом для операции [GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) . 
  
```XML
<GetPasswordExpirationDate>
    <MailboxSmtpAddress/>
</GetPasswordExpirationDate>
```

 **жетпассвордекспиратиондатетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[маилбокссмтпаддресс](mailboxsmtpaddress.md) <br/> |Представляет электронный адрес учетной записи электронной почты, для которой возвращается дата истечения срока действия пароля.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

