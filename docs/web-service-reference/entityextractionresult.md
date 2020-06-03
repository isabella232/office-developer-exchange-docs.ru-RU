---
title: ентитекстрактионресулт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: Элемент Ентитекстрактионресулт указывает свойство Ентитекстрактионресулт элемента.
ms.openlocfilehash: f2f069717a5862adff3349090c35f95499d135f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456957"
---
# <a name="entityextractionresult"></a>ентитекстрактионресулт

Элемент **ентитекстрактионресулт** указывает свойство **ентитекстрактионресулт** элемента. 
  
```XML
<EntityExtractionResult>
    <Addresses/>
    <MeetingSuggestions/>
    <TaskSuggestions/>
    <EmailAddresses/>
    <Contacts/>
    <Urls/>
    <PhoneNumbers/>
</EntityExtractionResult>
```

 **ентитекстрактионресулттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Адреса (Аррайофаддрессентитиестипе)](addresses-arrayofaddressentitiestype.md) <br/> |Указывает массив элементов **аддрессентити** .  <br/> |
|[MeetingSuggestions](meetingsuggestions.md) <br/> |Указывает массив элементов **Свойства meetingsuggestion** .  <br/> |
|[TaskSuggestions](tasksuggestions.md) <br/> |Указывает массив элементов **TaskSuggestion** .  <br/> |
|[EmailAddresses (Аррайофемаиладдрессентитиестипе)](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |Указывает массив сущностей адресов электронной почты.  <br/> |
|[Contacts (Аррайофконтактстипе)](contacts-arrayofcontactstype.md) <br/> |Указывает массив контактов.  <br/> |
|[URL-адреса (Аррайофурлентитиестипе)](urls-arrayofurlentitiestype.md) <br/> |Указывает массив URL-адресов.  <br/> |
|[PhoneNumbers (Аррайоффонинтитиестипе)](phonenumbers-arrayofphoneentitiestype.md) <br/> |Указывает массив телефонных номеров.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Ресурс](item.md) <br/> |Представляет общий элемент в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

