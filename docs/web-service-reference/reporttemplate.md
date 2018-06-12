---
title: Шаблон_отчета
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ReportTemplate
api_type:
- schema
ms.assetid: f528eee6-d5af-4745-8b00-a9834bf34be6
description: Элемент Шаблон_отчета представляет тип отчета требуется получить.
ms.openlocfilehash: 70aab69f4d20ad9fd7e878c7fccd16e261c9b94c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835118"
---
# <a name="reporttemplate"></a>Шаблон_отчета

Элемент **Шаблон_отчета** представляет тип отчета требуется получить. 
  
```xml
<ReportTemplate>Summary or RecipientPath</ReportTemplate>
```

 **MessageTrackingReportTemplateType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetMessageTrackingReport](getmessagetrackingreport.md) <br/> |Содержит запроса для [операции GetMessageTrackingReport](getmessagetrackingreport-operation.md) для получения полного сообщения, отслеживания отчетов для указанного идентификатора.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **Шаблон_отчета** . 
  
**Значения элементов Шаблон_отчета**

|**Значение**|**Описание**|
|:-----|:-----|
|Сводка  <br/> |Указывает, что отчет будет отображаться всех получателей сообщения, а также состояние доставки сообщения для каждого получателя.  <br/> |
|RecipientPath  <br/> |Указывает, что для одного получателя, отчет будет отображаться с помощью журнала событий, возникших.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

