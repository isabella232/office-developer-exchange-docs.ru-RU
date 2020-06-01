---
title: алловневтимепропосал
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
description: Элемент Алловневтимепропосал указывает, может ли новое время проведения собрания предлагаться участнику.
ms.openlocfilehash: b3f2c569bced08c66144680a4fddd6e8bac0cecf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464807"
---
# <a name="allownewtimeproposal"></a>алловневтимепропосал

Элемент **алловневтимепропосал** указывает, может ли новое время проведения собрания предлагаться участнику. 
  
```xml
<AllowNewTimeProposal/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Свойство meetingrequest](meetingrequest.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее логическое значение является обязательным. Значение **true** указывает, что можно создать новое предложение для времени собрания; значение **false** указывает, что новые предложения времени не разрешены. Организатор задает это значение в приглашении на собрание. 
  
## <a name="remarks"></a>Примечания

Свойство Алловневтимепропосал доступно для записи в элементе календаря организатора. Он доступен только для чтения для приглашений на собрания и элементов календаря участников.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
> [!NOTE]
> Веб-службы Exchange не поддерживают новые сообщения о предложениях времени. Чтобы получить свойства, связанные с новыми сообщениями предложений по времени, используйте расширенные свойства. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

