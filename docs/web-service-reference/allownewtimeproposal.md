---
title: AllowNewTimeProposal
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AllowNewTimeProposal
api_type:
- schema
ms.assetid: afdb4ec9-2daf-48a1-a0bb-a7f647f212f2
description: Элемент AllowNewTimeProposal указывает, можно ли участником предлагаться собрание для собрания.
ms.openlocfilehash: d5deed5044769c477ffe54cc533d5261ba2e1932
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761369"
---
# <a name="allownewtimeproposal"></a>AllowNewTimeProposal

Элемент **AllowNewTimeProposal** указывает, можно ли участником предлагаться собрание для собрания. 
  
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
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее логическое значение является обязательным. Значение **true** указывает, что можно создать новое предложение для время собрания; значение **false** указывает, что новые предложения времени не допускается. Это значение устанавливается организатора в приглашении на собрание. 
  
## <a name="remarks"></a>Замечания

Свойство AllowNewTimeProposal чтения записи для организатора элемента календаря. Оно доступно только для чтения, для приглашений на собрания и элементы календаря участников.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
> [!NOTE]
> Веб-служб Exchange не поддерживает новые сообщения предложения времени. Получение свойств, относящихся к сообщениям предложение нового времени, используйте расширенные свойства. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

