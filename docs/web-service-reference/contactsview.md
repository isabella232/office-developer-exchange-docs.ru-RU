---
title: контактсвиев
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
description: Элемент Контактсвиев определяет Поиск элементов контакта в соответствии с отображаемыми именами в алфавитном порядке.
ms.openlocfilehash: e578eb4dd0042b8c478e883c7fa54d7f2e984229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761752"
---
# <a name="contactsview"></a>контактсвиев

Элемент **контактсвиев** определяет Поиск элементов контакта в соответствии с отображаемыми именами в алфавитном порядке. 
  
[FindItem](finditem.md)
  
[контактсвиев](contactsview.md)
  
```xml
<ContactsView MaxEntriesReturned="" InitialName="" FinalName="" />
```

**контактсвиевтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**максентриесретурнед** <br/> |Описывает максимальное число результатов, возвращаемых в ответе [FindItem](finditem.md) .  <br/> |
|**инитиалнаме** <br/> |Определяет первое имя в списке контактов для возврата в ответе. Если указанное начальное имя отсутствует в списке Contacts (контакты), будет возвращено следующее буквенное имя, заданное культурным контекстом, за исключением случаев, когда следующее имя предшествует **финалнаме**. Если атрибут **инитиалнаме** опущен, ответ будет содержать список контактов, начинающихся с первого имени в списке контактов. Этот атрибут является необязательным.  <br/> |
|**финалнаме** <br/> |Определяет фамилию в списке контактов, возвращаемой в ответе. Если атрибут **финалнаме** опущен, ответ будет содержать все последующие контакты в указанном порядке сортировки. Если указанное итоговое имя отсутствует в списке Contacts (контакты), то следующее буквенное имя, заданное культурным контекстом, будет исключено.  <br/><br/>Например, если Финалнаме = "Name", но имя отсутствует в списке Contacts (контакты), то контакты, у которых отображаются имена Имя1 или NAME, не будут включены.  <br/><br/>Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.<br/><br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В приведенном ниже примере запроса показано, как найти первые три контакта, начиная с контакта с отображаемым именем Kelly.
  
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
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

