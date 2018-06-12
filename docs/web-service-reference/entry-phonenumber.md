---
title: Запись (PhoneNumber)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Entry
api_type:
- schema
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: Элемент представляет номер телефона контакта.
ms.openlocfilehash: 3953488fb0b57fcf01c2fb99039478bbe03c7f5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762375"
---
# <a name="entry-phonenumber"></a>Запись (PhoneNumber)

**Элемент** представляет номер телефона контакта. 
  
```xml
<Entry Key=""/>
```

 **PhoneNumberDictionaryEntryType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Key** <br/> | Номер телефона. Атрибут Key имеет тип **PhoneNumberKeyType**.<br/><br/> Ниже приведены возможные значения этого атрибута.<br/><br/>-AssistantPhone  <br/>-Рабочий  <br/>-BusinessPhone  <br/>-BusinessPhone2  <br/>-Обратного вызова  <br/>-Автомобильный телефон  <br/>-CompanyMainPhone  <br/>-Домашний факс  <br/>-HomePhone  <br/>-HomePhone2  <br/>-Isdn  <br/>-MobilePhone  <br/>-OtherFax  <br/>-OtherTelephone  <br/>-Пейджера  <br/>-PrimaryPhone  <br/>-RadioPhone  <br/>-Телекса  <br/>-TtyTddPhone  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PhoneNumbers](phonenumbers.md) <br/> |Представляет коллекцию телефонных номеров контакта.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее номер телефона является обязательным, если данный элемент используется.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание контактов (веб-служб Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [Обновление контактов](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Удаление контактов](http://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

