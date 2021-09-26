---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: Элемент AllowNewTimeProposal указывает, может ли участник использовать новое время собрания для собрания.
ms.openlocfilehash: 1acb95189e1949204a25f97a82770b88590df776
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543732"
---
# <a name="allownewtimeproposal"></a>AllowNewTimeProposal

Элемент **AllowNewTimeProposal** указывает, может ли участник использовать новое время собрания для собрания. 
  
```xml
<AllowNewTimeProposal/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее логическое значение является обязательным. Значение true **указывает** на то, что можно создать новое предложение для времени собрания; значение false **указывает** на то, что новые предложения времени не допускаются. Организатор задает это значение в запросе собрания. 
  
## <a name="remarks"></a>Заметки

Свойство AllowNewTimeProposal можно прочитать для элемента календаря организатора. Это только для чтения запросов на собрания и для элементов календаря участников.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
> [!NOTE]
> Exchange Веб-службы не поддерживают сообщения предложений о новом времени. Чтобы получить свойства, связанные с сообщениями о новом предложении времени, используйте расширенные свойства. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

