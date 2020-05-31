---
title: Language (Дисковерисеарчконфигуратионтипе)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 34eab81c-d832-4925-9f76-d69f24b36931
description: Элемент Language (Дисковерисеарчконфигуратионтипе) определяет язык и региональные параметры, используемые для форматирования диапазонов дат для определенного языка и региональных параметров. Он также определяет язык, используемый в поисковом запросе.
ms.openlocfilehash: 1e904ac4d7f525b2d12cfe83f0da33b9ed474066
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834197"
---
# <a name="language-discoverysearchconfigurationtype"></a>Language (Дисковерисеарчконфигуратионтипе)

Элемент **Language (дисковерисеарчконфигуратионтипе)** определяет язык и региональные параметры, используемые для форматирования диапазонов дат для определенного языка и региональных параметров. Он также определяет язык, используемый в поисковом запросе. 
  
```XML
<Language />
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

[дисковерисеарчконфигуратион](discoverysearchconfiguration.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Language (дисковерисеарчконфигуратионтипе)** — это язык и региональные параметры или язык. 
  
## <a name="remarks"></a>Примечания

Этот элемент указывает формат диапазонов дат, указанных в [операции SearchMailboxes](searchmailboxes-operation.md) или [SetHoldOnMailboxes](setholdonmailboxes-operation.md).
  
Этот элемент появился в Exchange Server 2013 с пакетом обновления 1 (SP1).
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[дисковерисеарчконфигуратион](discoverysearchconfiguration.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

