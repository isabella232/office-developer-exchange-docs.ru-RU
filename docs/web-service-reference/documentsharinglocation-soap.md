---
title: DocumentSharingLocation (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: Элемент DocumentSharingLocation содержит местоположение и сведения о метаданных для общего доступа к расположение документа.
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762198"
---
# <a name="documentsharinglocation-soap"></a>DocumentSharingLocation (SOAP)

Элемент **DocumentSharingLocation** содержит местоположение и сведения о метаданных для общего доступа к расположение документа. 
  
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
|[ServiceUrl (SOAP)](serviceurl-soap.md) <br/> |Представляет URL-адрес документа, общий доступ к веб-службе.  <br/> |
|[LocationUrl (SOAP)](locationurl-soap.md) <br/> |Представляет URL-адрес документа, общий доступ к расположения.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Представляет имя документа, общий доступ к папка, которая используется в пользовательском Интерфейсе.  <br/> |
|[SupportedFileExtensions (SOAP)](supportedfileextensions-soap.md) <br/> |Представляет расширений файлов, которые могут храниться в документе общего ресурса.  <br/> |
|[ExternalAccessAllowed (SOAP)](externalaccessallowed-soap.md) <br/> |Указывает, является ли документ, общий доступ к расположение доступны за пределами подключений.  <br/> |
|[AnonymousAccessAllowed (SOAP)](anonymousaccessallowed-soap.md) <br/> |Указывает, требуется ли доступ к месту общего доступа пользователя с разрешением.  <br/> |
|[CanModifyPermissions (SOAP)](canmodifypermissions-soap.md) <br/> |Указывает, является ли пользователь может изменить разрешения на доступ к документу общего ресурса.  <br/> |
|[IsDefault (SOAP)](isdefault-soap.md) <br/> |Указывает, является ли документ, общий доступ к расположение общего доступа расположение по умолчанию для пользователя.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[DocumentSharingLocations (SOAP)](documentsharinglocations-soap.md) <br/> |Содержит список документов, совместное использование расположения и метаданных.  <br/> |
   
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

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [Элементы XML автоматического обнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

