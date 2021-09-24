---
title: DomainSettingError (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: 48c3f7b5-2ee0-42ce-97a1-a881e2f60327
description: Элемент DomainSettingError представляет ошибку, которая произошла при ирисовке параметра домена. Это представляет ошибку из запроса GetDomainSettings.
ms.openlocfilehash: d2d7e1fc1509ade88de0013cb9e4ff54712d0f56
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530149"
---
# <a name="domainsettingerror-soap"></a>DomainSettingError (SOAP)

Элемент **DomainSettingError представляет** ошибку, которая произошла при ирисовке параметра домена. Это представляет ошибку из **запроса GetDomainSettings.** 
  
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
|[ErrorCode (SOAP)](errorcode-soap.md) <br/> |Определяет код ошибки, связанный с определенным запросом.  <br/> |
|[ErrorMessage (SOAP)](errormessage-soap.md) <br/> |Содержит сообщение об ошибке, связанное с определенным запросом.  <br/> |
|[SettingName (SOAP)](settingname-soap.md) <br/> |Представляет имя параметра.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DomainSettingErrors (SOAP)](domainsettingerrors-soap.md) <br/> |Содержит сведения об ошибках для параметров, которые не удалось вернуть.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetDomainSettings (SOAP)](getdomainsettings-operation-soap.md)

