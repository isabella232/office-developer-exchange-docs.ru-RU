---
title: Анонимаусакцессалловед (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: bf819a65-30f2-4881-a34f-cb30a9c2b6a7
description: Элемент Анонимаусакцессалловед указывает, требуется ли для расположения общего доступа к документу пользователь, прошедший проверку подлинности.
ms.openlocfilehash: b3ff22fbba603bbd74dc08a0dbb1d8687714fe7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466082"
---
# <a name="anonymousaccessallowed-soap"></a>Анонимаусакцессалловед (SOAP)

Элемент **анонимаусакцессалловед** указывает, требуется ли для расположения общего доступа к документу пользователь, прошедший проверку подлинности. 
  
```XML
<AnonymousAccessAllowed /> 
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Документшаринглокатион (SOAP)](documentsharinglocation-soap.md) <br/> |Представляет сведения о местоположении и метаданных для расположения общего доступа к документу.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Логическое значение элемента **анонимаусакцессалловед** указывает, требуется ли для расположения для общего доступа пользователь, прошедший проверку подлинности. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|Имя схемы  <br/> |Схема автообнаружения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |True  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetUserSettings (SOAP)](getusersettings-operation-soap.md)
- [Справочные материалы по веб-службе автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)
- [XML-элементы автообнаружения SOAP для Exchange 2013](soap-autodiscover-xml-elements-for-exchange-2013.md)

