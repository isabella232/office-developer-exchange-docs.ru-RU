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
ms.openlocfilehash: 5edf75afd556f67e815bc519c87586f2f62f057b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761252"
---
# <a name="use-the-exchange-management-shell-cmdlet-response"></a><span data-ttu-id="d5edf-103">Использование ответа командлета командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="d5edf-103">Use the Exchange Management Shell cmdlet response</span></span>

<span data-ttu-id="d5edf-104">Узнайте, как использовать ответ командлета командной консоли Exchange в управляемом приложении Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5edf-104">Learn how to use the response from an Exchange Management Shell cmdlet in your Exchange managed application.</span></span>
  
<span data-ttu-id="d5edf-105">**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365</span><span class="sxs-lookup"><span data-stu-id="d5edf-105">**Applies to:** Exchange Online | Exchange Server 2013 | Office 365</span></span>
  
<span data-ttu-id="d5edf-106">Каждый командлет командной консоли Exchange возвращает один или несколько экземпляров [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) , которые предоставляют согласованное представление любого объекта в среде командной консоли Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5edf-106">Each Exchange Management Shell cmdlet returns one or more [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) instances that provide a consistent view of any object in the Exchange Management Shell environment.</span></span> <span data-ttu-id="d5edf-107">В этой статье приводятся сведения о том, как использовать свойства экземпляра **PSObject** для возврата значений свойств базового объекта API сервера Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d5edf-107">This article provides information about how to use the properties of a **PSObject** instance to return the property values of the underlying Exchange Server 2013 API object.</span></span> 
  
## <a name="prerequisites-for-using-cmdlet-responses"></a><span data-ttu-id="d5edf-108">Предварительные требования для использования ответов командлетов</span><span class="sxs-lookup"><span data-stu-id="d5edf-108">Prerequisites for using cmdlet responses</span></span>
<span data-ttu-id="d5edf-109"><a name="prerequisites_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="d5edf-109"><a name="prerequisites_bk"> </a></span></span>

<span data-ttu-id="d5edf-110">Чтобы использовать ответы командлетов, вам потребуется ссылка на пространство имен **System. Automation. Management** .</span><span class="sxs-lookup"><span data-stu-id="d5edf-110">To use cmdlet responses, you need a reference to the **System.Automation.Management** namespace.</span></span> 
  
> [!NOTE]
>  <span data-ttu-id="d5edf-111">При создании приложения с помощью Visual Studio необходимо добавить в проект ссылку на сборку System. Мангажемент. Automation. dll.</span><span class="sxs-lookup"><span data-stu-id="d5edf-111">When you are using Visual Studio to create an application, you must add a reference to the System.Mangagement.Automation.dll assembly to the project.</span></span> <span data-ttu-id="d5edf-112">Сборку можно найти в одном из следующих расположений:</span><span class="sxs-lookup"><span data-stu-id="d5edf-112">You can find the assembly in one of the following locations:</span></span> 
> - <span data-ttu-id="d5edf-113">Для ОС Windows XP и Windows Vista — каталог установки Windows PowerShell ($PSHOME).</span><span class="sxs-lookup"><span data-stu-id="d5edf-113">For Windows XP and Windows Vista operating systems, the Windows PowerShell installation directory ($PSHOME).</span></span> 
> - <span data-ttu-id="d5edf-114">Для ОС Windows 7 и Windows 8 — папка Windows\assembly\GAC_MSIL\System.Management.Automation.</span><span class="sxs-lookup"><span data-stu-id="d5edf-114">For the Windows 7 and Windows 8 operating systems, the following folder: Windows\assembly\GAC_MSIL\System.Management.Automation.</span></span> 
  
## <a name="windows-powershell-remote-runspace"></a><span data-ttu-id="d5edf-115">Удаленное пространство выполнения Windows PowerShell</span><span class="sxs-lookup"><span data-stu-id="d5edf-115">Windows PowerShell remote runspace</span></span>
<span data-ttu-id="d5edf-116"><a name="usingremoterunspace_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="d5edf-116"><a name="usingremoterunspace_bk"> </a></span></span>

<span data-ttu-id="d5edf-117">Командная консоль Exchange использует удаленные функции Windows PowerShell для всех команд, даже команд, выполняемых на локальном сервере.</span><span class="sxs-lookup"><span data-stu-id="d5edf-117">The Exchange Management Shell uses remote Windows PowerShell features for all commands, even commands that are run on the local server.</span></span> <span data-ttu-id="d5edf-118">В результате все ответы от командлетов командной консоли Exchange сериализуются в XML.</span><span class="sxs-lookup"><span data-stu-id="d5edf-118">As a result, all responses from Exchange Management Shell cmdlets are serialized XML.</span></span> <span data-ttu-id="d5edf-119">Это означает, что несмотря на то, что объект Response указывает тип объекта Exchange, который использовался для создания ответа, объект Response не может быть приведен к типу объекта Exchange; Вместо этого необходимо использовать контейнер свойств, предоставленный объектом Response для получения значений из типа объекта Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5edf-119">This means that although the response object indicates the Exchange object type that was used to generate the response, the response object cannot be cast to the Exchange object type; instead, you must use the property bag that is exposed by the response object to obtain the values from the Exchange object type.</span></span>
  
<span data-ttu-id="d5edf-120">Контейнер свойств в объекте Response содержит набор ключей и значений для каждого общедоступного свойства или метода в типе объекта Exchange.</span><span class="sxs-lookup"><span data-stu-id="d5edf-120">The property bag in the response object contains a key/value pair for each public property or method in the Exchange object type.</span></span> <span data-ttu-id="d5edf-121">Объект Response содержит имя базового типа объекта Exchange; Это имя можно использовать для определения типа объекта Exchange, представленного объектом Response, чтобы можно было извлечь соответствующее свойство.</span><span class="sxs-lookup"><span data-stu-id="d5edf-121">The response object contains the name of the underlying Exchange object type; you can use this name to determine the Exchange object type that is represented by the response object so that you can extract the appropriate property.</span></span> <span data-ttu-id="d5edf-122">Каждое значение в контейнере свойств также включает сведения о типе, чтобы можно было привести значение свойства к соответствующему управляемому типу.</span><span class="sxs-lookup"><span data-stu-id="d5edf-122">Each value in the property bag also includes type information so that you can cast the property value to the appropriate managed type.</span></span>
  
## <a name="use-the-cmdlet-response"></a><span data-ttu-id="d5edf-123">Использование ответа командлета</span><span class="sxs-lookup"><span data-stu-id="d5edf-123">Use the cmdlet response</span></span>
<span data-ttu-id="d5edf-124"><a name="usingPSObject_bk"> </a></span><span class="sxs-lookup"><span data-stu-id="d5edf-124"><a name="usingPSObject_bk"> </a></span></span>

<span data-ttu-id="d5edf-125">Класс [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) предоставляет следующие три общедоступные свойства, которые содержат значения базового объекта API Exchange 2013: [Свойства](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [методы](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx)и [элементы](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="d5edf-125">The [PSObject](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject%28VS.85%29.aspx) class exposes the following three public properties that contain the values of the underlying Exchange 2013 API object: [Properties](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.properties%28VS.85%29.aspx), [Methods](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.methods%28VS.85%29.aspx), and [Members](http://msdn.microsoft.com/en-us/library/system.management.automation.psobject.members%28VS.85%29.aspx).</span></span> <span data-ttu-id="d5edf-126">Каждое свойство, предоставляемое объектом API Exchange 2013, имеет соответствующую запись key/value в свойствах **Properties** и **Members** .</span><span class="sxs-lookup"><span data-stu-id="d5edf-126">Each property that is exposed by the Exchange 2013 API object has a corresponding key/value pair in the **Properties** and **Members** properties.</span></span> <span data-ttu-id="d5edf-127">Приложение может индексировать коллекцию **свойств** по имени свойства, чтобы получить значение свойства.</span><span class="sxs-lookup"><span data-stu-id="d5edf-127">Your application can index the **Properties** collection by the name of a property to retrieve the value of the property.</span></span> 
  
<span data-ttu-id="d5edf-128">Свойство **typenames** экземпляра **PSObject** можно использовать для определения типа базового объекта Exchange, который инкапсулируется экземпляром **PSObject** .</span><span class="sxs-lookup"><span data-stu-id="d5edf-128">You can use the **TypeNames** property of the **PSObject** instance to determine the type of the underlying Exchange object that is encapsulated by the **PSObject** instance.</span></span> <span data-ttu-id="d5edf-129">Свойство **typenames** — это коллекция строк, которая содержит иерархию объектов представленного типа.</span><span class="sxs-lookup"><span data-stu-id="d5edf-129">The **TypeNames** property is a collection of strings that contains the object hierarchy of the represented type.</span></span> <span data-ttu-id="d5edf-130">С помощью этих имен можно определить объект, представленный экземпляром **PSObject** , чтобы можно было извлечь соответствующее свойство.</span><span class="sxs-lookup"><span data-stu-id="d5edf-130">You can use these names to determine the object that is represented by the **PSObject** instance so that you can extract the appropriate property.</span></span> 
  
<span data-ttu-id="d5edf-131">В следующем примере кода используется ответ командлета для вывода содержимого коллекции **свойств** экземпляра **PSObject** в консоли.</span><span class="sxs-lookup"><span data-stu-id="d5edf-131">The following code example uses the cmdlet response to print the contents of the **Properties** collection of a **PSObject** instance on the console.</span></span> <span data-ttu-id="d5edf-132">В этом примере кода требуется ссылка на пространство имен **System. Automation. Management** .</span><span class="sxs-lookup"><span data-stu-id="d5edf-132">The code example requires a reference to the **System.Automation.Management** namespace.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="d5edf-133">См. также</span><span class="sxs-lookup"><span data-stu-id="d5edf-133">See also</span></span>

- [<span data-ttu-id="d5edf-134">Создание средств командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="d5edf-134">Create Exchange Management Shell tools</span></span>](create-exchange-management-shell-tools.md)   
- [<span data-ttu-id="d5edf-135">Получение списка пользователей почты с помощью командной консоли Exchange</span><span class="sxs-lookup"><span data-stu-id="d5edf-135">Get a list of mail users by using the Exchange Management Shell</span></span>](how-to-get-a-list-of-mail-users-by-using-the-exchange-management-shell.md)
    

