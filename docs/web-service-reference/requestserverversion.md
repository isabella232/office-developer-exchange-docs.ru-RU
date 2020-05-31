---
title: рекуестсерверверсион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: Элемент Рекуестсерверверсион содержит сведения об управлении версиями, которые определяют версию схемы, предназначенную для запроса.
ms.openlocfilehash: 0092d90a5fc479363f6d774b793c7148ad29f21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835143"
---
# <a name="requestserverversion"></a>рекуестсерверверсион

Элемент **рекуестсерверверсион** содержит сведения об управлении версиями, которые определяют версию схемы, предназначенную для запроса. 
  
```XML
<RequestServerVersion Version=""/>
```

 **Простом типе exchangeversiontype**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Версия  <br/> |Описывает версию, целевую для запроса. Этот атрибут является обязательным, если версия целевого сервера является версией Exchange, начиная с Exchange Server 2010.  <br/> |
   
#### <a name="version-attribute-values"></a>Значения атрибутов Version

|**Значение**|**Описание**|
|:-----|:-----|
|Exchange2007  <br/> |Нацеливание файлов схемы для первоначальной версии Exchange 2007.  <br/> |
|Exchange2007_SP1  <br/> |Нацеливание файлов схемы для Exchange 2007 с пакетом обновления 1 (SP1), Exchange 2007 с пакетом обновления 2 (SP2) и Exchange 2007 с пакетом обновления 3 (SP3).  <br/> |
|Exchange2010  <br/> |Нацеливание файлов схемы для Exchange 2010.  <br/> |
|Exchange2010_SP1  <br/> |Нацеливание файлов схемы для Exchange 2010 с пакетом обновления 1 (SP1).  <br/> |
|Exchange2010_SP2  <br/> |Нацеливание файлов схемы для Exchange 2010 с пакетом обновления 2 (SP2) и Exchange 2010 с пакетом обновления 3 (SP3).  <br/> |
|Exchange2013  <br/> |Нацеливание файлов схемы для Exchange 2013.  <br/> |
|Exchange2013_SP1  <br/> |Нацеливание файлов схемы для Exchange 2013 с пакетом обновления 1 (SP1).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

Элемент **рекуестсерверверсион** находится в заголовке SOAP. 
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Запросы управления версиями](http://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

