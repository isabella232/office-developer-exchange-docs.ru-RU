---
title: Функция функция cchksgfiles. Еррчеккдбпажес
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbPages
api_type:
- dllExport
ms.assetid: 5e981a7c-28cd-470c-b7eb-606463e9dd05
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: 78d2dbee6253096d597b4ec2de3878f40ee1b6d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526727"
---
# <a name="cchksgfileserrcheckdbpages-function"></a><span data-ttu-id="df472-103">Функция функция cchksgfiles. Еррчеккдбпажес</span><span class="sxs-lookup"><span data-stu-id="df472-103">CChkSGFiles.ErrCheckDbPages function</span></span>

<span data-ttu-id="df472-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="df472-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="df472-105">Проверка диапазона страниц в указанной базе данных.</span><span class="sxs-lookup"><span data-stu-id="df472-105">Validates a range of pages in a specified database.</span></span> 
  
```cs
Vitual ERRErrCheckDbPages  
(
    Const ULONGiDb,
    Const VOID  * const pvPageBuffer,
    Const ULONGcbPageBuffer,
    PAGE_INFOrgPageInfo[],
    Const ULONGcPageInfo,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="df472-106">Параметры</span><span class="sxs-lookup"><span data-stu-id="df472-106">Parameters</span></span>

### <a name="idb"></a><span data-ttu-id="df472-107">Требуем</span><span class="sxs-lookup"><span data-stu-id="df472-107">iDb</span></span>
  
<span data-ttu-id="df472-108">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="df472-108">Input parameter.</span></span> <span data-ttu-id="df472-109">Индекс в массиве баз данных, заданном параметром **ргвсздб []** , в функцию **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="df472-109">An index into the array of databases specified in the **rgwszDb[]** parameter to the **ErrInit** function.</span></span> <span data-ttu-id="df472-110">Будет проверена база данных, индексируемая этим параметром.</span><span class="sxs-lookup"><span data-stu-id="df472-110">The database indexed by this parameter will be checked.</span></span> 
    
### <a name="pvpagebuffer"></a><span data-ttu-id="df472-111">пвпажебуффер</span><span class="sxs-lookup"><span data-stu-id="df472-111">pvPageBuffer</span></span> 
  
<span data-ttu-id="df472-112">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="df472-112">Input parameter.</span></span> <span data-ttu-id="df472-113">Указатель на буфер, содержащий одну или несколько страниц базы данных, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="df472-113">A pointer to a buffer containing one or more database pages to be checked.</span></span> <span data-ttu-id="df472-114">Размер буфера должен быть кратен размеру страницы базы данных, возвращаемому функцией **еррчеккдбхеадерс** в параметре **пкбдбпажесизе** .</span><span class="sxs-lookup"><span data-stu-id="df472-114">The size of the buffer must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> <span data-ttu-id="df472-115">Вызывающее приложение должно заполнить буфер содержимым страницы базы данных перед вызовом **еррчеккдбпажес**.</span><span class="sxs-lookup"><span data-stu-id="df472-115">The calling application must fill the buffer with the database page contents before calling **ErrCheckDbPages**.</span></span>
    
### <a name="cbpagebuffer"></a><span data-ttu-id="df472-116">кбпажебуффер</span><span class="sxs-lookup"><span data-stu-id="df472-116">cbPageBuffer</span></span>
  
<span data-ttu-id="df472-117">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="df472-117">Input parameter.</span></span> <span data-ttu-id="df472-118">Размер параметра **пвпажебуффер** в байтах.</span><span class="sxs-lookup"><span data-stu-id="df472-118">The size of the **pvPageBuffer** parameter, in bytes.</span></span> <span data-ttu-id="df472-119">Это значение должно быть кратно размеру страницы базы данных, которое возвращается функцией **еррчеккдбхеадерс** в параметре **пкбдбпажесизе** .</span><span class="sxs-lookup"><span data-stu-id="df472-119">This value must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> 
    
### <a name="rgpageinfo"></a><span data-ttu-id="df472-120">Ргпажеинфо []</span><span class="sxs-lookup"><span data-stu-id="df472-120">rgPageInfo[]</span></span> 
  
<span data-ttu-id="df472-121">Входной/выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="df472-121">Input/output parameter.</span></span> <span data-ttu-id="df472-122">Массив структур \*\* \_ сведений о странице\*\* , которые **еррчеккдбпажес** заполняют детальные результаты каждой проверенной страницы базы данных.</span><span class="sxs-lookup"><span data-stu-id="df472-122">An array of **PAGE\_INFO** structures that **ErrCheckDbPages** fills with detailed results of each database page that is checked.</span></span> <span data-ttu-id="df472-123">Массив должен иметь по одному элементу для каждой страницы базы данных, переданной в параметре **пвпажебуффер** , а в поле **улпгно** в каждой структуре \*\* \_ сведений о странице\*\* должен быть задан логический номер страницы, соответствующий странице базы данных.</span><span class="sxs-lookup"><span data-stu-id="df472-123">The array must have one element for each database page passed in the **pvPageBuffer** parameter, and the **ulPgno** field in each **PAGE\_INFO** structure must be set to the logical page number that corresponds to the database page.</span></span> <span data-ttu-id="df472-124">Дополнительные сведения см. в разделе "Примечания" Далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="df472-124">For more information, see "Remarks" later in this topic.</span></span> 
    
### <a name="cpageinfo"></a><span data-ttu-id="df472-125">кпажеинфо</span><span class="sxs-lookup"><span data-stu-id="df472-125">cPageInfo</span></span>
  
<span data-ttu-id="df472-126">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="df472-126">Input parameter.</span></span> <span data-ttu-id="df472-127">Число записей в массиве **ргпажеинфо []** .</span><span class="sxs-lookup"><span data-stu-id="df472-127">The number of entries in the **rgPageInfo[]** array.</span></span> <span data-ttu-id="df472-128">Это значение должно быть равно числу страниц базы данных, переданных в параметре **пвпажебуффер** .</span><span class="sxs-lookup"><span data-stu-id="df472-128">This value must be equal to the number of database pages passed in the **pvPageBuffer** parameter.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="df472-129">ulFlags</span><span class="sxs-lookup"><span data-stu-id="df472-129">ulFlags</span></span> 
  
<span data-ttu-id="df472-130">Необязательный входной параметр.</span><span class="sxs-lookup"><span data-stu-id="df472-130">Optional input parameter.</span></span> <span data-ttu-id="df472-131">Это значение зарезервировано для использования в будущем.</span><span class="sxs-lookup"><span data-stu-id="df472-131">This value is reserved for future use.</span></span> <span data-ttu-id="df472-132">Значение, передаваемое в этом параметре, должно быть равно 0 (нулю).</span><span class="sxs-lookup"><span data-stu-id="df472-132">The value passed in this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="df472-133">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="df472-133">Return value</span></span>

<span data-ttu-id="df472-134">Код ошибки из перечисления [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="df472-134">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="df472-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="df472-135">Remarks</span></span>

<span data-ttu-id="df472-136">Обратите внимание, что необходимо указать базу данных в массиве баз данных, передаваемых функции **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="df472-136">Note that you need to have specified the database in the array of databases passed to the **ErrInit** function.</span></span> <span data-ttu-id="df472-137">Кроме того, **еррчеккдбхеадерс** должен вызываться до **еррчеккдбпажес**.</span><span class="sxs-lookup"><span data-stu-id="df472-137">Also, **ErrCheckDbHeaders** must be called before **ErrCheckDbPages**.</span></span>
  
<span data-ttu-id="df472-138">Вызывающее приложение должно выделить буфер памяти, достаточно большой для хранения страниц базы данных, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="df472-138">The calling application must allocate a memory buffer that is large enough to hold the database pages to be checked.</span></span> <span data-ttu-id="df472-139">Приложение несет ответственность за заполнение буфера содержимым одной или нескольких таких страниц базы данных.</span><span class="sxs-lookup"><span data-stu-id="df472-139">The application is responsible for filling the buffer with the contents of one or more such database pages.</span></span> 
  
<span data-ttu-id="df472-140">Вызывающее приложение должно вызвать **еррчеккдбхеадерс** перед вызовом **еррчеккдбпажес**.</span><span class="sxs-lookup"><span data-stu-id="df472-140">The calling application must call **ErrCheckDbHeaders** before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="df472-141">Эту функцию можно вызывать столько раз, сколько необходимо, чтобы охватить все страницы всех файлов базы данных, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="df472-141">This function can be called as many times as necessary to cover all the pages in all database files that are to be checked.</span></span>
  
<span data-ttu-id="df472-142">В параметре **ргпажеинфо []** каждый возвращаемый элемент содержит сведения о странице базы данных в структуре \*\* \_ сведений о странице\*\* .</span><span class="sxs-lookup"><span data-stu-id="df472-142">In the **rgPageInfo[]** parameter, each element returned contains information about the database page in a **PAGE\_INFO** structure.</span></span> <span data-ttu-id="df472-143">Если функция **еррчеккдбпажес** возвращает ошибку, приложение должно проверять каждую структуру \*\* \_ сведений о странице\*\* , чтобы определить, на какой странице была обнаружена ошибка.</span><span class="sxs-lookup"><span data-stu-id="df472-143">If the **ErrCheckDbPages** function returns an error, the application should check each **PAGE\_INFO** structure to determine on which page the error was found.</span></span> <span data-ttu-id="df472-144">Например, сравнение значений **чекксумактуал** и **чекксумекспектед** будет указывать на то, была ли обнаружена ошибка контрольной суммы на этой странице базы данных.</span><span class="sxs-lookup"><span data-stu-id="df472-144">For example, comparing the **checksumActual** and **checksumExpected** values will indicate whether a checksum error was detected on that database page.</span></span> 
  
<span data-ttu-id="df472-145">Если **еррчеккдбпажес** обнаруживает ошибки в содержимом базы данных, он создает запись в журнале событий ошибок Windows.</span><span class="sxs-lookup"><span data-stu-id="df472-145">If **ErrCheckDbPages** detects any errors in the database content, it will create a Windows Error event log entry.</span></span> 
  
<span data-ttu-id="df472-146">Объект **функция cchksgfiles** определяет, действительно ли проверены все базы данных, зарегистрированные с помощью функции **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="df472-146">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="df472-147">В частности, **функция cchksgfiles** использует функцию **еррчеккдбпажес** , чтобы определить, действительно ли проверено то же количество страниц базы данных, что и в **еррчеккдбхеадерс** .</span><span class="sxs-lookup"><span data-stu-id="df472-147">Specifically, **CChkSGFiles** uses the **ErrCheckDbPages** function to determine whether the same number of database pages indicated by **ErrCheckDbHeaders** were actually verified.</span></span> <span data-ttu-id="df472-148">Если правильное количество страниц в каждой базе данных не прошло проверку, функция **ерртерм** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="df472-148">If the correct number of pages in each database were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="df472-149">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, вы можете вызвать функцию **еррчеккдбпажес** в многопоточной части приложения.</span><span class="sxs-lookup"><span data-stu-id="df472-149">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckDbPages** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="df472-150">Обратите внимание, что **еррчеккдбпажес** обычно вызывается несколько раз для каждой проверенной базы данных.</span><span class="sxs-lookup"><span data-stu-id="df472-150">Note that **ErrCheckDbPages** is typically called multiple times for each database that is checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="df472-151">Requirements</span><span class="sxs-lookup"><span data-stu-id="df472-151">Requirements</span></span>

<span data-ttu-id="df472-152">Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="df472-152">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="df472-153">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="df472-153">The account that the application is running under must have read permissions to the database and log files that are to be checked.</span></span>
  

