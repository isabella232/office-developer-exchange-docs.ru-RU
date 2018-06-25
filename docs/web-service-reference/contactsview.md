---
title: ContactsView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsView
api_type:
- schema
ms.assetid: 8534f44b-a5af-4a9f-9621-23a3eff5f9d8
description: Элемент ContactsView определяет поиска на основе алфавитном отображения имен контактов.
ms.openlocfilehash: e578eb4dd0042b8c478e883c7fa54d7f2e984229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761752"
---
# <a name="contactsview"></a>ContactsView

Элемент **ContactsView** определяет поиска на основе алфавитном отображения имен контактов. 
  
[FindItem](finditem.md)
  
[ContactsView](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

**ContactsViewType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Описывает максимальное число результатов, возвращаемых в ответе [FindItem](finditem.md) .  <br/> |
|**InitialName** <br/> |Определяет имя в списке контактов, чтобы вернуться в ответе. Если указанный начальное имя не в списке контактов, далее алфавитном имя в соответствии с культурные контекста будут возвращены, за исключением Если далее имя идет после **FinalName**. Если указан атрибут **InitialName** , ответ будет содержать список контактов, начинающимся на имя в списке контактов. Этот атрибут является необязательным.  <br/> |
|**FinalName** <br/> |Определяет имя последнего в списке контактов, чтобы вернуться в ответе. Если указан атрибут **FinalName** , ответ будет содержать все последующие контакты в заданный порядок сортировки. Если указанный окончательное имя не в списке контактов, далее алфавитном имя в соответствии с культурные контекста будет исключен.  <br/><br/>Например если FinalName = «Имя», но имя не входит в список контактов, контакты, имеющие отображение имен из Имя1 или не будет включен.  <br/><br/>Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос для поиска элементов в почтовом ящике.<br/><br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

Следующий пример запроса показано, как найти первые три контакты, начиная с контактом, который содержит отображаемое имя Келли Ролин.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ContactsView MaxEntriesReturned="3" InitialName="Kelly Rollin" />
      <SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="contacts:DisplayName"/>
        </t:FieldOrder>
        </SortOrder>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [FindItem Operation](finditem-operation.md)
- [Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

