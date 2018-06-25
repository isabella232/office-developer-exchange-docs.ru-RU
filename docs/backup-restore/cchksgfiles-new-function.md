---
title: Функция CChkSGFiles.New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: b40f8b1a95477715b29defb4addabfb333e92d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760914"
---
# <a name="cchksgfilesnew-function"></a><span data-ttu-id="086b7-103">Функция CChkSGFiles.New</span><span class="sxs-lookup"><span data-stu-id="086b7-103">CChkSGFiles.New function</span></span>

<span data-ttu-id="086b7-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="086b7-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="086b7-105">Создает новый экземпляр класса **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="086b7-105">Creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="086b7-106">Перед можно указать группы хранения и базы данных для проверки, необходимо вызвать эту функцию.</span><span class="sxs-lookup"><span data-stu-id="086b7-106">You must call this function before you can specify the storage group and databases to be checked.</span></span> 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a><span data-ttu-id="086b7-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="086b7-107">Parameters</span></span>

<span data-ttu-id="086b7-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="086b7-108">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="086b7-109">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="086b7-109">Return value</span></span>

<span data-ttu-id="086b7-110">Ссылка (указатель) на только что созданный объект.</span><span class="sxs-lookup"><span data-stu-id="086b7-110">A reference (pointer) to the newly created object.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="086b7-111">Замечания</span><span class="sxs-lookup"><span data-stu-id="086b7-111">Remarks</span></span>

<span data-ttu-id="086b7-112">Функция **New** создает объект **CCheckSGFiles** и возвращает вызывающему (указатель) ссылку на этот объект.</span><span class="sxs-lookup"><span data-stu-id="086b7-112">The **New** function creates a **CCheckSGFiles** object and returns to the caller a reference (pointer) to that object.</span></span> <span data-ttu-id="086b7-113">Эта функция необходимо вызвать до вызова любой из других функций в классе **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="086b7-113">You must call this function before it calls any of the other functions in the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="086b7-114">Если вы используете многопоточного приложения CHKSGFILES, необходимо вызвать функцию **New** в одном потоке часть приложения и его можно вызвать только один раз для каждого объекта **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="086b7-114">If you're using CHKSGFILES in a multithreaded application, you must call the **New** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="086b7-115">Требования</span><span class="sxs-lookup"><span data-stu-id="086b7-115">Requirements</span></span>

<span data-ttu-id="086b7-116">Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="086b7-116">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="086b7-117">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="086b7-117">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

