---
title: Использование ответа командлет командной консоли Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Узнайте, как использовать ответ от это командлет командной консоли Exchange в Exchange управляемые приложения.
ms.openlocfilehash: 5edf75afd556f67e815bc519c87586f2f62f057b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761252"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Использование ответа командлет командной консоли Exchange

Узнайте, как использовать ответ от это командлет командной консоли Exchange в Exchange управляемые приложения.
  
**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365
  
Каждый командной консоли Exchange командлет возвращает один или несколько экземпляров [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) , которые обеспечивают согласованность представление какого-либо объекта в среде управления Exchange. В этой статье представлены сведения об использовании свойства экземпляра **PSObject** для возврата значения свойств базового объекта Exchange Server 2013 API. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Необходимые условия для использования командлета ответы
<a name="prerequisites_bk"> </a>

Чтобы использовать командлет ответов, требуется ссылку на пространство имен **System.Automation.Management** . 
  
> [!NOTE]
>  Если вы используете Visual Studio для создания приложения, необходимо добавить ссылку на сборку System.Mangagement.Automation.dll в проект. Сборки можно найти в одном из следующих расположений: 
> - Для ОС Windows XP и Windows Vista — каталог установки Windows PowerShell ($PSHOME). 
> - Для ОС Windows 7 и Windows 8 — папка Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Удаленный рабочей среде Windows PowerShell
<a name="usingremoterunspace_bk"> </a>

Командная консоль Exchange использует удаленных компонентов Windows PowerShell для всех команд, даже команды, которые выполняются на локальном сервере. В результате все ответы из командной консоли Exchange, командлеты сериализованным XML. Это означает, что несмотря на то, что объект ответа указывает тип объекта Exchange, который использовался для создания ответа, объект ответа не может быть приведен к типу объекта Exchange; Вместо этого необходимо использовать контейнер свойств, предоставляемые элементом объект ответа для получения значений из типа объекта Exchange.
  
Контейнер свойств в объекте ответа содержит пары ключ значение для каждого открытое свойство или метод в тип объекта Exchange. Объект ответа содержит имя базового типа объекта Exchange; Это имя можно использовать для определения типа объекта Exchange, представленного объектом ответа таким образом, вы можете извлечь соответствующего свойства. Каждое значение в контейнере свойств также содержит сведения о типе, поэтому можно привести значение свойства соответствующий управляемый тип.
  
## <a name="use-the-cmdlet-response"></a>Используйте командлет ответа
<a name="usingPSObject_bk"> </a>

Класс [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) предоставляет следующие три общих свойств, содержащих значения базового объекта Exchange 2013 API: [Свойства](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [методы](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx)и [члены](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx). Каждого свойства, предоставляемые объектом Exchange 2013 API имеет соответствующий пары ключ значение в окне Свойства **Свойства** и **его элементы** . Приложения можно проиндексировать коллекции **свойств** , имя свойства для извлечения значения свойства. 
  
Свойство **TypeNames** экземпляра **PSObject** можно использовать для определения типа базовый объект Exchange, инкапсулированную в экземпляре **PSObject** . Свойство **TypeNames** — это набор строк, содержащий иерархии объектов представленного типа. Эти имена можно использовать для определения объектов, представленный в экземпляре **PSObject** таким образом, вы можете извлекать соответствующее свойство. 
  
В следующем примере кода используется командлет ответа для печати содержимое коллекции **свойств** экземпляра **PSObject** на консоль. В примере требуется ссылка на пространство имен **System.Automation.Management** . 
  
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

- [Создание средств управления Exchange](create-exchange-management-shell-tools.md)   
- [Ознакомьтесь со списком пользователей почты с помощью командной консоли Exchange](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

