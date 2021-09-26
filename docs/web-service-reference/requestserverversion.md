---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: Элемент RequestServerVersion содержит сведения о версии, определяющие версию схемы для целевого запроса.
ms.openlocfilehash: 4f01d5fcc2a2e08d426efc8d1f0a193d6139a038
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541877"
---
# <a name="requestserverversion"></a>RequestServerVersion

Элемент **RequestServerVersion** содержит сведения о версии, определяющие версию схемы для целевого запроса. 
  
```XML
<RequestServerVersion Version=""/>
```

 **ExchangeVersionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Версия  <br/> |Описывает версию для целевого запроса. Этот атрибут необходим, когда версия целевого сервера является версией Exchange начиная с Exchange Server 2010 года.  <br/> |
   
#### <a name="version-attribute-values"></a>Значения атрибута версии

|**Значение**|**Описание**|
|:-----|:-----|
|Exchange2007  <br/> |Целевые файлы схемы для начальной версии Exchange 2007.  <br/> |
|Exchange2007_SP1  <br/> |Целевые файлы схемы для Exchange 2007 Пакет обновления 1 (SP1), Exchange 2007 Пакет обновления 2 (SP2) и Exchange 2007 Пакет обновления 3 (SP3).  <br/> |
|Exchange2010  <br/> |Целевые файлы схемы для Exchange 2010.  <br/> |
|Exchange2010_SP1  <br/> |Целевые файлы схемы для Exchange 2010 Пакет обновления 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Целевые файлы схемы для Exchange 2010 Пакет обновления 2 (SP2) и Exchange 2010 Пакет обновления 3 (SP3).  <br/> |
|Exchange2013  <br/> |Целевые файлы схемы для Exchange 2013.  <br/> |
|Exchange2013_SP1  <br/> |Целевые файлы схемы для Exchange 2013 Пакет обновления 1 (SP1).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

Элемент **RequestServerVersion** расположен в загонах SOAP. 
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Запросы на версию](https://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

