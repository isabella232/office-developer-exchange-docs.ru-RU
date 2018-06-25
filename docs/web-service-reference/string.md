---
title: String
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- String
api_type:
- schema
ms.assetid: e6e362b1-4526-49e1-b283-1c4bc4295874
description: Строковый элемент представляет строку, которая используется с элементами, контакты, задачи и бесед.
ms.openlocfilehash: 66260c7ebcb56049a78c5eddbe057dfa8d61f193
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835607"
---
# <a name="string"></a>String

**Строковый** элемент представляет строку, которая используется с элементами, контакты, задачи и бесед. 
  
```XML
<String/>
```

 **string**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Категории](categories-ex15websvcsotherref.md) <br/> |Содержит коллекцию строк, чтобы указать, к какой категории относится элемент в почтовом ящике.  <br/> |
|[Дочерние элементы](children.md) <br/> |Содержит имена дочерние элементы элемента контакта.  <br/> |
|[Компании](companies.md) <br/> |Представляет коллекцию компании, связанные с контактом или задач.  <br/> |
|[Контакты](contacts-ex15websvcsotherref.md) <br/> |Содержит список контактов, связанных с задачей.  <br/> |
|[GlobalCategories](globalcategories.md) <br/> |Содержит список категорий для всех элементов беседы в почтовом ящике.  <br/> |
|[GlobalUniqueRecipients](globaluniquerecipients.md) <br/> |Содержит список получателей беседы сводный в почтовый ящик.  <br/> |
|[GlobalUniqueSenders](globaluniquesenders.md) <br/> |Содержит список всех отправителей беседы элементов в почтовом ящике.  <br/> |
|[GlobalUniqueUnreadSenders](globaluniqueunreadsenders.md) <br/> |Содержит список всех людей, отправленные сообщения, в настоящее время непрочитанные сообщения в беседе для всех папок в почтовом ящике.  <br/> |
|[ItemClasses](itemclasses.md) <br/> |Содержит список классов элементов, которые необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[MessageClassifications](messageclassifications.md) <br/> |Содержит список классификации сообщений, которые необходимо ставится отметка для входящих сообщений в порядке для условие или исключение для применения.  <br/> |
|[UniqueRecipients](uniquerecipients.md) <br/> |Содержит список получателей беседы. Этот элемент доступен только для чтения.  <br/> |
|[UniqueSenders](uniquesenders.md) <br/> |Содержит список всех отправителей элементов беседы в текущую папку. Этот элемент доступен только для чтения.  <br/> |
|[UniqueUnreadSenders](uniqueunreadsenders.md) <br/> |Содержит список всех людей, отправленные сообщения, которые в настоящее время непрочитанные сообщения в эту беседу в текущую папку.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение этого элемента — это строка, представляющая категорию дочернего элемента контакта, компании, уникальный получателя беседы или контакт, который связан с задачей.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[FindConversation Operation](findconversation-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

