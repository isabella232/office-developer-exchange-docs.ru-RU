---
title: жетпассвордекспиратиондатереспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: Элемент Жетпассвордекспиратиондатереспонсе определяет ответ на запрос операции GetPasswordExpirationDate.
ms.openlocfilehash: c925b2b37879ba0f8f25b2dd73737ed2f3202555
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530206"
---
# <a name="getpasswordexpirationdateresponse"></a>жетпассвордекспиратиондатереспонсе

Элемент **жетпассвордекспиратиондатереспонсе** определяет ответ на запрос операции [GetPasswordExpirationDate](getpasswordexpirationdate-operation.md) . 
  
- [респонсемессажес](responsemessages.md)
- [жетпассвордекспиратиондатереспонсе](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 **жетпассвордекспиратиондатереспонсемессажетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**респонсекласс** <br/> | Описывает состояние ответа. <br/><br/>Для этого атрибута допустимы следующие значения:  <br/><br/>Успешное выполнение  <br/>— Предупреждение  <br/>— Ошибка  <br/> |
   
#### <a name="responseclass-attribute-values"></a>Значения атрибутов Респонсекласс

|**Значение**|**Описание**|
|:-----|:-----|
|**Success** <br/> |Описывает выполненный запрос.  <br/> |
|**Warning** <br/> | Описывает запрос, который не был обработан. Если при обработке элемента в запросе возникла ошибка, которая не может быть обработана, может быть возвращено предупреждение.<br/><br/> Ниже приведены примеры источников предупреждений.  <br/><br/>— Хранилище Exchange находится в автономном режиме во время выполнения пакета.  <br/>-Доменные службы Active Directory (AD DS) находятся в автономном режиме.  <br/>— Почтовые ящики были перемещены.  <br/>— База данных сообщений (MDB) находится в автономном режиме.  <br/>— Срок действия пароля истек.  <br/>— Превышена квота.  <br/> |
|**Error** <br/> | Описывает запрос, который не может быть выполнен. <br/><br/>Ниже приведены примеры источников ошибок.  <br/><br/>— Недопустимые атрибуты или элементы.  <br/>— Атрибуты или элементы, которые выходят за пределы диапазона.  <br/>— Неизвестный тег.  <br/>— Атрибут или элемент, который не является допустимым в контексте.  <br/>— Попытки несанкционированного доступа, выполняемые любым клиентом.  <br/>— Сбой на стороне сервера в ответ на действительный вызов на стороне клиента.  <br/><br/>  Сведения об ошибке можно найти в элементах [респонсекоде](responsecode.md) и [мессажетекст](messagetext.md) .  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[пассвордекспиратиондате](passwordexpirationdate.md) <br/> |Предоставляет срок действия пароля для учетной записи электронной почты, указанной в запросе.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Имя элемента**|**Описание**|
|:-----|:-----|
|[респонсемессажес](responsemessages.md) <br/> |Содержит сообщения ответа для запроса веб-служб Exchange (EWS).  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2010 с пакетом обновления 2 (SP2).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetPasswordExpirationDate](getpasswordexpirationdate-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

