---
title: Функция CChkSGFiles.Delete
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
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: 5c41007a797e5a256692b2c4bdcb3cfae82c12ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760920"
---
# <a name="cchksgfilesdelete-function"></a><span data-ttu-id="5ed4a-103">Функция CChkSGFiles.Delete</span><span class="sxs-lookup"><span data-stu-id="5ed4a-103">CChkSGFiles.Delete function</span></span>

<span data-ttu-id="5ed4a-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="5ed4a-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="5ed4a-105">Удаляет существующий экземпляр класса **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="5ed4a-105">Destroys an existing instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="5ed4a-106">После завершения работы с указанным объектом приложения, необходимо вызвать эту функцию.</span><span class="sxs-lookup"><span data-stu-id="5ed4a-106">You must call this function after the application has finished working with the specified object.</span></span> 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a><span data-ttu-id="5ed4a-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="5ed4a-107">Parameters</span></span>

### <a name="pcchecksgfiles"></a><span data-ttu-id="5ed4a-108">pcchecksgfiles</span><span class="sxs-lookup"><span data-stu-id="5ed4a-108">pcchecksgfiles</span></span> 
  
<span data-ttu-id="5ed4a-109">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="5ed4a-109">Input parameter.</span></span> <span data-ttu-id="5ed4a-110">Указатель на существующий объект **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="5ed4a-110">A pointer to an existing **CCheckSGFiles** object.</span></span> <span data-ttu-id="5ed4a-111">Затем освободится память, связанную с объектом.</span><span class="sxs-lookup"><span data-stu-id="5ed4a-111">The memory associated with the object will then be freed.</span></span> 
    
## <a name="return-value"></a><span data-ttu-id="5ed4a-112">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="5ed4a-112">Return value</span></span>

<span data-ttu-id="5ed4a-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="5ed4a-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5ed4a-114">Замечания</span><span class="sxs-lookup"><span data-stu-id="5ed4a-114">Remarks</span></span>

<span data-ttu-id="5ed4a-115">Функция **Удаление** освобождает память, связанного с объектом **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="5ed4a-115">The **Delete** function frees the memory associated with the **CCheckSGFiles** object.</span></span> <span data-ttu-id="5ed4a-116">После вызова **Удаление**указателя мыши, переданной в параметре *pcchecksgfiles* будет недопустимый и никакие другие операции, которые могут выполняться для этого объекта.</span><span class="sxs-lookup"><span data-stu-id="5ed4a-116">After you call **Delete**, the pointer passed in the  *pcchecksgfiles*  parameter will be invalid and no other operations can be performed on that object.</span></span> 
  
<span data-ttu-id="5ed4a-117">Если приложение использует функцию **ErrCheckDbPages** , приложение должно освободить буфер памяти вручную; **Удаление** функции не освобождает его.</span><span class="sxs-lookup"><span data-stu-id="5ed4a-117">If the application uses the **ErrCheckDbPages** function, the application must free the memory buffer manually; the **Delete** function will not free it.</span></span> 
  
<span data-ttu-id="5ed4a-118">Если вы используете многопоточного приложения CHKSGFILES, необходимо вызвать функцию **Удалить** в одном потоке часть приложения и его можно вызвать только один раз для каждого объекта **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="5ed4a-118">If you're using CHKSGFILES in a multithreaded application, you must call the **Delete** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="5ed4a-119">Требования</span><span class="sxs-lookup"><span data-stu-id="5ed4a-119">Requirements</span></span>

<span data-ttu-id="5ed4a-120">Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="5ed4a-120">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="5ed4a-121">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="5ed4a-121">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

