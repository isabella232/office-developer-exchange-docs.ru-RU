---
title: фаиледмаилбокс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: Элемент Фаиледмаилбокс указывает сообщение об ошибке для почтового ящика, на который произошел сбой поиска.
ms.openlocfilehash: a4f5cd975eba121dd1d8d918b638d34f907588a8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762522"
---
# <a name="failedmailbox"></a>фаиледмаилбокс

Элемент **фаиледмаилбокс** указывает сообщение об ошибке для почтового ящика, на который произошел сбой поиска. 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 **фаиледсеарчмаилбокстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox (строка)](mailbox-string.md) <br/> |Содержит идентификатор для почтового ящика.  <br/> |
|[ErrorCode (int)](errorcode-int.md) <br/> |Указывает код ошибки почтового ящика, в котором произошел сбой поиска.  <br/> |
|[ErrorMessage](errormessage.md) <br/> |Представляет причину ошибки проверки.  <br/> |
|[IsArchive](isarchive.md) <br/> |Задает логическое значение, указывающее, является ли почтовый ящик архивным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фаиледмаилбоксес](failedmailboxes.md) <br/> |Указывает массив неудачных почтовых ящиков.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

