---
title: Используйте ответ команды Exchange Management Shell
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: dac8e526-11c6-4c2e-b9a2-f016b1fc738a
description: Узнайте, как использовать ответ из команды Exchange в управляемом приложении Exchange.
ms.openlocfilehash: be66be31e435be1553eba16d8f367a79317618f2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520966"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a>Используйте ответ команды Exchange Management Shell

Узнайте, как использовать ответ из команды Exchange в управляемом приложении Exchange.
  
**Применяется к:** Exchange Online | Exchange Server 2013 | Office 365
  
Каждый Exchange команды Management Shell возвращает один или несколько экземпляров [PSObject,](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) которые обеспечивают согласованное представление любого объекта в среде Exchange Management Shell. В этой статье данная статья содержит сведения об использовании свойств экземпляра **PSObject** для возврата значений свойств объекта API Exchange Server 2013 г. 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a>Необходимые условия для использования ответов на cmdlet
<a name="prerequisites_bk"> </a>

Чтобы использовать ответы на команды, вам потребуется ссылка на пространство имен **System.Automation.Management.** 
  
> [!NOTE]
>  При использовании Visual Studio для создания приложения необходимо добавить ссылку на сборку System.Mangagement.Automation.dll в проект. Сборку можно найти в одном из следующих местоположений: 
> - Для ОС Windows XP и Windows Vista — каталог установки Windows PowerShell ($PSHOME). 
> - Для ОС Windows 7 и Windows 8 — папка Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
## <a name="windows-powershell-remote-runspace"></a>Windows PowerShell пространства удаленного запуска
<a name="usingremoterunspace_bk"> </a>

В Exchange management Shell используются удаленные Windows PowerShell для всех команд, даже команд, которые запускаются на локальном сервере. В результате все ответы из Exchange Management Shell будут сериализованы по XML. Это означает, что, хотя объект отклика указывает тип объекта Exchange, который был использован для создания ответа, объект ответа не может быть отлит в Exchange объекта; Вместо этого необходимо использовать пакет свойств, который подвергается объекту ответа, для получения значений из Exchange объекта.
  
Пакет свойств в объекте ответа содержит пару ключей и значений для каждого общего свойства или метода Exchange объекта. Объект ответа содержит имя Exchange объекта; Это имя можно использовать для определения типа Exchange объекта, представленного объектом отклика, чтобы можно было извлечь соответствующее свойство. Каждое значение в пакете свойств также включает сведения о типе, чтобы можно было перенаправить значение свойства в соответствующий управляемый тип.
  
## <a name="use-the-cmdlet-response"></a>Использование отклика командлета
<a name="usingPSObject_bk"> </a>

Класс [PSObject](https://msdn.microsoft.com/library/system.management.automation.psobject%28VS.85%29.aspx) предоставляет следующие три общедоступных свойства, которые содержат значения объекта API 2013 Exchange 2013 [года:](https://msdn.microsoft.com/library/system.management.automation.psobject.properties%28VS.85%29.aspx) [Свойства,](https://msdn.microsoft.com/library/system.management.automation.psobject.methods%28VS.85%29.aspx)методы и члены [.](https://msdn.microsoft.com/library/system.management.automation.psobject.members%28VS.85%29.aspx) Каждое свойство, выставленное объектом API Exchange 2013 г., имеет соответствующую пару ключей и значений в свойствах **Свойств** **и** Членов. Приложение может индексировать коллекцию **свойств** по имени свойства, чтобы получить значение свойства. 
  
Свойство **TypeNames** экземпляра **PSObject** можно использовать для определения типа Exchange объекта, инкапсулированного экземпляром **PSObject.** Свойство **TypeNames** — это коллекция строк, которая содержит объектную иерархию представленного типа. Эти имена можно использовать для определения объекта, представленного экземпляром **PSObject,** чтобы можно было извлечь соответствующее свойство. 
  
В следующем примере кода для печати **содержимого** коллекции свойств экземпляра **PSObject** на консоли используется ответ на cmdlet. В примере кода требуется ссылка на пространство **имен System.Automation.Management.** 
  
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

- [Создание инструментов командной консоли Exchange](create-exchange-management-shell-tools.md)   
- [Получить список пользователей почты с помощью Exchange shell](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

