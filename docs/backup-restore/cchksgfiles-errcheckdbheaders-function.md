---
title: Функция CChkSGFiles.ErrCheckDbHeaders
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
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: a407019063b34970e883a00ca4f4d730935d7cba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760926"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a><span data-ttu-id="6e60f-103">Функция CChkSGFiles.ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="6e60f-103">CChkSGFiles.ErrCheckDbHeaders function</span></span>

<span data-ttu-id="6e60f-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="6e60f-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span> 
  
<span data-ttu-id="6e60f-105">Проверяет заголовки файлов базы данных, которые были указаны с помощью функции **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="6e60f-105">Validates the headers of the database files that were specified by the **ErrInit** function.</span></span> <span data-ttu-id="6e60f-106">Эта функция также возвращает размер страницы и число страниц в каждой указанной базы данных.</span><span class="sxs-lookup"><span data-stu-id="6e60f-106">This function also returns the page size and number of pages in each of the specified databases.</span></span> 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="6e60f-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="6e60f-107">Parameters</span></span>

### <a name="pcbdbpagesize"></a><span data-ttu-id="6e60f-108">pcbDbPageSize</span><span class="sxs-lookup"><span data-stu-id="6e60f-108">pcbDbPageSize</span></span> 
  
<span data-ttu-id="6e60f-109">Выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="6e60f-109">Output parameter.</span></span> <span data-ttu-id="6e60f-110">Размер страницы каждой указанной базы данных, в байтах.</span><span class="sxs-lookup"><span data-stu-id="6e60f-110">The page size of each of the specified databases, in bytes.</span></span>
    
### <a name="pcheaderpagesperdb"></a><span data-ttu-id="6e60f-111">pcHeaderPagesPerDb</span><span class="sxs-lookup"><span data-stu-id="6e60f-111">pcHeaderPagesPerDb</span></span> 
  
<span data-ttu-id="6e60f-112">Выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="6e60f-112">Output parameter.</span></span> <span data-ttu-id="6e60f-113">Число страниц в начале каждой указанной базы данных, зарезервированные ядро базы данных для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="6e60f-113">The number of pages at the beginning of each specified database that are reserved by the database engine for internal use.</span></span> <span data-ttu-id="6e60f-114">Обратите внимание, что вы должны *прохода страницы заголовка в функцию **ErrCheckDbPages** для проверки* .</span><span class="sxs-lookup"><span data-stu-id="6e60f-114">Note that you should *not* pass header pages to the **ErrCheckDbPages** function for validation.</span></span> 
    
### <a name="pidberrorencountered"></a><span data-ttu-id="6e60f-115">piDbErrorEncountered</span><span class="sxs-lookup"><span data-stu-id="6e60f-115">piDbErrorEncountered</span></span>
  
<span data-ttu-id="6e60f-116">Выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="6e60f-116">Output parameter.</span></span> <span data-ttu-id="6e60f-117">Если возвращаемое значение функции, указывающий на ошибки, данный параметр будет индекса в массив **rgwszDb []** , переданное в функцию **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="6e60f-117">If the return value of the function indicates an error, this parameter will be an index into the **rgwszDb[]** array passed to the **ErrInit** function.</span></span> <span data-ttu-id="6e60f-118">Индексированный элемент массива представляет базу данных, в котором возникла ошибка.</span><span class="sxs-lookup"><span data-stu-id="6e60f-118">The indexed array element represents the database in which the error was encountered.</span></span> <span data-ttu-id="6e60f-119">Если функция не возвращает ошибку, значение этого параметра является недопустимым.</span><span class="sxs-lookup"><span data-stu-id="6e60f-119">If the function does not return an error value, this parameter value is invalid.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="6e60f-120">ulFlags</span><span class="sxs-lookup"><span data-stu-id="6e60f-120">ulFlags</span></span> 
  
<span data-ttu-id="6e60f-121">Необязательный параметр ввода.</span><span class="sxs-lookup"><span data-stu-id="6e60f-121">Optional input parameter.</span></span> <span data-ttu-id="6e60f-122">Это значение зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="6e60f-122">This value is reserved for future use.</span></span> <span data-ttu-id="6e60f-123">Значение, переданное должны быть нуль (0).</span><span class="sxs-lookup"><span data-stu-id="6e60f-123">The value passed should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="6e60f-124">������������ ��������</span><span class="sxs-lookup"><span data-stu-id="6e60f-124">Return value</span></span>

<span data-ttu-id="6e60f-125">Эта функция возвращает код ошибки из [перечисления CChkSGFiles.ERR](cchksgfiles-err-enumeration.md).</span><span class="sxs-lookup"><span data-stu-id="6e60f-125">This function returns an error code from the [CChkSGFiles.ERR enumeration](cchksgfiles-err-enumeration.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e60f-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="6e60f-126">Remarks</span></span>

<span data-ttu-id="6e60f-127">**ErrCheckDbHeaders** проверяет, что все базы данных, зарегистрированные с **ErrInit** же журнала подписи и база данных размер страницы.</span><span class="sxs-lookup"><span data-stu-id="6e60f-127">**ErrCheckDbHeaders** verifies that all databases registered with **ErrInit** have the same log signature and database page size.</span></span> <span data-ttu-id="6e60f-128">Минимальное значение параметра **genMin** и наибольшее значение параметра **genMax** также можно использовать для определения набора файлов журнала, которые необходимо установить все зарегистрированные базы данных в состояние чистого отключения.</span><span class="sxs-lookup"><span data-stu-id="6e60f-128">You can also use the lowest **genMin** parameter value and the highest **genMax** parameter value to determine the set of log files that are necessary to bring all of the registered databases to a clean-shutdown state.</span></span> 
  
<span data-ttu-id="6e60f-129">Параметр **piDbErrorEncountered** имеет значение только в том случае, если обнаружена ошибка, как указано в отличное от нуля **ErrCheckDbHeaders** возвращаемое значение.</span><span class="sxs-lookup"><span data-stu-id="6e60f-129">The **piDbErrorEncountered** parameter is set only when an error is detected, as indicated by a non-zero **ErrCheckDbHeaders** return value.</span></span> 
  
<span data-ttu-id="6e60f-130">При возникновении ошибки в этой функции, событие ошибки будут добавлены в журнал событий Windows ошибки.</span><span class="sxs-lookup"><span data-stu-id="6e60f-130">When an error occurs in this function, an error event will be added to the Windows Error event log.</span></span>
  
<span data-ttu-id="6e60f-131">Можно вызвать **ErrCheckDbHeaders** только после вызова **ErrInit**и его необходимо вызвать до вызова метода **ErrCheckDbPages** и **ErrCheckLogs**.</span><span class="sxs-lookup"><span data-stu-id="6e60f-131">You can call **ErrCheckDbHeaders** only after calling **ErrInit**, and you must call it before calling **ErrCheckDbPages** and **ErrCheckLogs**.</span></span>
  
<span data-ttu-id="6e60f-132">Если вы используете многопоточного приложения CHKSGFILES, необходимо вызвать функцию **ErrCheckDbHeaders** в части одного потока, и его можно вызвать только один раз для каждого объекта **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="6e60f-132">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrCheckDbHeaders** function in the single-threaded portion, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="6e60f-133">Требования</span><span class="sxs-lookup"><span data-stu-id="6e60f-133">Requirements</span></span>

<span data-ttu-id="6e60f-134">Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="6e60f-134">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="6e60f-135">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="6e60f-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

