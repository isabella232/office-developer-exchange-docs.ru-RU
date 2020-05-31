---
title: Документшаринглокатион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 21bc388c-33be-422b-a89d-30ade0fae8f1
description: Элемент Документшаринглокатион содержит сведения о расположении и метаданных расположения для общего доступа к документу.
ms.openlocfilehash: d258efecb46d570138c7c2c78ed9d2fa9a275103
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762198"
---
# <a name="documentsharinglocation-soap"></a>Документшаринглокатион (SOAP)

Элемент **документшаринглокатион** содержит сведения о расположении и метаданных расположения для общего доступа к документу. 
  
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

 **документшаринглокатион**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Сервицеурл (SOAP)](serviceurl-soap.md) <br/> |Представляет URL-адрес веб-службы общего доступа к документам.  <br/> |
|[Локатионурл (SOAP)](locationurl-soap.md) <br/> |Представляет URL-адрес расположения общего доступа к документу.  <br/> |
|[DisplayName (SOAP)](displayname-soap.md) <br/> |Представляет имя расположения для общего доступа к документу, которое будет использоваться в пользовательском интерфейсе.  <br/> |
|[Суппортедфиликстенсионс (SOAP)](supportedfileextensions-soap.md) <br/> |Представляет расширения файлов, которые могут храниться в расположении общего доступа к документам.  <br/> |
|[Екстерналакцессалловед (SOAP)](externalaccessallowed-soap.md) <br/> |Указывает, доступно ли расположение для общего доступа к документу для внешнего подключения.  <br/> |
|[Анонимаусакцессалловед (SOAP)](anonymousaccessallowed-soap.md) <br/> |Указывает, требуется ли пользователю, прошедшему проверку подлинности, доступ к общему ресурсу.  <br/> |
|[Канмодифипермиссионс (SOAP)](canmodifypermissions-soap.md) <br/> |Указывает, может ли пользователь изменять разрешения доступа к расположению общего доступа к документам.  <br/> |
|[По умолчанию (SOAP)](isdefault-soap.md) <br/> |Указывает, является ли расположение общего доступа к документу общим расположением пользователя по умолчанию.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Документшаринглокатионс (SOAP)](documentsharinglocations-soap.md) <br/> |Содержит список расположений и метаданных общего доступа к документам.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Справочные материалы по веб-службе автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [XML-элементы автообнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

