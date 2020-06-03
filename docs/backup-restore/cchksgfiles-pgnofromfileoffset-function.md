---
title: Функция функция cchksgfiles. Пгнофромфилеоффсет
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
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: 3c8f749a03b4aa251bf9312eba5d7e2d46c91fae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452897"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a><span data-ttu-id="23f6a-103">Функция функция cchksgfiles. Пгнофромфилеоффсет</span><span class="sxs-lookup"><span data-stu-id="23f6a-103">CChkSGFiles.PgnoFromFileOffset function</span></span>

<span data-ttu-id="23f6a-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="23f6a-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="23f6a-105">Возвращает номер страницы логической базы данных, соответствующий указанному индексу байтов в физическом файле базы данных.</span><span class="sxs-lookup"><span data-stu-id="23f6a-105">Returns the logical database page number that corresponds to the specified byte index in the physical database file.</span></span> <span data-ttu-id="23f6a-106">Если смещение файла недопустимо или функция **еррчеккдбхеадерс** не была вызвана для баз данных, эта функция возвращает значение 0 (ноль).</span><span class="sxs-lookup"><span data-stu-id="23f6a-106">If the file offset is invalid, or if the **ErrCheckDbHeaders** function has not been called for the databases, this function returns 0 (zero).</span></span> 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a><span data-ttu-id="23f6a-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="23f6a-107">Parameters</span></span>

### <a name="ibfileoffset"></a><span data-ttu-id="23f6a-108">ибфилеоффсет</span><span class="sxs-lookup"><span data-stu-id="23f6a-108">ibFileOffset</span></span>
  
<span data-ttu-id="23f6a-109">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="23f6a-109">Input parameter.</span></span> <span data-ttu-id="23f6a-110">Смещение в файле базы данных в байтах.</span><span class="sxs-lookup"><span data-stu-id="23f6a-110">The offset into a database file, in bytes.</span></span>
    
## <a name="return-value"></a><span data-ttu-id="23f6a-111">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="23f6a-111">Return value</span></span>

<span data-ttu-id="23f6a-112">Логический номер страницы файла базы данных, включающий указанное смещение.</span><span class="sxs-lookup"><span data-stu-id="23f6a-112">The database file's logical page number that includes the specified offset.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="23f6a-113">Примечания</span><span class="sxs-lookup"><span data-stu-id="23f6a-113">Remarks</span></span>

<span data-ttu-id="23f6a-114">Если параметр **ибфилеоффсет** является недопустимым, функция **пгнофромфилеоффсет** возвращает значение 0 (ноль).</span><span class="sxs-lookup"><span data-stu-id="23f6a-114">If the **ibFileOffset** parameter is invalid, the **PgnoFromFileOffset** function returns 0 (zero).</span></span> 
  
<span data-ttu-id="23f6a-115">**Пгнофромфилеоффсет** также возвращает 0 (ноль), если вы не вызывали функцию **еррчеккдбхеадерс** в экземпляре **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="23f6a-115">**PgnoFromFileOffset** also returns 0 (zero) if you haven't called the **ErrCheckDbHeaders** function on the **CCheckSGFiles** instance.</span></span> <span data-ttu-id="23f6a-116">Для инициализации размера страницы базы данных и количества страниц, выделенных для заголовков баз данных, необходимо вызвать **еррчеккдбхеадерс** .</span><span class="sxs-lookup"><span data-stu-id="23f6a-116">You must call **ErrCheckDbHeaders** to initialize the database page size and number of pages allocated to database headers.</span></span> 
  
<span data-ttu-id="23f6a-117">**Пгнофромфилеоффсет** следует использовать для заполнения элементов структуры \*\* \_ сведений о странице\*\* при подготовке к вызову **еррчеккдбпажес**.</span><span class="sxs-lookup"><span data-stu-id="23f6a-117">You should use **PgnoFromFileOffset** to fill in the **PAGE\_INFO** structure elements in preparation for calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="23f6a-118">Для параметра **ргпажеинфо** в **еррчеккдбпажес** необходимо, чтобы каждый элемент массива был структурой **PAGE_INFO** с корректной инициализацией значений элементов **улпгно** .</span><span class="sxs-lookup"><span data-stu-id="23f6a-118">The **rgPageInfo** parameter to **ErrCheckDbPages** requires that each element in the array be a **PAGE_INFO** structure, with the **ulPgno** member values correctly initialized.</span></span> 
  
<span data-ttu-id="23f6a-119">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, вы можете вызвать функцию **пгнофромфилеоффсет** в многопоточной части приложения.</span><span class="sxs-lookup"><span data-stu-id="23f6a-119">If you're using CHKSGFILES in a multithreaded application, you can call the **PgnoFromFileOffset** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="23f6a-120">Обратите внимание, что эта функция обычно вызывается для каждой проверяемой базы данных несколько раз.</span><span class="sxs-lookup"><span data-stu-id="23f6a-120">Note that you would typically call this function multiple times for each database being checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="23f6a-121">Requirements</span><span class="sxs-lookup"><span data-stu-id="23f6a-121">Requirements</span></span>

<span data-ttu-id="23f6a-122">Exchange Server 2013 включает в себя только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="23f6a-122">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="23f6a-123">Учетная запись, под которой выполняется приложение, должна иметь разрешение на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="23f6a-123">The account that the application is running under must have read permission to the database and log files that are to be checked.</span></span>
  

