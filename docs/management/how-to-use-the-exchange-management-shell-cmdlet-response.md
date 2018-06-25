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
# <a name="use-the-exchange-management-shell-cmdlet-response"></a><span data-ttu-id="e0c73-103">Использование ответа командлет командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="e0c73-103">Use the Exchange Management Shell cmdlet response</span></span>

<span data-ttu-id="e0c73-104">Узнайте, как использовать ответ от это командлет командной консоли Exchange в Exchange управляемые приложения.</span><span class="sxs-lookup"><span data-stu-id="e0c73-104">Learn how to use the response from an Exchange Management Shell cmdlet in your Exchange managed application.</span></span>
  
<span data-ttu-id="e0c73-105">**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="e0c73-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="e0c73-106">Каждый командной консоли Exchange командлет возвращает один или несколько экземпляров [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) , которые обеспечивают согласованность представление какого-либо объекта в среде управления Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0c73-106">Each Exchange Management Shell cmdlet returns one or more [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) instances that provide a consistent view of any object in the Exchange Management Shell environment.</span></span> <span data-ttu-id="e0c73-107">В этой статье представлены сведения об использовании свойства экземпляра **PSObject** для возврата значения свойств базового объекта Exchange Server 2013 API.</span><span class="sxs-lookup"><span data-stu-id="e0c73-107">This article provides information about how to use the properties of a **PSObject** instance to return the property values of the underlying Exchange Server 2013 API object.</span></span> 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a><span data-ttu-id="e0c73-108">Необходимые условия для использования командлета ответы</span><span class="sxs-lookup"><span data-stu-id="e0c73-108">Prerequisites for using cmdlet responses</span></span>
<span data-ttu-id="e0c73-109"><a name="prerequisites_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="e0c73-109"></span></span>

<span data-ttu-id="e0c73-110">Чтобы использовать командлет ответов, требуется ссылку на пространство имен **System.Automation.Management** .</span><span class="sxs-lookup"><span data-stu-id="e0c73-110">To use cmdlet responses, you need a reference to the **System.Automation.Management** namespace.</span></span> 
  
> [!NOTE]
>  <span data-ttu-id="e0c73-111">Если вы используете Visual Studio для создания приложения, необходимо добавить ссылку на сборку System.Mangagement.Automation.dll в проект.</span><span class="sxs-lookup"><span data-stu-id="e0c73-111">When you are using Visual Studio to create an application, you must add a reference to the System.Mangagement.Automation.dll assembly to the project.</span></span> <span data-ttu-id="e0c73-112">Сборки можно найти в одном из следующих расположений:</span><span class="sxs-lookup"><span data-stu-id="e0c73-112">You can find the assembly in one of the following locations:</span></span> 
> - <span data-ttu-id="e0c73-113">Для ОС Windows XP и Windows Vista — каталог установки Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="e0c73-113">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span> 
> - <span data-ttu-id="e0c73-114">Для ОС Windows 7 и Windows 8 — папка Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="e0c73-114">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
## <a name="windows-powershell-remote-runspace"></a><span data-ttu-id="e0c73-115">Удаленный рабочей среде Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="e0c73-115">Windows PowerShell remote runspace</span></span>
<span data-ttu-id="e0c73-116"><a name="usingremoterunspace_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="e0c73-116"></span></span>

<span data-ttu-id="e0c73-117">Командная консоль Exchange использует удаленных компонентов Windows PowerShell для всех команд, даже команды, которые выполняются на локальном сервере.</span><span class="sxs-lookup"><span data-stu-id="e0c73-117">The Exchange Management Shell uses remote Windows PowerShell features for all commands, even commands that are run on the local server.</span></span> <span data-ttu-id="e0c73-118">В результате все ответы из командной консоли Exchange, командлеты сериализованным XML.</span><span class="sxs-lookup"><span data-stu-id="e0c73-118">As a result, all responses from Exchange Management Shell cmdlets are serialized XML.</span></span> <span data-ttu-id="e0c73-119">Это означает, что несмотря на то, что объект ответа указывает тип объекта Exchange, который использовался для создания ответа, объект ответа не может быть приведен к типу объекта Exchange; Вместо этого необходимо использовать контейнер свойств, предоставляемые элементом объект ответа для получения значений из типа объекта Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0c73-119">This means that although the response object indicates the Exchange object type that was used to generate the response, the response object cannot be cast to the Exchange object type; instead, you must use the property bag that is exposed by the response object to obtain the values from the Exchange object type.</span></span>
  
<span data-ttu-id="e0c73-120">Контейнер свойств в объекте ответа содержит пары ключ значение для каждого открытое свойство или метод в тип объекта Exchange.</span><span class="sxs-lookup"><span data-stu-id="e0c73-120">The property bag in the response object contains a key/value pair for each public property or method in the Exchange object type.</span></span> <span data-ttu-id="e0c73-121">Объект ответа содержит имя базового типа объекта Exchange; Это имя можно использовать для определения типа объекта Exchange, представленного объектом ответа таким образом, вы можете извлечь соответствующего свойства.</span><span class="sxs-lookup"><span data-stu-id="e0c73-121">The response object contains the name of the underlying Exchange object type; you can use this name to determine the Exchange object type that is represented by the response object so that you can extract the appropriate property.</span></span> <span data-ttu-id="e0c73-122">Каждое значение в контейнере свойств также содержит сведения о типе, поэтому можно привести значение свойства соответствующий управляемый тип.</span><span class="sxs-lookup"><span data-stu-id="e0c73-122">Each value in the property bag also includes type information so that you can cast the property value to the appropriate managed type.</span></span>
  
## <a name="use-the-cmdlet-response"></a><span data-ttu-id="e0c73-123">Используйте командлет ответа</span><span class="sxs-lookup"><span data-stu-id="e0c73-123">Use the cmdlet response</span></span>
<span data-ttu-id="e0c73-124"><a name="usingPSObject_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="e0c73-124"></span></span>

<span data-ttu-id="e0c73-125">Класс [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) предоставляет следующие три общих свойств, содержащих значения базового объекта Exchange 2013 API: [Свойства](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [методы](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx)и [члены](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e0c73-125">The [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) class exposes the following three public properties that contain the values of the underlying Exchange 2013 API object: [Properties](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [Methods](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx), and [Members](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span></span> <span data-ttu-id="e0c73-126">Каждого свойства, предоставляемые объектом Exchange 2013 API имеет соответствующий пары ключ значение в окне Свойства **Свойства** и **его элементы** .</span><span class="sxs-lookup"><span data-stu-id="e0c73-126">Each property that is exposed by the Exchange 2013 API object has a corresponding key/value pair in the **Properties** and **Members** properties.</span></span> <span data-ttu-id="e0c73-127">Приложения можно проиндексировать коллекции **свойств** , имя свойства для извлечения значения свойства.</span><span class="sxs-lookup"><span data-stu-id="e0c73-127">Your application can index the **Properties** collection by the name of a property to retrieve the value of the property.</span></span> 
  
<span data-ttu-id="e0c73-128">Свойство **TypeNames** экземпляра **PSObject** можно использовать для определения типа базовый объект Exchange, инкапсулированную в экземпляре **PSObject** .</span><span class="sxs-lookup"><span data-stu-id="e0c73-128">You can use the **TypeNames** property of the **PSObject** instance to determine the type of the underlying Exchange object that is encapsulated by the **PSObject** instance.</span></span> <span data-ttu-id="e0c73-129">Свойство **TypeNames** — это набор строк, содержащий иерархии объектов представленного типа.</span><span class="sxs-lookup"><span data-stu-id="e0c73-129">The **TypeNames** property is a collection of strings that contains the object hierarchy of the represented type.</span></span> <span data-ttu-id="e0c73-130">Эти имена можно использовать для определения объектов, представленный в экземпляре **PSObject** таким образом, вы можете извлекать соответствующее свойство.</span><span class="sxs-lookup"><span data-stu-id="e0c73-130">You can use these names to determine the object that is represented by the **PSObject** instance so that you can extract the appropriate property.</span></span> 
  
<span data-ttu-id="e0c73-131">В следующем примере кода используется командлет ответа для печати содержимое коллекции **свойств** экземпляра **PSObject** на консоль.</span><span class="sxs-lookup"><span data-stu-id="e0c73-131">The following code example uses the cmdlet response to print the contents of the **Properties** collection of a **PSObject** instance on the console.</span></span> <span data-ttu-id="e0c73-132">В примере требуется ссылка на пространство имен **System.Automation.Management** .</span><span class="sxs-lookup"><span data-stu-id="e0c73-132">The code example requires a reference to the **System.Automation.Management** namespace.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="e0c73-133">См. также</span><span class="sxs-lookup"><span data-stu-id="e0c73-133">See also</span></span>

- [<span data-ttu-id="e0c73-134">Создание средств управления Exchange</span><span class="sxs-lookup"><span data-stu-id="e0c73-134">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="e0c73-135">Ознакомьтесь со списком пользователей почты с помощью командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="e0c73-135">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

