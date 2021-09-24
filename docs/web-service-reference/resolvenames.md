---
title: ResolveNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ResolveNames
api_type:
- schema
ms.assetid: c85207e1-1315-443b-94ec-2b58f405076b
description: Элемент ResolveNames определяет запрос на разрешение неоднозначных имен.
ms.openlocfilehash: 8fbf933593b43de656bf8731aa86cc8c8eb76bb4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514146"
---
# <a name="resolvenames"></a>ResolveNames

Элемент **ResolveNames** определяет запрос на разрешение неоднозначных имен. 
  
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
|**ReturnFullContactData** <br/> |Описывает, возвращаются ли в ответ полные контактные данные для общедоступных контактов для разрешенного имени. Этот атрибут необходим для общедоступных контактов. Это значение не влияет на частные контакты и частные списки рассылки, для которых [ItemId](itemid.md) всегда возвращается.  <br/> |
|**SearchScope** <br/> |Определяет порядок и область поиска ResolveNames.  <br/> |
|ContactDataShape  <br/> |Определяет набор свойств, возвращаемый для контактов. Этот атрибут был введен в Exchange Server 2010 Пакет обновления 2 (SP2).  <br/> |
   
#### <a name="returnfullcontactdata-attribute-values"></a>Значения атрибута ReturnFullContactData

|**Значение**|**Описание**|
|:-----|:-----|
|Верно  <br/> |Возвращаются полные контактные данные для общедоступных контактов.  <br/> |
|Неверно  <br/> |Полные контактные данные для общедоступных контактов не возвращаются.  <br/> |
   
#### <a name="searchscope-attribute-values"></a>Значения атрибута SearchScope

|**Значение**|**Описание**|
|:-----|:-----|
|ActiveDirectory  <br/> |Поиск ведется только в службе каталогов Active Directory.  <br/> |
|ActiveDirectoryContacts  <br/> |Сначала поиск active Directory, а затем поиск папок контактов, указанных в свойстве [ParentFolderIds.](parentfolderids.md)  <br/> |
|Контакты  <br/> |Поиск ведется только в папках контактов, идентифицированных [свойством ParentFolderIds.](parentfolderids.md)  <br/> |
|ContactsActiveDirectory  <br/> |Сначала ищут папки контактов, которые определены [свойством ParentFolderIds,](parentfolderids.md) а затем — Active Directory.  <br/> |
   
#### <a name="contactdatashape-attribute-values"></a>Значения атрибутов ContactDataShape

|**Значение**|**Описание**|
|:-----|:-----|
|IdOnly  <br/> |Возвращается свойство идентификатора элемента контакта.  <br/> |
|По умолчанию  <br/> |Возвращается набор свойств контактных элементов по умолчанию. Дополнительные сведения см. [в дополнительных сведениях о формах ответа в EWS.](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)  <br/> |
|AllProperties  <br/> |Возвращается набор свойств контактных элементов AllProperties. Дополнительные сведения см. [в дополнительных сведениях о формах ответа в EWS.](https://msdn.microsoft.com/library/1c5ddc0a-c4e0-4488-8972-7543b5b464df%28Office.15%29.aspx)  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ParentFolderIds](parentfolderids.md) <br/> |Содержит массив идентификаторов контактных папок, которые будут искать, если атрибут **SearchScope** задарен ActiveDirectoryContacts, Contacts Или ContactsActiveDirectory. Массив ParentFolderIds может содержать только один идентификатор папки контактов. Если элемента **ParentFolderIds** нет, папка Contacts по умолчанию будет искаться.  <br/> Идентификатор папки можно использовать для делегирования доступа.  <br/> Поиск active Directory выполняется с помощью списков управления доступом (ACLs). Некоторые пользователи могут не иметь прав на просмотр некоторых объектов Active Directory.  <br/> Этот элемент является необязательным.  <br/> |
|[UnresolvedEntry](unresolvedentry.md) <br/> |Содержит имя списка контактов или рассылки для решения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция ResolveNames](resolvenames-operation.md)
  
[ResolveNamesType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesType.aspx)
  
[ResolveNamesSearchScopeType](https://msdn.microsoft.com/library/ExchangeWebServices.ResolveNamesSearchScopeType.aspx)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Использование разрешения имен](https://msdn.microsoft.com/library/9257fb07-89d2-46eb-b885-e2173fe6fbc1%28Office.15%29.aspx)

