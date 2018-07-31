---
title: CompleteName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: Элемент CompleteName представляет полное имя контакта.
ms.openlocfilehash: bca6f7e0eb915841673d00b5485da2f0f9794e80
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354262"
---
# <a name="completename"></a>CompleteName

Элемент **CompleteName** представляет полное имя контакта. 
  
```xml
<CompleteName>
   <Title/>
   <FirstName/>
   <MiddleName/>
   <LastName/>
   <Suffix/>
   <Initials/>
   <FullName/>
   <Nickname/>
   <YomiFirstName/>
   <YomiLastName/>
</CompleteName>
```

 **CompleteNameType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Название](title.md) <br/> |Представляет должность контакта.  <br/> |
|[FirstName](firstname.md) <br/> |Представляет имя контакта.  <br/> |
|[MiddleName](middlename.md) <br/> |Представляет отчество контакта.  <br/> |
|[LastName](lastname.md) <br/> |Представляет фамилию контакта.  <br/> |
|[Suffix](suffix.md) <br/> |Представляет суффикса имени контакта.  <br/> |
|[Initials](initials.md) <br/> |Представляет отчество контакта.  <br/> |
|[FullName](fullname.md) <br/> |Представляет полное имя контакта.  <br/> |
|[Nickname](nickname.md) <br/> |Представляет псевдоним контакта.  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |Представляет имя, используемое в Японии для поиска или фонетическое написание имя японского языка.  <br/> |
|[YomiLastName](yomilastname.md) <br/> |Представляет имя, используемое в Японии для поиска или фонетическое орфографию японского Фамилия.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
   
## <a name="remarks"></a>Замечания

Свойство CompleteName является частью фигуры [по умолчанию](https://docs.microsoft.com/en-us/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) . В первоначальной версии Microsoft Exchange Server 2007 свойство CompleteName возвращается [операции GetItem](getitem-operation.md), но не [FindItem операции](finditem-operation.md). Начиная с Exchange Server 2007 с пакетом обновления 1 (SP1), [операция FindItem](finditem-operation.md) также возвращает свойство CompleteName формы [по умолчанию](https://docs.microsoft.com/en-us/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) . Это изменение не влияет на схеме. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [CompleteNameType](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание контактов (веб-служб Exchange)](http://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

