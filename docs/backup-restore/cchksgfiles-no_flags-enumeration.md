---
title: Перечисление CChkSGFiles.NO_FLAGS
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NO_FLAGS
api_type:
- dllExport
ms.assetid: 6b18b645-fec4-429a-9900-62ad0f19bf96
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: dbe4cedf2011a1607a6db55dc064bd42dc229123
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761868"
---
# <a name="cchksgfilesnoflags-enumeration"></a><span data-ttu-id="eb2d3-103">Перечисление CChkSGFiles.NO_FLAGS</span><span class="sxs-lookup"><span data-stu-id="eb2d3-103">CChkSGFiles.NO_FLAGS enumeration</span></span>

<span data-ttu-id="eb2d3-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="eb2d3-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="eb2d3-105">Выступает в качестве значение-заполнитель для параметров **ulFlags** , которые были приняты большинство функций класса **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="eb2d3-105">Serves as a placeholder value for the **ulFlags** parameters that are accepted by most **CCheckSGFiles** class functions.</span></span> 
  
```cs
Enum { NO_FLAGS = 0 }

```

## <a name="requirements"></a><span data-ttu-id="eb2d3-106">Требования</span><span class="sxs-lookup"><span data-stu-id="eb2d3-106">Requirements</span></span>

<span data-ttu-id="eb2d3-107">Exchange Server 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="eb2d3-107">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="eb2d3-108">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="eb2d3-108">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

