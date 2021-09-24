---
title: Language (DiscoverySearchConfigurationType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: Элемент Language (DiscoverySearchConfigurationType) определяет культуру, используемую для определенного для культуры формата диапазонов дат. Он также указывает язык, используемый в поисковом запросе.
ms.openlocfilehash: 5d51960aa00b2c47d96972abc05e4d6027eeecb3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540897"
---
# <a name="language-discoverysearchconfigurationtype"></a>Language (DiscoverySearchConfigurationType)

Элемент **Language (DiscoverySearchConfigurationType)** определяет культуру, используемую для определенного для культуры формата диапазонов дат. Он также указывает язык, используемый в поисковом запросе. 
  
```XML
<Language />
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[DiscoverySearchConfiguration](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Language (DiscoverySearchConfigurationType)** — это культура или язык. 
  
## <a name="remarks"></a>Заметки

Этот элемент указывает формат диапазонов дат, указанных в операции [SearchMailboxes](searchmailboxes-operation.md) или [операции SetHoldOnMailboxes.](setholdonmailboxes-operation.md)
  
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



[DiscoverySearchConfiguration](discoverysearchconfiguration.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

