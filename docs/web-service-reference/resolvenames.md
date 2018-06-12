---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: Элемент ResolveNames определяет запрос для разрешения неоднозначных имен.
ms.openlocfilehash: e97b6e78d99cf8ffa3d680907916882d40963f59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835172"
---
# <a name="resolvenames"></a>ResolveNames

Элемент **ResolveNames** определяет запрос для разрешения неоднозначных имен. 
  
```XML
<ResolveNames ReturnFullContactData="" SearchScope="" ContactDataShape="">
   <ParentFolderIds/>
   <UnresolvedEntry/>
</ResolveNames>
```

 **ResolveNamesType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ReturnFullContactData** <br/> |Описание, возвращаются ли полные контактные данные для контактов общедоступной для разрешения имени в ответе. Этот атрибут является обязательным для контактов общедоступной. Это значение не влияет на закрытый контактов и частные списки рассылки, для которых всегда возвращается [идентификатор элемента](itemid.md) .  <br/> |
|**Область поиска** <br/> |Определяет порядок и области для поиска ResolveNames.  <br/> |
|ContactDataShape  <br/> |Определяет свойство набор, возвращаемый для контактов. Этот атрибут появился в Exchange Server 2010 с пакетом обновления 2 (SP2).  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>Значения атрибутов ReturnFullContactData

|**Значение**|**Описание**|
|:-----|:-----|
|True  <br/> |Возвращаются полные контактные данные для контактов общедоступной.  <br/> |
|False  <br/> |Полное контактные данные для контактов общедоступной не возвращается.  <br/> |
   
#### <a name="searchscope-attribute-values"></a>Значения атрибутов область поиска

|**Значение**|**Описание**|
|:-----|:-----|
|ActiveDirectory  <br/> |Поиск службы каталогов Active Directory.  <br/> |
|ActiveDirectoryContacts  <br/> |Сначала выполняется поиск Active Directory, а затем выполняется поиск контакта папках, указанных в свойстве [ParentFolderIds](parentfolderids.md) .  <br/> |
|Контакты  <br/> |Поиск осуществляется только папки контактов, указанных в свойстве [ParentFolderIds](parentfolderids.md) .  <br/> |
|ContactsActiveDirectory  <br/> |Сначала выполняется поиск папок контактов, указанных в свойстве [ParentFolderIds](parentfolderids.md) и затем выполняется поиск Active Directory.  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>Значения атрибутов ContactDataShape

|**Значение**|**Описание**|
|:-----|:-----|
|IdOnly  <br/> |Свойство идентификатора элемента контакта, возвращается.  <br/> |
|Значение по умолчанию  <br/> |Возвращается набор по умолчанию свойства элемента контакта. Для получения дополнительных сведений см [ответа фигур в веб-служб Exchange](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
|AllProperties  <br/> |Возвращаются AllProperties набора свойств элемента контакта. Для получения дополнительных сведений см [ответа фигур в веб-служб Exchange](http://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |Содержит массив идентификаторов папке контактов, которые будет искать, если значение атрибута **область поиска** ActiveDirectoryContacts, контактов или ContactsActiveDirectory. Массив ParentFolderIds может содержать только идентификатор одной папке контактов. Если элемент **ParentFolderIds** не задан, выполняется поиск папки Контакты по умолчанию.  <br/> Идентификатор папки можно использовать для доступа делегата.  <br/> Поиск Active Directory выполняются с помощью списки управления доступом (ACL). Некоторым пользователям может не иметь права на доступ, чтобы увидеть некоторые объекты Active Directory.  <br/> Этот элемент является необязательным.  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |Содержит имя контакта или список рассылки для разрешения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ResolveNames](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[С помощью разрешения имен](http://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

