---
title: RecipientAddress
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecipientAddress
api_type:
- schema
ms.assetid: 9ae6351a-2c60-4715-a489-5681a13641f9
description: Элемент Получательимеет адрес представляет почтовый ящик получателя.
ms.openlocfilehash: f4b6edd034dd91471e6496f6b0cca65bd3ffb69a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465851"
---
# <a name="recipientaddress"></a>RecipientAddress

Элемент **получательимеет адрес** представляет почтовый ящик получателя. 
  
```xml
<RecipientAddress>
   <Name/>
   <EmailAddress/>
   <RoutingType/>
   <MailboxType/>
   <ItemId/>
</RecipientAddress>
```

 **EmailAddressType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Имя (EmailAddressType)](name-emailaddresstype.md) <br/> |Представляет имя пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md) <br/> |Определяет SMTP-адрес пользователя почтового ящика. Этот элемент является необязательным.  <br/> |
|[Раутингтипе (EmailAddress)](routingtype-emailaddress.md) <br/> |Представляет протокол маршрутизации для получателя. По умолчанию используется протокол SMTP. Этот элемент является необязательным.  <br/> |
|[MailboxType](mailboxtype.md) <br/> |Представляет тип почтового ящика, представленного адресом электронной почты.  <br/> |
|[Идентификатор](itemid.md) <br/> |Определяет идентификатор контакта или частный список рассылки для получателей из папки "Контакты" пользователя. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Подсказки](mailtips.md) <br/> |Представляет значения для различных типов советов по использованию электронной почты.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

