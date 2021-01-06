---
title: Функция CChkSGFiles.PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: 3c8f749a03b4aa251bf9312eba5d7e2d46c91fae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452897"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a><span data-ttu-id="6f70d-103">Функция CChkSGFiles.PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="6f70d-103">CChkSGFiles.PgnoFromFileOffset function</span></span>

<span data-ttu-id="6f70d-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="6f70d-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="6f70d-105">Возвращает номер страницы логической базы данных, соответствующий указанному индексу в физическом файле базы данных.</span><span class="sxs-lookup"><span data-stu-id="6f70d-105">Returns the logical database page number that corresponds to the specified byte index in the physical database file.</span></span> <span data-ttu-id="6f70d-106">Если смещение файла недопустимо или функция **ErrCheckDbHeaders** не была вызвана для баз данных, эта функция возвращает 0 (ноль).</span><span class="sxs-lookup"><span data-stu-id="6f70d-106">If the file offset is invalid, or if the **ErrCheckDbHeaders** function has not been called for the databases, this function returns 0 (zero).</span></span> 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a><span data-ttu-id="6f70d-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="6f70d-107">Parameters</span></span>

### <a name="ibfileoffset"></a><span data-ttu-id="6f70d-108">ibFileOffset</span><span class="sxs-lookup"><span data-stu-id="6f70d-108">ibFileOffset</span></span>
  
<span data-ttu-id="6f70d-109">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="6f70d-109">Input parameter.</span></span> <span data-ttu-id="6f70d-110">Смещение в файл базы данных в ветвях.</span><span class="sxs-lookup"><span data-stu-id="6f70d-110">The offset into a database file, in bytes.</span></span>
    
## <a name="return-value"></a><span data-ttu-id="6f70d-111">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="6f70d-111">Return value</span></span>

<span data-ttu-id="6f70d-112">Логический номер страницы файла базы данных, который включает указанное смещение.</span><span class="sxs-lookup"><span data-stu-id="6f70d-112">The database file's logical page number that includes the specified offset.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6f70d-113">Примечания</span><span class="sxs-lookup"><span data-stu-id="6f70d-113">Remarks</span></span>

<span data-ttu-id="6f70d-114">Если параметр **ibFileOffset** недействителен, функция **PgnoFromFileOffset** возвращает значение 0 (ноль).</span><span class="sxs-lookup"><span data-stu-id="6f70d-114">If the **ibFileOffset** parameter is invalid, the **PgnoFromFileOffset** function returns 0 (zero).</span></span> 
  
<span data-ttu-id="6f70d-115">**PgnoFromFileOffset** также возвращает 0 (ноль), если вы не вызвали функцию **ErrCheckDbHeaders** в экземпляре **CCheckSGFiles.**</span><span class="sxs-lookup"><span data-stu-id="6f70d-115">**PgnoFromFileOffset** also returns 0 (zero) if you haven't called the **ErrCheckDbHeaders** function on the **CCheckSGFiles** instance.</span></span> <span data-ttu-id="6f70d-116">Необходимо вызвать **ErrCheckDbHeaders,** чтобы инициализировать размер страницы базы данных и количество страниц, выделенных для headers базы данных.</span><span class="sxs-lookup"><span data-stu-id="6f70d-116">You must call **ErrCheckDbHeaders** to initialize the database page size and number of pages allocated to database headers.</span></span> 
  
<span data-ttu-id="6f70d-117">**PgnoFromFileOffset** следует использовать для заполнения элементов структуры **PAGE \_ INFO** при подготовке к вызову **ErrCheckDbPages.**</span><span class="sxs-lookup"><span data-stu-id="6f70d-117">You should use **PgnoFromFileOffset** to fill in the **PAGE\_INFO** structure elements in preparation for calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="6f70d-118">Параметр **rgPageInfo** для **ErrCheckDbPages** требует, чтобы каждый  элемент в массиве был PAGE_INFO структурой с правильно инициализированными значениями членов **ulPgno.**</span><span class="sxs-lookup"><span data-stu-id="6f70d-118">The **rgPageInfo** parameter to **ErrCheckDbPages** requires that each element in the array be a **PAGE_INFO** structure, with the **ulPgno** member values correctly initialized.</span></span> 
  
<span data-ttu-id="6f70d-119">Если вы используете CHKSGFILES в многопрочитаном приложении, вы можете вызвать функцию **PgnoFromFileOffset** в многопрочитаной части приложения.</span><span class="sxs-lookup"><span data-stu-id="6f70d-119">If you're using CHKSGFILES in a multithreaded application, you can call the **PgnoFromFileOffset** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="6f70d-120">Обратите внимание, что обычно эта функция вызывалась несколько раз для каждой проверяемой базы данных.</span><span class="sxs-lookup"><span data-stu-id="6f70d-120">Note that you would typically call this function multiple times for each database being checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="6f70d-121">Требования</span><span class="sxs-lookup"><span data-stu-id="6f70d-121">Requirements</span></span>

<span data-ttu-id="6f70d-122">Exchange Server 2013 включает только 64-битную версию API CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="6f70d-122">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="6f70d-123">Учетная запись, в которой запущено приложение, должна иметь разрешение на чтение базы данных и файлов журналов, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="6f70d-123">The account that the application is running under must have read permission to the database and log files that are to be checked.</span></span>
  

