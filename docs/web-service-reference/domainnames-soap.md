---
title: DomainNames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: Элемент DomainNames представляет коллекцию доменных имен. Элемент DomainNames используется только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 7697b05d7432051b9048837cb41894684f52be15
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526418"
---
# <a name="domainnames-soap"></a>DomainNames (SOAP)

Элемент **DomainNames** представляет коллекцию доменных имен. Элемент **DomainNames** используется только для внутреннего использования. Этот элемент не используется клиентами. 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 **DomainNames**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Domains (SOAP)](domains-soap.md) <br/> |Представляет коллекцию доменов, возвращающихся из операции [GetDomainSettings (SOAP),](getdomainsettings-operation-soap.md) [операции GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)или [операции GetOrganizationRelationshipSettings (SOAP).](getorganizationrelationshipsettings-operation-soap.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[OrganizationRelationshipSettings (SOAP)](organizationrelationshipsettings-soap.md) <br/> |Представляет список отношений организации для одной организации.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Этот элемент представляет домены SMTP внешних организаций.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автооткрытия  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetOrganizationRelationshipSettings (SOAP)](getorganizationrelationshipsettings-operation-soap.md)

