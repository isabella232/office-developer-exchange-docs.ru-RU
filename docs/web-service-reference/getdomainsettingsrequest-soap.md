---
title: Жетдомаинсеттингсрекуест (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5ac0ff6d-9e02-4e4c-973d-cd9e076661d5
description: Элемент Жетдомаинсеттингсрекуест представляет запрос операции Жетдомаинсеттингс (SOAP).
ms.openlocfilehash: 400016d0817131fb70ec7ff3db7fbfdc1b51f8f9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460962"
---
# <a name="getdomainsettingsrequest-soap"></a>Жетдомаинсеттингсрекуест (SOAP)

Элемент **жетдомаинсеттингсрекуест** представляет запрос операции [жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) . 
  
```XML
<GetDomainSettingsRequest>
   <Domains/>
   <RequestedSettings/>
   <RequestedVersion/>
</GetDomainSettingsRequest>
```

 **жетдомаинсеттингсрекуест**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Домены (SOAP)](domains-soap.md) <br/> |Представляет коллекцию идентификаторов доменов.  <br/> |
|[Рекуестедсеттингс (SOAP)](requestedsettings-soap.md) <br/> |Содержит имена запрошенных параметров конфигурации домена.  <br/> |
|[Рекуестедверсион (SOAP)](requestedversion-soap.md) <br/> |Указывает версию сервера, который будет использоваться поставщиком.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Отсутствуют.
  
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также



[Операция Жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md)

