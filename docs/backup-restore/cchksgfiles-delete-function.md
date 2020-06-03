---
title: Функция функция cchksgfiles. Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: 38cb72b42727855f652de607bb2a02ecdeaae16e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44447052"
---
# <a name="cchksgfilesdelete-function"></a><span data-ttu-id="3ab94-103">Функция функция cchksgfiles. Delete</span><span class="sxs-lookup"><span data-stu-id="3ab94-103">CChkSGFiles.Delete function</span></span>

<span data-ttu-id="3ab94-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="3ab94-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="3ab94-105">Уничтожает существующий экземпляр класса **функция cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="3ab94-105">Destroys an existing instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="3ab94-106">Эту функцию необходимо вызвать после завершения работы приложения с указанным объектом.</span><span class="sxs-lookup"><span data-stu-id="3ab94-106">You must call this function after the application has finished working with the specified object.</span></span> 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a><span data-ttu-id="3ab94-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="3ab94-107">Parameters</span></span>

### <a name="pcchecksgfiles"></a><span data-ttu-id="3ab94-108">пкчекксгфилес</span><span class="sxs-lookup"><span data-stu-id="3ab94-108">pcchecksgfiles</span></span> 
  
<span data-ttu-id="3ab94-109">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="3ab94-109">Input parameter.</span></span> <span data-ttu-id="3ab94-110">Указатель на существующий объект **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="3ab94-110">A pointer to an existing **CCheckSGFiles** object.</span></span> <span data-ttu-id="3ab94-111">После этого память, связанная с объектом, будет освобождена.</span><span class="sxs-lookup"><span data-stu-id="3ab94-111">The memory associated with the object will then be freed.</span></span> 
    
## <a name="return-value"></a><span data-ttu-id="3ab94-112">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="3ab94-112">Return value</span></span>

<span data-ttu-id="3ab94-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3ab94-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3ab94-114">Примечания</span><span class="sxs-lookup"><span data-stu-id="3ab94-114">Remarks</span></span>

<span data-ttu-id="3ab94-115">Функция **Delete** освобождает память, связанную с объектом **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="3ab94-115">The **Delete** function frees the memory associated with the **CCheckSGFiles** object.</span></span> <span data-ttu-id="3ab94-116">После вызова метода **Delete**указатель, переданный в параметре *пкчекксгфилес* , будет недопустимым, и для этого объекта невозможно выполнить другие операции.</span><span class="sxs-lookup"><span data-stu-id="3ab94-116">After you call **Delete**, the pointer passed in the  *pcchecksgfiles*  parameter will be invalid and no other operations can be performed on that object.</span></span> 
  
<span data-ttu-id="3ab94-117">Если приложение использует функцию **еррчеккдбпажес** , приложение должно освободить буфер памяти вручную; Функция **удаления** не позволит освободить ее.</span><span class="sxs-lookup"><span data-stu-id="3ab94-117">If the application uses the **ErrCheckDbPages** function, the application must free the memory buffer manually; the **Delete** function will not free it.</span></span> 
  
<span data-ttu-id="3ab94-118">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, необходимо вызвать функцию **Delete** в однопотоковой части приложения, и вы можете вызвать его только один раз для каждого объекта **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="3ab94-118">If you're using CHKSGFILES in a multithreaded application, you must call the **Delete** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="3ab94-119">Requirements</span><span class="sxs-lookup"><span data-stu-id="3ab94-119">Requirements</span></span>

<span data-ttu-id="3ab94-120">Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="3ab94-120">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="3ab94-121">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="3ab94-121">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

