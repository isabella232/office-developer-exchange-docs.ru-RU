---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: Элемент DocumentSharingLocation содержит сведения о расположении и метаданных для расположения общего доступа к документам.
ms.openlocfilehash: f4011dfb846d314d926ba644f4ddc2176283008a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541485"
---
# <a name="documentsharinglocation-soap"></a>DocumentSharingLocation (SOAP)

Элемент **DocumentSharingLocation содержит** сведения о расположении и метаданных для расположения общего доступа к документам. 
  
```XML
<DocumentSharingLocation>
   <ServiceUrl />
   <LocationUrl />
   <DisplayName />
   <SupportedFileExtensions />
   <ExternalAccessAllowed />
   <AnonymousAccessAllowed />
   <CanModifyPermissions />
   <IsDefault />
</DocumentSharingLocation>
```

 **DocumentSharingLocation**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ServiceUrl (SOAP)](serviceurl-soap.md) <br/> |Представляет URL-адрес веб-службы общего доступа к документам.  <br/> |
|[LocationUrl (SOAP)](locationurl-soap.md) <br/> |Представляет URL-адрес расположения общего доступа к документам.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Представляет имя расположения общего доступа к документам, используемого в пользовательском интерфейсе.  <br/> |
|[SupportedFileExtensions (SOAP)](supportedfileextensions-soap.md) <br/> |Представляет расширения файлов, которые можно хранить в расположении общего доступа к документам.  <br/> |
|[ExternalAccessAllowed (SOAP)](externalaccessallowed-soap.md) <br/> |Указывает, доступно ли расположение общего доступа к документам внешним подключениям.  <br/> |
|[AnonymousAccessAllowed (SOAP)](anonymousaccessallowed-soap.md) <br/> |Указывает, требуется ли доступ к расположению общего доступа пользователю, который имеет проверку подлинности.  <br/> |
|[CanModifyPermissions (SOAP)](canmodifypermissions-soap.md) <br/> |Указывает, может ли пользователь изменять разрешения доступа к расположению общего доступа к документам.  <br/> |
|[IsDefault (SOAP)](isdefault-soap.md) <br/> |Указывает, является ли расположение общего доступа к документам расположением общего доступа пользователя по умолчанию.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |Содержит список местоположений и метаданных общего доступа к документам.  <br/> |
   
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

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Ссылка на веб-службу автооткрытия для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Элементы XML автооткрытия SOAP для Exchange 2013 г.](soap-autodiscover-xml-elements-for-exchange-2013.md)

