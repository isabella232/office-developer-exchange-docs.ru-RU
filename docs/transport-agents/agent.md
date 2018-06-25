---
title: агент
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
description: 'Последнее изменение: 17 сентября 2015'
ms.openlocfilehash: 3895095ed4e469cdb9fec489ba6b6e228779a9c8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761286"
---
# <a name="agent"></a>агент
  
**Применимо к:** Exchange Server 2013
  
Элемент **агента** содержит сведения о конфигурации об установленных агентов. 
  
- [Конфигурация](configuration.md) 
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
|**name** <br/> |Имя, которое было указано при установке агента. Этот атрибут иметь значение пустая строка, которая содержит не более 64 символов.  <br/> |
|**baseType** <br/> |Полное имя, включая пространства имен, класса, от которого наследует агент. Этот атрибут иметь значение пустая строка, которая содержит по крайней мере один знак.  <br/> |
|**classFactory** <br/> |Полное имя, включая пространство имен, класс, реализующий фабрика агентов, который создает экземпляры агента. Этот атрибут должен содержать полное имя класса, реализующего фабрика агентов, который создает экземпляры агента. Этот класс должен наследовать от класса либо [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) , либо [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .  <br/> |
|**путь _ сборки** <br/> |Полный путь, включая имя файла сборки, которая содержит код для агента. Этот атрибут иметь значение пустая строка, которая содержит по крайней мере один знак.  <br/> |
|**включено** <br/> |Логическое значение, указывающее, включено ли агент. Значение равно **true** , если включена агент. в противном случае — значение **false**. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[agentList](agentlist.md) <br/> |Содержит элемент **агентов** для каждого установленного агента.  <br/> |
   
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |Этот файл не определяет пространство имен.  <br/> |
|Имя схемы  <br/> |Компонент недоступен.  <br/> |
|Файл проверки  <br/> |Компонент недоступен.  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы файла конфигурации агентов для Exchange 2013](agents-configuration-file-elements-for-exchange-2013.md)

