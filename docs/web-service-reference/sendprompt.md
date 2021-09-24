---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: Элемент SendPrompt указывает тип действий, разрешенных для выбора.
ms.openlocfilehash: 32537210aadce91911d1fb5002fbafcaa70aa9ab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532134"
---
# <a name="sendprompt"></a>SendPrompt

Элемент **SendPrompt** указывает тип действий, разрешенных для выбора. 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 **SendPromptType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[VotingOptionData](votingoptiondata.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **SendPrompt** — это действие параметра голосования. В таблице ниже перечислены возможные варианты последнего. 
  
****

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Никаких действий.  <br/> |
|Send  <br/> |Ответ отправляется немедленно.  <br/> |
|VotingOption  <br/> |Утвердитель может вводить комментарии при одобрении или отклонении.  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[VotingOptionData](votingoptiondata.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

