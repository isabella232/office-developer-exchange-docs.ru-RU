---
title: Entry (PhoneNumber)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Entry
api_type:
- schema
ms.assetid: e3d0a4d5-8af8-4607-aa2e-ef3111b63b55
description: Элемент Entry представляет телефонный номер для контакта.
ms.openlocfilehash: f9f8f08c8d167614bfc5772d6d74ebee77234c70
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545246"
---
# <a name="entry-phonenumber"></a>Entry (PhoneNumber)

Элемент **Entry** представляет телефонный номер для контакта. 
  
```xml
<Entry Key=""/>
```

 **PhoneNumberDictionaryEntryType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Ключ** <br/> | Определяет номер телефона. Атрибут Key — тип **PhoneNumberKeyType.**<br/><br/> Возможные значения для этого атрибута:<br/><br/>- AssistantPhone  <br/>- BusinessFax  <br/>- BusinessPhone  <br/>- BusinessPhone2  <br/>- Callback  <br/>- CarPhone  <br/>- CompanyMainPhone  <br/>- HomeFax  <br/>- HomePhone  <br/>- HomePhone2  <br/>- Isdn  <br/>- MobilePhone  <br/>- OtherFax  <br/>- OtherTelephone  <br/>- Pager  <br/>- PrimaryPhone  <br/>- RadioPhone  <br/>- Telex  <br/>- TtyTddPhone  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PhoneNumbers](phonenumbers.md) <br/> |Представляет коллекцию номеров телефонов для контакта.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если используется этот элемент, требуется текстовое значение, представляю которое представляет телефонный номер.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание контактов (Exchange веб-служб)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [Обновление контактов](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Удаление контактов](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

