---
title: Серверверсион (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2c0bc41c-2452-4fc8-a19c-0e85f9fdbc4a
description: Элемент Серверверсион представляет номер версии компьютера, на котором работает Microsoft Exchange Server.
ms.openlocfilehash: 3ef531a69d2dd00ee9784c9eb191684ce517e842
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461970"
---
# <a name="serverversion-pox"></a><span data-ttu-id="9fe23-103">Серверверсион (POX)</span><span class="sxs-lookup"><span data-stu-id="9fe23-103">ServerVersion (POX)</span></span>

<span data-ttu-id="9fe23-104">Элемент **серверверсион** представляет номер версии компьютера, на котором работает Microsoft Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="9fe23-104">The **ServerVersion** element represents the version number of the computer that is running Microsoft Exchange Server.</span></span> 
  
- [<span data-ttu-id="9fe23-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="9fe23-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="9fe23-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="9fe23-106">Response (POX)</span></span>](response-pox.md)
- [<span data-ttu-id="9fe23-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="9fe23-107">Account (POX)</span></span>](account-pox.md)
- [<span data-ttu-id="9fe23-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="9fe23-108">Protocol (POX)</span></span>](protocol-pox.md)
- [<span data-ttu-id="9fe23-109">Серверверсион (POX)</span><span class="sxs-lookup"><span data-stu-id="9fe23-109">ServerVersion (POX)</span></span>](serverversion-pox.md)
  
```xml
<ServerVersion/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9fe23-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9fe23-110">Attributes and elements</span></span>

<span data-ttu-id="9fe23-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9fe23-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fe23-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fe23-112">Attributes</span></span>

<span data-ttu-id="9fe23-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9fe23-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fe23-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9fe23-114">Child elements</span></span>

<span data-ttu-id="9fe23-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9fe23-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9fe23-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9fe23-116">Parent elements</span></span>

|<span data-ttu-id="9fe23-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9fe23-117">**Element**</span></span>|<span data-ttu-id="9fe23-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9fe23-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fe23-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="9fe23-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9fe23-120">Содержит спецификации для подключения клиента к компьютеру, на котором выполняется Microsoft Exchange, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9fe23-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9fe23-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9fe23-121">Text value</span></span>

<span data-ttu-id="9fe23-122">Текстовое значение представляет номер версии сервера Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="9fe23-122">The text value represents the Exchange server version number.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9fe23-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="9fe23-123">Remarks</span></span>

<span data-ttu-id="9fe23-124">Значение **серверверсион** является допустимым только в том случае, если элемент [Type (POX)](type-pox.md) РАВЕН сумме или expr.</span><span class="sxs-lookup"><span data-stu-id="9fe23-124">The **ServerVersion** value is only valid if the [Type (POX)](type-pox.md) element is equal to EXCH or EXPR.</span></span> <span data-ttu-id="9fe23-125">Значение **серверверсион** — это шестнадцатеричное число, которое содержит MajorVersion, minorversion и мажорбуилднумбер сервера.</span><span class="sxs-lookup"><span data-stu-id="9fe23-125">The **ServerVersion** value is a hexadecimal number that contains the MajorVersion, MinorVersion, and MajorBuildNumber of the server.</span></span> 
  
## <a name="example"></a><span data-ttu-id="9fe23-126">Пример</span><span class="sxs-lookup"><span data-stu-id="9fe23-126">Example</span></span>

<span data-ttu-id="9fe23-127">В следующем примере показано, как преобразовать значение **серверверсион** , которое возвращается в ответе автообнаружения для получения и отображения MajorVersion, minorversion и мажорбуилднумбер.</span><span class="sxs-lookup"><span data-stu-id="9fe23-127">The following example coverts a **ServerVersion** value that is returned in an Autodiscover response to obtain and display the MajorVersion, MinorVersion, and MajorBuildNumber.</span></span> <span data-ttu-id="9fe23-128">В этом примере показано, как ввести шестнадцатеричное значение для значения **серверверсион** .</span><span class="sxs-lookup"><span data-stu-id="9fe23-128">This example enables you to enter a hexadecimal value for the **ServerVersion** value.</span></span> <span data-ttu-id="9fe23-129">Если значение **серверверсион** не введено, используется значение **серверверсион** по умолчанию 738180DA.</span><span class="sxs-lookup"><span data-stu-id="9fe23-129">If no **ServerVersion** value is entered, a default **ServerVersion** value of 738180DA is used.</span></span> 
  
```csharp
static void Main(string[] args)
{
    // Convert a ServerVersion value that is returned from an Autodiscover request.
    // The value is a hex value and can be converted to the MajorVersion, MinorVersion,
    // and MajorBuildNumber.
    Console.WriteLine("Enter ServerVersion returned from the Autodiscover (eg. 738180DA) and Enter.");
    Console.WriteLine("To use the default ServerVersion of 738180DA, just hit Enter.");
    // Get the hexadecimal ServerVersion value.
    string serverversionhex = Console.ReadLine();
    // If nothing is entered, use the default server version of "738180DA"
    if (serverversionhex == "")
    {
        serverversionhex = "738180DA";
    }
    Console.WriteLine("ServerVersion (Hex) = " + serverversionhex);
    string serverversionbinary = Convert.ToString(Convert.ToInt32(serverversionhex, 16), 2);
    // The ServerVersion (binary) should be 32 bits in length. If the 
    // server version in binary is a length of 31 characters, the leading
    // zero has been removed in the conversion process. Put the missing zero back.
    if (serverversionbinary.Length == 31)
    {
        serverversionbinary = String.Concat("0", serverversionbinary);
    }
    Console.WriteLine("ServerVersion (bin) = " + serverversionbinary);
    // The first 4 bits represent a number used for comparison against  
    // older version number structures. You can ignore this.
    // The next 6 bits represent the major version number.
    int majorversion = Convert.ToInt32(serverversionbinary.Substring(4, 6), 2);
    Console.WriteLine("MajorVersion: " + majorversion);
    // The next 6 bits represent the minor version number.
    int minorversion = Convert.ToInt32(serverversionbinary.Substring(10, 6), 2);
    Console.WriteLine("MinorVersion: " + minorversion);
    
    // The next bit represent a flag - you can ignore this.
    // The next 15 bits represent the major build number.
    int majorbuild = Convert.ToInt32(serverversionbinary.Substring(17, 15), 2);
    Console.WriteLine("MajorBuildVersion: " + majorbuild);
    Console.WriteLine("\n\nPress any key to continue");
    Console.ReadKey();
}
```

## <a name="see-also"></a><span data-ttu-id="9fe23-130">См. также</span><span class="sxs-lookup"><span data-stu-id="9fe23-130">See also</span></span>

- [<span data-ttu-id="9fe23-131">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="9fe23-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

