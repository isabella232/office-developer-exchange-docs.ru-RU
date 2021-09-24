---
title: agent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- agent
api_type:
- schema
ms.assetid: 0bf744a5-9d79-4c82-8ea7-45fdb3f55300
description: 'Последнее изменение: 17 сентября 2015 г.'
ms.openlocfilehash: 8bcfdd9bffd4c7a15af40528fd431a99c7868637
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520970"
---
# <a name="agent"></a>agent
  
**Применяется к:** Exchange Server 2013 г.
  
Элемент **агента** содержит сведения о конфигурации установленного агента. 
  
- [configuration](configuration.md) 
- [mexRuntime](mexruntime.md)
- [agentList](agentlist.md)
- [агент](agent.md)
  
```XML
<agent
        name=""
        baseType=""
        classFactory=""
        assemblyPath=""
        enabled="" />
</agent>
```

**agentType (complexType)**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**name** <br/> |Имя, указанное при установке агента. Этот атрибут требует несущестного значения строки, которое содержит не более 64 символов.  <br/> |
|**baseType** <br/> |Полное имя, в том числе пространство имен класса, из которого происходит агент. Этот атрибут требует несущестного значения строки, которое содержит по крайней мере один символ.  <br/> |
|**classFactory** <br/> |Полное имя, в том числе пространство имен класса, реализуемого фабрикой агентов, создав экземпляры агента. Этот атрибут должен содержать полностью квалифицированное имя класса, реализуемого фабрикой агентов, создав экземпляры агента. Этот класс должен исходить из класса [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) или [RoutingAgentFactory.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)  <br/> |
|**assemblyPath** <br/> |Полностью квалифицированный путь, включая имя файла, сборки, которая содержит код агента. Этот атрибут требует несущестного значения строки, которое содержит по крайней мере один символ.  <br/> |
|**enabled** <br/> |Значение Boolean, которое указывает, включен ли агент. Значение **верно, если** включен агент; в противном случае значение является **ложным.** Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |Содержит элемент **агента** для каждого установленного агента.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Недоступно.  <br/> |
|Файл проверки  <br/> |Недоступно.  <br/> |
|Может быть пустым  <br/> |Неверно.  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы конфигурации файлов агентов для Exchange 2013 г.](agents-configuration-file-elements-for-exchange-2013.md)

