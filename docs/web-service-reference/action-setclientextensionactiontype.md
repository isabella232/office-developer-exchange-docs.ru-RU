---
title: Action (Сетклиентекстенсионактионтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c5624a87-3436-40ce-8d6b-cc01eecab64d
description: Элемент Action содержит действие, которое сервер Exchange должен выполнить в приложении.
ms.openlocfilehash: 29579e26377edacb5fb0bb8406144eeb116b8d15
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529688"
---
# <a name="action-setclientextensionactiontype"></a>Action (Сетклиентекстенсионактионтипе)

Элемент **Action** содержит действие, которое сервер Exchange должен выполнить в приложении. 
  
```XML
<Action ActionId="" ExtensionId="">
   <ClientExtension/>
</Action>
```

 **сетклиентекстенсионактионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|ActionId  <br/> |Задает идентификатор действия. Этот атрибут является обязательным.  <br/> |
|екстенсионид  <br/> |Задает идентификатор расширения. Этот атрибут является необязательным.  <br/> |
   
#### <a name="actionid"></a>ActionId

|**Значение**|**Описание**|
|:-----|:-----|
|Configure (Настроить)  <br/> |Указывает действие конфигурации.  <br/> |
|Установка  <br/> |Указывает действие установки.  <br/> |
|Uninstall  <br/> |Указывает действие по удалению.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[клиентекстенсион](clientextension.md) <br/> |Содержит сведения о пользователях и конфигурации приложения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Actions (Аррайофсетклиентекстенсионактионстипе)](actions-arrayofsetclientextensionactionstype.md) <br/> |Указывает массив элементов **Action** .  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

