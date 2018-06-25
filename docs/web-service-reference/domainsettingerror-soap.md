---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: Элемент DomainSettingError представляет ошибки, возникшей при получении Настройка домена. Представляет ошибку из GetDomainSettings запроса.
ms.openlocfilehash: 08b0a47acea8d35ec78efd701168a251771effac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762216"
---
# <a name="domainsettingerror-soap"></a>DomainSettingError (SOAP)

Элемент **DomainSettingError** представляет ошибки, возникшей при получении Настройка домена. Представляет ошибку из **GetDomainSettings** запроса. 
  
```XML
<DomainSettingError>
   <ErrorCode/>
   <ErrorMessage/>
   <SettingName/>
</DomainSettingError>
```

 **DomainSettingError**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Код ошибки (SOAP)](errorcode-soap.md) <br/> |Определяет код ошибки, связанный с данным запросом.  <br/> |
|[Сообщение об ошибке (SOAP)](errormessage-soap.md) <br/> |Содержит сообщение об ошибке, связанный с данным запросом.  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |Представляет имя удаляемого параметра.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Содержит сведения об ошибке для параметров, которые не будут получены.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема службы автообнаружения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

