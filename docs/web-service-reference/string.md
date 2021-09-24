---
title: String
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- String
api_type:
- schema
ms.assetid: e6e362b1-4526-49e1-b283-1c4bc4295874
description: Элемент String представляет строку, используемую элементами, контактами, задачами и беседами.
ms.openlocfilehash: dd85cae34ddf829f00660c8b87feb9331505183c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509296"
---
# <a name="string"></a>String

Элемент **String** представляет строку, используемую элементами, контактами, задачами и беседами. 
  
```XML
<String/>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Categories](categories-ex15websvcsotherref.md) <br/> |Содержит коллекцию строк, которые определяют, к какой категории относится элемент в почтовом ящике.  <br/> |
|[Children](children.md) <br/> |Содержит имена детей контакта.  <br/> |
|[Companies](companies.md) <br/> |Представляет коллекцию компаний, связанных с контактом или задачей.  <br/> |
|[Контакты](contacts-ex15websvcsotherref.md) <br/> |Содержит список контактов, связанных с задачей.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Содержит список категорий для всех элементов беседы в почтовом ящике.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Содержит список получателей беседы, агрегированных в почтовом ящике.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Содержит список всех отправителей элементов беседы в почтовом ящике.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Содержит список всех людей, которые отправили сообщения, которые в настоящее время нечитаются в этом разговоре во всех папках в почтовом ящике.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Содержит список классов элементов, которые должны быть запечатаны на входящих сообщениях, чтобы применить условие или исключение.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Содержит список классификаций сообщений, которые необходимо маркировать на входящих сообщениях, чтобы применить условие или исключение.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Содержит список получателей беседы. Этот элемент доступен только для чтения.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Содержит список всех отправителей элементов беседы в текущей папке. Этот элемент доступен только для чтения.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Содержит список всех людей, отправивших сообщения, которые в настоящее время нечитаются в этом разговоре в текущей папке.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение этого элемента представляет собой строку, которая представляет категорию, ребенка контакта, компании, уникального получателя беседы или контакта, связанного с задачей.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция FindConversation](findconversation-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

