---
title: Организатионрелатионшипсеттингс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 917481bb-46fc-4b88-8683-4cf812dcb0ab
description: Элемент Организатионрелатионшипсеттингс представляет список отношений Организации для одной организации. Элемент Организатионрелатионшипсеттингс предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 383b3635e1435c6597ccf793a7990c411c02d36d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462460"
---
# <a name="organizationrelationshipsettings-soap"></a>Организатионрелатионшипсеттингс (SOAP)

Элемент **организатионрелатионшипсеттингс** представляет список отношений Организации для одной организации. Элемент **организатионрелатионшипсеттингс** предназначен только для внутреннего использования. Этот элемент не используется клиентами. 
  
```XML
<OrganizationRelationshipSettings>
    <DeliveryReportEnabled/>
    <DomainNames/>
    <FreeBusyAccessEnabled/>
    <FreeBusyAccessLevel/>
    <MailTipsAccessEnabled/>
    <MailTipsAccessLevel/>
    <MailboxMoveEnabled/>
    <Name/>
    <TargetApplicationUri/>
    <TargetAudodiscoverEpr/>
    <TargetSharingEpr/>
</OrganizationRelationshipSettings>
```

 **организатионрелатионшипсеттингс**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Деливерирепортенаблед (SOAP)](deliveryreportenabled-soap.md) <br/> |Представляет флаг [деливерирепортенаблед ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) .  <br/> |
|[Имя_домена (SOAP)](domainnames-soap.md) <br/> |Представляет коллекцию доменных имен.  <br/> |
|[Фрибусякцессенаблед (SOAP)](freebusyaccessenabled-soap.md) <br/> |Представляет флаг [фрибусякцессенаблед ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) .  <br/> |
|[FreeBusyAccessLevel (SOAP)](freebusyaccesslevel-soap.md) <br/> |Представляет свойство [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) .  <br/> |
|[Маилтипсакцессенаблед (SOAP)](mailtipsaccessenabled-soap.md) <br/> |Представляет флаг [маилтипсакцессенаблед ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) .  <br/> |
|[MailTipsAccessLevel (SOAP)](mailtipsaccesslevel-soap.md) <br/> |Представляет свойство [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) .  <br/> |
|[Маилбоксмовинаблед (SOAP)](mailboxmoveenabled-soap.md) <br/> |Представляет флаг [маилбоксмовинаблед ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) .  <br/> |
|[Имя (SOAP)](name-soap.md) <br/> |Представляет имя связи Организации.  <br/> |
|[Таржетаппликатионури (SOAP)](targetapplicationuri-soap.md) <br/> |Определяет универсальный код ресурса (URI) конечного приложения.  <br/> |
|[Таржетаутодисковерепр (SOAP)](targetautodiscoverepr-soap.md) <br/> |Представляет свойство [таржетаутодисковерепр](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) .  <br/> |
|[Таржетшаринжепр (SOAP)](targetsharingepr-soap.md) <br/> |Представляет свойство [таржетшаринжепр](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Организатионрелатионшипсеттингсколлектион (SOAP)](organizationrelationshipsettingscollection-soap.md) <br/> |Представляет список отношений Организации, которые совпадают с запросом.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Отсутствуют.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   

