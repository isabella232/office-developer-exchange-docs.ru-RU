---
title: CompleteName
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CompleteName
api_type:
- schema
ms.assetid: 22d30d1f-a84d-48bb-ad8f-ce13f8e76604
description: Элемент CompleteName представляет полное имя контакта.
ms.openlocfilehash: 873d372657089d21e86025cdf7812659ac505491
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543557"
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
|[Title](title.md) <br/> |Представляет название контакта.  <br/> |
|[FirstName](firstname.md) <br/> |Представляет имя контакта.  <br/> |
|[MiddleName](middlename.md) <br/> |Представляет второе имя контакта.  <br/> |
|[LastName](lastname.md) <br/> |Представляет фамилию контакта.  <br/> |
|[Suffix](suffix.md) <br/> |Представляет суффикс имени контакта.  <br/> |
|[Initials](initials.md) <br/> |Представляет инициалы контакта.  <br/> |
|[FullName](fullname.md) <br/> |Представляет полное имя контакта.  <br/> |
|[Nickname](nickname.md) <br/> |Представляет псевдоним контакта.  <br/> |
|[YomiFirstName](yomifirstname.md) <br/> |Представляет имя, используемое в Японии для поиска или фонетической орфографии японского имени.  <br/> |
|[YomiLastName](yomilastname.md) <br/> |Представляет имя, используемое в Японии для поиска или фонетической орфографии японской фамилии.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
   
## <a name="remarks"></a>Заметки

Свойство CompleteName является частью фигуры [по умолчанию.](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) В начальной версии выпуска Microsoft Exchange Server 2007 г. свойство CompleteName возвращается операцией [GetItem,](getitem-operation.md)но не [операцией FindItem.](finditem-operation.md) Начиная с Exchange Server 2007 Пакет обновления 1 (SP1), операция [FindItem](finditem-operation.md) также возвращает свойство CompleteName с фигурой [По умолчанию.](https://docs.microsoft.com/dotnet/api/exchangewebservices.defaultshapenamestype?view=exchange-ews-proxy) Это изменение не влияет на схему. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [CompleteNameType](https://msdn.microsoft.com/library/ExchangeWebServices.CompleteNameType.aspx)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание контактов (Exchange веб-служб)](https://msdn.microsoft.com/library/4845917e-70d1-481c-bbd7-011ec6571789%28Office.15%29.aspx)

