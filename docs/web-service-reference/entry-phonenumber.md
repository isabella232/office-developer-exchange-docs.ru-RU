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
description: Элемент entry представляет телефонный номер контакта.
ms.openlocfilehash: 62f7091bb750dc7ca74b1e5637a437e2cdad4f1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459639"
---
# <a name="entry-phonenumber"></a>Запись (PhoneNumber)

Элемент **entry** представляет телефонный номер контакта. 
  
```xml
<Entry Key=""/>
```

 **фоненумбердиктионарентритипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Key** <br/> | Указывает номер телефона. Ключевой атрибут относится к типу **фоненумберкэйтипе**.<br/><br/> Ниже приведены возможные значения для этого атрибута.<br/><br/>— Ассистантфоне  <br/>— Бусинессфакс  <br/>— Бусинессфоне  <br/>- BusinessPhone2  <br/>Ответный вызов  <br/>— Карфоне  <br/>— Компанимаинфоне  <br/>— Хомефакс  <br/>— HomePhone  <br/>- HomePhone2  <br/>– ISDN  <br/>— MobilePhone  <br/>— OtherFax  <br/>— OtherTelephone  <br/>— Пейджер  <br/>— Примарифоне  <br/>— Радиофоне  <br/>— Телекса  <br/>— Ттитддфоне  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PhoneNumbers](phonenumbers.md) <br/> |Представляет коллекцию телефонных номеров контакта.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

При использовании этого элемента необходимо указать текстовое значение, представляющее номер телефона.
  
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
- [Создание контактов (веб-службы Exchange)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx) 
- [Обновление контактов](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)  
- [Удаление контактов](https://msdn.microsoft.com/library/fcc3dc84-cd3e-455e-a1a7-ae6921c9b588%28Office.15%29.aspx)

