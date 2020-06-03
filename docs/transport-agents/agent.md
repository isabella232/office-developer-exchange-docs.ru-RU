---
title: агента
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Дата последнего изменения: 17 сентября 2015 г.'
ms.openlocfilehash: a810bb229015054e0f244773760235114655a982
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455683"
---
# <a name="agent"></a>агента
  
**Применимо к:** Exchange Server 2013
  
Элемент **Agent** содержит сведения о конфигурации установленного агента. 
  
- [configuration](configuration.md) 
- [мексрунтиме](mexruntime.md)
- [ажентлист](agentlist.md)
- [агента](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

**Аженттипе (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**name** <br/> |Имя, указанное при установке агента. Для этого атрибута требуется непустое строковое значение, содержащее не более 64 символов.  <br/> |
|**baseType** <br/> |Полное имя класса, который является производным от агента, включая пространство имен. Для этого атрибута требуется непустое строковое значение, содержащее по крайней мере один символ.  <br/> |
|**классфактори** <br/> |Полное имя (включая пространство имен) класса, который реализует фабрику агентов, которая создает экземпляры агента. Этот атрибут должен содержать полное имя класса, реализующего фабрику агентов, которая создает экземпляры агента. Этот класс должен быть производным от класса [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) или [раутингажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .  <br/> |
|**Путь** <br/> |Полный путь, включая имя файла сборки, содержащей код для агента. Для этого атрибута требуется непустое строковое значение, содержащее по крайней мере один символ.  <br/> |
|**enabled** <br/> |Логическое значение, которое указывает, включен ли агент. Значение **true** , если агент включен; в противном случае — значение **false**. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ажентлист](agentlist.md) <br/> |Содержит элемент **Agent** для каждого установленного агента.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Namespace  <br/> |В этом файле не определено пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

