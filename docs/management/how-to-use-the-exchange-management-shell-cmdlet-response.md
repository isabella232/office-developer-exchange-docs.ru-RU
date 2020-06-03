---
title: Использование ответа командлета командной консоли Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Узнайте, как использовать ответ командлета командной консоли Exchange в управляемом приложении Exchange.
ms.openlocfilehash: c1b81356ab5dc288ab08287d47581871c36beb05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435704"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Использование ответа командлета командной консоли Exchange

Узнайте, как использовать ответ командлета командной консоли Exchange в управляемом приложении Exchange.
  
**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365
  
Каждый командлет командной консоли Exchange возвращает один или несколько экземпляров [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) , которые предоставляют согласованное представление любого объекта в среде командной консоли Exchange. В этой статье приводятся сведения о том, как использовать свойства экземпляра **PSObject** для возврата значений свойств базового объекта API сервера Exchange Server 2013. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Предварительные требования для использования ответов командлетов
<a name="prerequisites_bk"> </a>

Чтобы использовать ответы командлетов, вам потребуется ссылка на пространство имен **System. Automation. Management** . 
  
> [!NOTE]
>  При создании приложения с помощью Visual Studio необходимо добавить в проект ссылку на сборку System. Мангажемент. Automation. dll. Сборку можно найти в одном из следующих расположений: 
> - Для ОС Windows XP и Windows Vista — каталог установки Windows PowerShell ($PSHOME). 
> - Для ОС Windows 7 и Windows 8 — папка Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Удаленное пространство выполнения Windows PowerShell
<a name="usingremoterunspace_bk"> </a>

Командная консоль Exchange использует удаленные функции Windows PowerShell для всех команд, даже команд, выполняемых на локальном сервере. В результате все ответы от командлетов командной консоли Exchange сериализуются в XML. Это означает, что несмотря на то, что объект Response указывает тип объекта Exchange, который использовался для создания ответа, объект Response не может быть приведен к типу объекта Exchange; Вместо этого необходимо использовать контейнер свойств, предоставленный объектом Response для получения значений из типа объекта Exchange.
  
Контейнер свойств в объекте Response содержит набор ключей и значений для каждого общедоступного свойства или метода в типе объекта Exchange. Объект Response содержит имя базового типа объекта Exchange; Это имя можно использовать для определения типа объекта Exchange, представленного объектом Response, чтобы можно было извлечь соответствующее свойство. Каждое значение в контейнере свойств также включает сведения о типе, чтобы можно было привести значение свойства к соответствующему управляемому типу.
  
## <a name="use-the-cmdlet-response"></a>Использование ответа командлета
<a name="usingPSObject_bk"> </a>

Класс [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) предоставляет следующие три общедоступные свойства, которые содержат значения базового объекта API Exchange 2013: [Свойства](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [методы](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx)и [элементы](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx). Каждое свойство, предоставляемое объектом API Exchange 2013, имеет соответствующую запись key/value в свойствах **Properties** и **Members** . Приложение может индексировать коллекцию **свойств** по имени свойства, чтобы получить значение свойства. 
  
Свойство **typenames** экземпляра **PSObject** можно использовать для определения типа базового объекта Exchange, который инкапсулируется экземпляром **PSObject** . Свойство **typenames** — это коллекция строк, которая содержит иерархию объектов представленного типа. С помощью этих имен можно определить объект, представленный экземпляром **PSObject** , чтобы можно было извлечь соответствующее свойство. 
  
В следующем примере кода используется ответ командлета для вывода содержимого коллекции **свойств** экземпляра **PSObject** в консоли. В этом примере кода требуется ссылка на пространство имен **System. Automation. Management** . 
  
```cs
foreach (PSPropertyInfo propertyInfo in psObject.Properties)
{
    Console.WriteLine(string.Format("{0}: {1}",
        propertyInfo.Name, propertyInfo.Value);
}
```

<br/>

```vb
For Each PropertyInfo As PSProperty In ObjectInfo.Properties
    Console.WriteLine(String.Format("{0}: {1}", PropertyInfo.Name, PropertyInfo.Value))
Next

```

## <a name="see-also"></a>См. также

- [Создание средств командной консоли Exchange](create-exchange-management-shell-tools.md)   
- [Получение списка пользователей почты с помощью командной консоли Exchange](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

