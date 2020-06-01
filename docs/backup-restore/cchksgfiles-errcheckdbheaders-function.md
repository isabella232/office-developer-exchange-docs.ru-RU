---
title: Функция функция cchksgfiles. Еррчеккдбхеадерс
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: a62c5940322d3d7a71f2db93214f1e970fc6859b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455249"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a><span data-ttu-id="1870a-103">Функция функция cchksgfiles. Еррчеккдбхеадерс</span><span class="sxs-lookup"><span data-stu-id="1870a-103">CChkSGFiles.ErrCheckDbHeaders function</span></span>

<span data-ttu-id="1870a-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="1870a-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span> 
  
<span data-ttu-id="1870a-105">Проверяет заголовки файлов базы данных, которые были указаны функцией **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="1870a-105">Validates the headers of the database files that were specified by the **ErrInit** function.</span></span> <span data-ttu-id="1870a-106">Эта функция также возвращает размер страницы и количество страниц в каждой из указанных баз данных.</span><span class="sxs-lookup"><span data-stu-id="1870a-106">This function also returns the page size and number of pages in each of the specified databases.</span></span> 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="1870a-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="1870a-107">Parameters</span></span>

### <a name="pcbdbpagesize"></a><span data-ttu-id="1870a-108">пкбдбпажесизе</span><span class="sxs-lookup"><span data-stu-id="1870a-108">pcbDbPageSize</span></span> 
  
<span data-ttu-id="1870a-109">Выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="1870a-109">Output parameter.</span></span> <span data-ttu-id="1870a-110">Размер страницы каждой из указанных баз данных в байтах.</span><span class="sxs-lookup"><span data-stu-id="1870a-110">The page size of each of the specified databases, in bytes.</span></span>
    
### <a name="pcheaderpagesperdb"></a><span data-ttu-id="1870a-111">пчеадерпажеспердб</span><span class="sxs-lookup"><span data-stu-id="1870a-111">pcHeaderPagesPerDb</span></span> 
  
<span data-ttu-id="1870a-112">Выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="1870a-112">Output parameter.</span></span> <span data-ttu-id="1870a-113">Количество страниц в начале каждой заданной базы данных, зарезервированных ядром СУБД для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="1870a-113">The number of pages at the beginning of each specified database that are reserved by the database engine for internal use.</span></span> <span data-ttu-id="1870a-114">Обратите внимание, что *не* следует передавать страницы заголовков в функцию **еррчеккдбпажес** для проверки.</span><span class="sxs-lookup"><span data-stu-id="1870a-114">Note that you should *not* pass header pages to the **ErrCheckDbPages** function for validation.</span></span> 
    
### <a name="pidberrorencountered"></a><span data-ttu-id="1870a-115">пидберроренкаунтеред</span><span class="sxs-lookup"><span data-stu-id="1870a-115">piDbErrorEncountered</span></span>
  
<span data-ttu-id="1870a-116">Выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="1870a-116">Output parameter.</span></span> <span data-ttu-id="1870a-117">Если возвращаемое значение функции указывает на ошибку, этот параметр будет индексом в массиве **ргвсздб []** , переданном функции **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="1870a-117">If the return value of the function indicates an error, this parameter will be an index into the **rgwszDb[]** array passed to the **ErrInit** function.</span></span> <span data-ttu-id="1870a-118">Элемент индексированного массива представляет базу данных, в которой произошла ошибка.</span><span class="sxs-lookup"><span data-stu-id="1870a-118">The indexed array element represents the database in which the error was encountered.</span></span> <span data-ttu-id="1870a-119">Если функция не возвращает значение ошибки, значение этого параметра не является допустимым.</span><span class="sxs-lookup"><span data-stu-id="1870a-119">If the function does not return an error value, this parameter value is invalid.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="1870a-120">ulFlags</span><span class="sxs-lookup"><span data-stu-id="1870a-120">ulFlags</span></span> 
  
<span data-ttu-id="1870a-121">Необязательный входной параметр.</span><span class="sxs-lookup"><span data-stu-id="1870a-121">Optional input parameter.</span></span> <span data-ttu-id="1870a-122">Это значение зарезервировано для использования в будущем.</span><span class="sxs-lookup"><span data-stu-id="1870a-122">This value is reserved for future use.</span></span> <span data-ttu-id="1870a-123">Передаваемое значение должно быть равно 0 (нулю).</span><span class="sxs-lookup"><span data-stu-id="1870a-123">The value passed should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="1870a-124">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="1870a-124">Return value</span></span>

<span data-ttu-id="1870a-125">Эта функция возвращает код ошибки из [перечисления функция cchksgfiles. ERR](cchksgfiles-err-enumeration.md).</span><span class="sxs-lookup"><span data-stu-id="1870a-125">This function returns an error code from the [CChkSGFiles.ERR enumeration](cchksgfiles-err-enumeration.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1870a-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="1870a-126">Remarks</span></span>

<span data-ttu-id="1870a-127">**Еррчеккдбхеадерс** проверяет, что все базы данных, зарегистрированные в **ерринит** , имеют одинаковую подпись журнала и размер страницы базы данных.</span><span class="sxs-lookup"><span data-stu-id="1870a-127">**ErrCheckDbHeaders** verifies that all databases registered with **ErrInit** have the same log signature and database page size.</span></span> <span data-ttu-id="1870a-128">Кроме того, можно использовать самое низкое значение параметра **женмин** и максимальное значение параметра **женмакс** , чтобы определить набор файлов журнала, необходимых для переноса всех зарегистрированных баз данных в состояние чистого отключения.</span><span class="sxs-lookup"><span data-stu-id="1870a-128">You can also use the lowest **genMin** parameter value and the highest **genMax** parameter value to determine the set of log files that are necessary to bring all of the registered databases to a clean-shutdown state.</span></span> 
  
<span data-ttu-id="1870a-129">Параметр **пидберроренкаунтеред** задается только при обнаружении ошибки, что определяется ненулевым возвращаемым значением **еррчеккдбхеадерс** .</span><span class="sxs-lookup"><span data-stu-id="1870a-129">The **piDbErrorEncountered** parameter is set only when an error is detected, as indicated by a non-zero **ErrCheckDbHeaders** return value.</span></span> 
  
<span data-ttu-id="1870a-130">При возникновении ошибки в этой функции в журнал событий ошибок Windows добавляется событие Error.</span><span class="sxs-lookup"><span data-stu-id="1870a-130">When an error occurs in this function, an error event will be added to the Windows Error event log.</span></span>
  
<span data-ttu-id="1870a-131">Вы можете вызвать **еррчеккдбхеадерс** только после вызова **ерринит**, и его необходимо вызвать перед вызовом **еррчеккдбпажес** и **еррчекклогс**.</span><span class="sxs-lookup"><span data-stu-id="1870a-131">You can call **ErrCheckDbHeaders** only after calling **ErrInit**, and you must call it before calling **ErrCheckDbPages** and **ErrCheckLogs**.</span></span>
  
<span data-ttu-id="1870a-132">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, вы должны вызвать функцию **еррчеккдбхеадерс** в однопотоковой части, и вы можете вызвать ее только один раз для каждого объекта **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="1870a-132">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrCheckDbHeaders** function in the single-threaded portion, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="1870a-133">Requirements</span><span class="sxs-lookup"><span data-stu-id="1870a-133">Requirements</span></span>

<span data-ttu-id="1870a-134">Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="1870a-134">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="1870a-135">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="1870a-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

