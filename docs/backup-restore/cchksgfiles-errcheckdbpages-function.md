---
title: Функция CChkSGFiles.ErrCheckDbPages
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
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: f1588b1dbc4bd7e83683fa4432a175405ad17903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760919"
---
# <a name="cchksgfileserrcheckdbpages-function"></a><span data-ttu-id="c758a-103">Функция CChkSGFiles.ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="c758a-103">CChkSGFiles.ErrCheckDbPages function</span></span>

<span data-ttu-id="c758a-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="c758a-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="c758a-105">Проверяет диапазон страниц в указанной базе данных.</span><span class="sxs-lookup"><span data-stu-id="c758a-105">Validates a range of pages in a specified database.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="c758a-106">Parameters</span><span class="sxs-lookup"><span data-stu-id="c758a-106">Parameters</span></span>

### <a name="idb"></a><span data-ttu-id="c758a-107">iDb</span><span class="sxs-lookup"><span data-stu-id="c758a-107">iDb</span></span>
  
<span data-ttu-id="c758a-108">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="c758a-108">Input parameter.</span></span> <span data-ttu-id="c758a-109">Индекс массива баз данных, указанной в параметре **[] rgwszDb** в функцию **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="c758a-109">An index into the array of databases specified in the **rgwszDb[]** parameter to the **ErrInit** function.</span></span> <span data-ttu-id="c758a-110">Базы данных, индексированные данный параметр будет проверяться.</span><span class="sxs-lookup"><span data-stu-id="c758a-110">The database indexed by this parameter will be checked.</span></span> 
    
### <a name="pvpagebuffer"></a><span data-ttu-id="c758a-111">pvPageBuffer</span><span class="sxs-lookup"><span data-stu-id="c758a-111">pvPageBuffer</span></span> 
  
<span data-ttu-id="c758a-112">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="c758a-112">Input parameter.</span></span> <span data-ttu-id="c758a-113">Указатель на буфер, содержащий один или несколько страниц базы данных для проверки.</span><span class="sxs-lookup"><span data-stu-id="c758a-113">A pointer to a buffer containing one or more database pages to be checked.</span></span> <span data-ttu-id="c758a-114">Размер буфера должен быть несколько страниц размера базы данных, как с помощью параметра **pcbDbPageSize** возвращаемых функцией **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="c758a-114">The size of the buffer must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> <span data-ttu-id="c758a-115">До вызова метода **ErrCheckDbPages**вызывающему приложению необходимо переполнить буфер с содержимым страниц базы данных.</span><span class="sxs-lookup"><span data-stu-id="c758a-115">The calling application must fill the buffer with the database page contents before calling **ErrCheckDbPages**.</span></span>
    
### <a name="cbpagebuffer"></a><span data-ttu-id="c758a-116">cbPageBuffer</span><span class="sxs-lookup"><span data-stu-id="c758a-116">cbPageBuffer</span></span>
  
<span data-ttu-id="c758a-117">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="c758a-117">Input parameter.</span></span> <span data-ttu-id="c758a-118">Размер параметр **pvPageBuffer** в байтах.</span><span class="sxs-lookup"><span data-stu-id="c758a-118">The size of the **pvPageBuffer** parameter, in bytes.</span></span> <span data-ttu-id="c758a-119">Это значение должно быть несколько страниц размера базы данных, как с помощью параметра **pcbDbPageSize** возвращаемых функцией **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="c758a-119">This value must be a multiple of the database page size, as returned in the **pcbDbPageSize** parameter by the **ErrCheckDbHeaders** function.</span></span> 
    
### <a name="rgpageinfo"></a><span data-ttu-id="c758a-120">[rgPageInfo]</span><span class="sxs-lookup"><span data-stu-id="c758a-120">rgPageInfo[]</span></span> 
  
<span data-ttu-id="c758a-121">Параметр ввода вывода.</span><span class="sxs-lookup"><span data-stu-id="c758a-121">Input/output parameter.</span></span> <span data-ttu-id="c758a-122">Массив **Страница\_INFO** структуры, которые заполняет **ErrCheckDbPages** подробные результаты каждой странице базы данных, который копируется обратно.</span><span class="sxs-lookup"><span data-stu-id="c758a-122">An array of **PAGE\_INFO** structures that **ErrCheckDbPages** fills with detailed results of each database page that is checked.</span></span> <span data-ttu-id="c758a-123">Массив должен иметь один элемент для каждой базы данных страницы, переданной в параметр **pvPageBuffer** , а также поле **ulPgno** в каждом **Страница\_INFO** структуры должен иметь значение логической страницы номер, соответствующий на страницу базы данных.</span><span class="sxs-lookup"><span data-stu-id="c758a-123">The array must have one element for each database page passed in the **pvPageBuffer** parameter, and the **ulPgno** field in each **PAGE\_INFO** structure must be set to the logical page number that corresponds to the database page.</span></span> <span data-ttu-id="c758a-124">Дополнительные сведения см в разделе «Примечания» далее в этом разделе.</span><span class="sxs-lookup"><span data-stu-id="c758a-124">For more information, see "Remarks" later in this topic.</span></span> 
    
### <a name="cpageinfo"></a><span data-ttu-id="c758a-125">cPageInfo</span><span class="sxs-lookup"><span data-stu-id="c758a-125">cPageInfo</span></span>
  
<span data-ttu-id="c758a-126">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="c758a-126">Input parameter.</span></span> <span data-ttu-id="c758a-127">Число записей в массив **rgPageInfo []** .</span><span class="sxs-lookup"><span data-stu-id="c758a-127">The number of entries in the **rgPageInfo[]** array.</span></span> <span data-ttu-id="c758a-128">Это значение должно быть равно числу страниц базы данных, переданной в параметре **pvPageBuffer** .</span><span class="sxs-lookup"><span data-stu-id="c758a-128">This value must be equal to the number of database pages passed in the **pvPageBuffer** parameter.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="c758a-129">ulFlags</span><span class="sxs-lookup"><span data-stu-id="c758a-129">ulFlags</span></span> 
  
<span data-ttu-id="c758a-130">Необязательный параметр ввода.</span><span class="sxs-lookup"><span data-stu-id="c758a-130">Optional input parameter.</span></span> <span data-ttu-id="c758a-131">Это значение зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="c758a-131">This value is reserved for future use.</span></span> <span data-ttu-id="c758a-132">Значение, переданное в этот параметр должен быть нуль (0).</span><span class="sxs-lookup"><span data-stu-id="c758a-132">The value passed in this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="c758a-133">������������ ��������</span><span class="sxs-lookup"><span data-stu-id="c758a-133">Return value</span></span>

<span data-ttu-id="c758a-134">Код ошибки из перечисления [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="c758a-134">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c758a-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="c758a-135">Remarks</span></span>

<span data-ttu-id="c758a-136">Обратите внимание, что необходимо указаны в массиве баз данных, переданных функции **ErrInit** базы данных.</span><span class="sxs-lookup"><span data-stu-id="c758a-136">Note that you need to have specified the database in the array of databases passed to the **ErrInit** function.</span></span> <span data-ttu-id="c758a-137">Кроме того необходимо вызвать **ErrCheckDbHeaders** перед **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="c758a-137">Also, **ErrCheckDbHeaders** must be called before **ErrCheckDbPages**.</span></span>
  
<span data-ttu-id="c758a-138">Вызывающему приложению необходимо выделить буфер памяти, достаточное для хранения страниц базы данных для проверки.</span><span class="sxs-lookup"><span data-stu-id="c758a-138">The calling application must allocate a memory buffer that is large enough to hold the database pages to be checked.</span></span> <span data-ttu-id="c758a-139">Приложение отвечает за заполнение буфера содержимое одного или нескольких таких страниц базы данных.</span><span class="sxs-lookup"><span data-stu-id="c758a-139">The application is responsible for filling the buffer with the contents of one or more such database pages.</span></span> 
  
<span data-ttu-id="c758a-140">Вызывающему приложению необходимо вызвать **ErrCheckDbHeaders** перед вызовом **ErrCheckDbPages**.</span><span class="sxs-lookup"><span data-stu-id="c758a-140">The calling application must call **ErrCheckDbHeaders** before calling **ErrCheckDbPages**.</span></span> <span data-ttu-id="c758a-141">Эта функция может быть вызвана любое число раз на случай всех страниц на все файлы базы данных, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="c758a-141">This function can be called as many times as necessary to cover all the pages in all database files that are to be checked.</span></span>
  
<span data-ttu-id="c758a-142">В параметре **[] rgPageInfo** каждый возвращаемый элемент содержит сведения о странице базы данных в **Страница\_INFO** структуры.</span><span class="sxs-lookup"><span data-stu-id="c758a-142">In the **rgPageInfo[]** parameter, each element returned contains information about the database page in a **PAGE\_INFO** structure.</span></span> <span data-ttu-id="c758a-143">Если функция **ErrCheckDbPages** возвращает ошибку, приложение должно проверять каждый **Страница\_INFO** структуры, чтобы определить, на какую страницу обнаружены ошибки.</span><span class="sxs-lookup"><span data-stu-id="c758a-143">If the **ErrCheckDbPages** function returns an error, the application should check each **PAGE\_INFO** structure to determine on which page the error was found.</span></span> <span data-ttu-id="c758a-144">Например, для сравнения значения **checksumActual** и **checksumExpected** появится сообщение о том обнаружена ли ошибка контрольной суммой на этой странице базы данных.</span><span class="sxs-lookup"><span data-stu-id="c758a-144">For example, comparing the **checksumActual** and **checksumExpected** values will indicate whether a checksum error was detected on that database page.</span></span> 
  
<span data-ttu-id="c758a-145">Если **ErrCheckDbPages** обнаруживает все ошибки в базе данных контента, она будет создана запись в журнал событий Windows ошибки.</span><span class="sxs-lookup"><span data-stu-id="c758a-145">If **ErrCheckDbPages** detects any errors in the database content, it will create a Windows Error event log entry.</span></span> 
  
<span data-ttu-id="c758a-146">Объект **CChkSGFiles** определяет проверены ли все базы данных, зарегистрированные с помощью функции **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="c758a-146">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="c758a-147">В частности **CChkSGFiles** функция **ErrCheckDbPages** для определения предназначены ли такое же число страниц базы данных, указанный в параметре **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="c758a-147">Specifically, **CChkSGFiles** uses the **ErrCheckDbPages** function to determine whether the same number of database pages indicated by **ErrCheckDbHeaders** were actually verified.</span></span> <span data-ttu-id="c758a-148">Если не были успешно установлен правильный число страниц в каждой базе данных, функция **ErrTerm** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="c758a-148">If the correct number of pages in each database were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="c758a-149">Если вы используете многопоточного приложения CHKSGFILES, можно вызвать функцию **ErrCheckDbPages** в многопоточные части приложения.</span><span class="sxs-lookup"><span data-stu-id="c758a-149">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckDbPages** function in the multithreaded portion of the application.</span></span> <span data-ttu-id="c758a-150">Обратите внимание на то, что **ErrCheckDbPages** обычно вызывается несколько раз для каждой базы данных, который копируется обратно.</span><span class="sxs-lookup"><span data-stu-id="c758a-150">Note that **ErrCheckDbPages** is typically called multiple times for each database that is checked.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="c758a-151">Требования</span><span class="sxs-lookup"><span data-stu-id="c758a-151">Requirements</span></span>

<span data-ttu-id="c758a-152">Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="c758a-152">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="c758a-153">Учетная запись, приложения в разделе должен иметь разрешения на чтение базы данных и журналов файлов, которые должны быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="c758a-153">The account that the application is running under must have read permissions to the database and log files that are to be checked.</span></span>
  

