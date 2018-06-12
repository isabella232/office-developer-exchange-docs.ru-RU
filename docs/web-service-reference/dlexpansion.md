---
title: DLExpansion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DLExpansion
api_type:
- schema
ms.assetid: 9e50278d-fe6a-45e2-a72b-0fb06809e128
description: Элемент DLExpansion содержит массив почтовых ящиков, которые содержатся в списке рассылки.
ms.openlocfilehash: 06081b4aba761a7137f921b3bc1c8d6b2afab88c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762199"
---
# <a name="dlexpansion"></a>DLExpansion

Элемент **DLExpansion** содержит массив почтовых ящиков, которые содержатся в списке рассылки. 
  
- [ExpandDLResponse](expanddlresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [ExpandDLResponseMessage](expanddlresponsemessage.md)
- [DLExpansion](dlexpansion.md)
  
```xml
<DLExpansion AbsoluteDenominator"" IncludesLastItemInRange="" IndexedPagingOffset="" NumeratorOffset="" TotalItemsInView="">
   <Mailbox/>
</DLExpansion>
```

 **ArrayOfDLExpansionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**IndexedPagingOffset** <br/> |Представляет следующий индекс, который необходимо использовать для следующего запроса при использовании индексированного страницы представления.  <br/> |
|**NumeratorOffset** <br/> |Представляет новое значение перечислителя использовать для следующего запроса при использовании просмотров страниц дроби.  <br/> |
|**AbsoluteDenominator** <br/> |Представляет Далее делителя будет использоваться для следующего запроса при использовании просмотров страниц дроби.  <br/> |
|**IncludesLastItemInRange** <br/> |Указывает, содержат ли текущие результаты последнего элемента в запросе, чтобы дополнительные разбиение на страницы не требуется.  <br/> |
|**TotalItemsInView** <br/> |Представляет общее число элементов в представлении.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ExpandDLResponseMessage](expanddlresponsemessage.md) <br/> |Содержит состояние и результат одного запроса ExpandDL.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ExpandDL](expanddl-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md) 
- [Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)

