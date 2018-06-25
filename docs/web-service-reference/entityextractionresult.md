---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: Элемент EntityExtractionResult указывает свойство EntityExtractionResult элемента.
ms.openlocfilehash: ef99629beb95f1e1123569fa99e3f495c1b56e95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762371"
---
# <a name="entityextractionresult"></a>EntityExtractionResult

Элемент **EntityExtractionResult** указывает свойство **EntityExtractionResult** элемента. 
  
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

 **EntityExtractionResultType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Адреса (ArrayOfAddressEntitiesType)](addresses-arrayofaddressentitiestype.md) <br/> |Указывает массив элементов **AddressEntity** .  <br/> |
|[MeetingSuggestions](meetingsuggestions.md) <br/> |Указывает массив элементов **MeetingSuggestion** .  <br/> |
|[TaskSuggestions](tasksuggestions.md) <br/> |Указывает массив элементов **TaskSuggestion** .  <br/> |
|[EmailAddresses (ArrayOfEmailAddressEntitiesType)](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |Указывает массив сущностей, адрес электронной почты.  <br/> |
|[Контакты (ArrayOfContactsType)](contacts-arrayofcontactstype.md) <br/> |Указывает массив контакты.  <br/> |
|[URL-адреса (ArrayOfUrlEntitiesType)](urls-arrayofurlentitiestype.md) <br/> |Указывает массив URL-адресов.  <br/> |
|[PhoneNumbers (ArrayOfPhoneEntitiesType)](phonenumbers-arrayofphoneentitiestype.md) <br/> |Указывает массив телефонных номеров.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент](item.md) <br/> |Представляет универсальный элемент в хранилище Exchange.  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

