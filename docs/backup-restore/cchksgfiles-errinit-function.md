---
title: Функция функция cchksgfiles. Ерринит
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: 'Дата последнего изменения: 03 марта, 2013'
ms.openlocfilehash: d4b76933a747fe4bf084061cf080bc68264132ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760918"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="a4a44-103">Функция функция cchksgfiles. Ерринит</span><span class="sxs-lookup"><span data-stu-id="a4a44-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="a4a44-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="a4a44-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="a4a44-105">Инициализирует объект **функция cchksgfiles** , указывая проверяемые базы данных и путь и базовое имя файлов журнала транзакций, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="a4a44-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="a4a44-106">Приложения должны вызывать эту функцию сразу после успешного вызова **новой** функции.</span><span class="sxs-lookup"><span data-stu-id="a4a44-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
```cs
Vitual ERRErrInit  
(
    Const WCHAR  * const rgwszDb[],
    Const ULONGcDB,
    __in_z const WCHAR  * const wszLogPath,
    __in_z const WCHAR  * const wszBaseName,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="a4a44-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="a4a44-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="a4a44-108">Ргвсздб []</span><span class="sxs-lookup"><span data-stu-id="a4a44-108">rgwszDb[]</span></span>
  
<span data-ttu-id="a4a44-109">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="a4a44-109">Input parameter.</span></span> <span data-ttu-id="a4a44-110">Массив, указывающий базы данных, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="a4a44-110">An array that specifies the databases to be checked.</span></span> <span data-ttu-id="a4a44-111">Каждый элемент массива — это строка Юникода с завершающим нулем, которая содержит путь и имя файла проверяемой базы данных.</span><span class="sxs-lookup"><span data-stu-id="a4a44-111">Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="a4a44-112">cDB</span><span class="sxs-lookup"><span data-stu-id="a4a44-112">cDB</span></span>
  
<span data-ttu-id="a4a44-113">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="a4a44-113">Input parameter.</span></span> <span data-ttu-id="a4a44-114">Число допустимых элементов пути к базе данных в массиве **ргвсздб** .</span><span class="sxs-lookup"><span data-stu-id="a4a44-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="a4a44-115">всзлогпас</span><span class="sxs-lookup"><span data-stu-id="a4a44-115">wszLogPath</span></span>
  
<span data-ttu-id="a4a44-116">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="a4a44-116">Input parameter.</span></span> <span data-ttu-id="a4a44-117">Полный путь к файлам журнала транзакций, которые необходимо проверить, в виде строки Юникод с завершающим нулем.</span><span class="sxs-lookup"><span data-stu-id="a4a44-117">The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="a4a44-118">всзбасенаме</span><span class="sxs-lookup"><span data-stu-id="a4a44-118">wszBaseName</span></span>
  
<span data-ttu-id="a4a44-119">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="a4a44-119">Input parameter.</span></span> <span data-ttu-id="a4a44-120">3 – строчное имя файлов журнала транзакций Exchange в виде строки Юникода, заканчивающейся нулем.</span><span class="sxs-lookup"><span data-stu-id="a4a44-120">The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="a4a44-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="a4a44-121">ulFlags</span></span>
  
<span data-ttu-id="a4a44-122">Необязательный входной параметр.</span><span class="sxs-lookup"><span data-stu-id="a4a44-122">Optional input parameter.</span></span> <span data-ttu-id="a4a44-123">Это значение зарезервировано для использования в будущем.</span><span class="sxs-lookup"><span data-stu-id="a4a44-123">This value is reserved for future use.</span></span> <span data-ttu-id="a4a44-124">Значение, передаваемое этим параметром, должно быть равно 0 (нулю).</span><span class="sxs-lookup"><span data-stu-id="a4a44-124">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="a4a44-125">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="a4a44-125">Return value</span></span>

<span data-ttu-id="a4a44-126">Код ошибки из перечисления [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="a4a44-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a4a44-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="a4a44-127">Remarks</span></span>

<span data-ttu-id="a4a44-128">Функция **ерринит** регистрирует базы данных и файлы журналов, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="a4a44-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="a4a44-129">Эту функцию необходимо вызвать после вызова функции **New** , но перед вызовом любой другой функции **чксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="a4a44-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="a4a44-130">Необходимо указать все имена баз данных, путь к файлу журнала и базовое имя как строки Юникод, заканчивающиеся нулем.</span><span class="sxs-lookup"><span data-stu-id="a4a44-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="a4a44-131">Вы можете проверять только файлы баз данных, файлы журнала или базы данных и файлы журналов.</span><span class="sxs-lookup"><span data-stu-id="a4a44-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="a4a44-132">Однако при вызове этой функции приложение должно указать по крайней мере одну сущность для проверки.</span><span class="sxs-lookup"><span data-stu-id="a4a44-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="a4a44-133">Если передать значение 0 (ноль) для **cDB** и NULL для **всзлогпас** , будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="a4a44-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="a4a44-134">Если значение **cDB** отлично от 0 (ноль), то при передаче значения NULL для **ргвсздб** будет возникать ошибка.</span><span class="sxs-lookup"><span data-stu-id="a4a44-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="a4a44-135">Для проверки файлов базы данных приложение должно предоставить имена баз данных.</span><span class="sxs-lookup"><span data-stu-id="a4a44-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="a4a44-136">Если для **всзбасенаме** передается значение null, но **всзлогпас** не NULL, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="a4a44-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="a4a44-137">При проверке файлов журнала всегда необходимо указывать базовое имя файла журнала.</span><span class="sxs-lookup"><span data-stu-id="a4a44-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="a4a44-138">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, необходимо вызвать функцию **ерринит** в однопотоковой части приложения, и вы можете вызвать его только один раз для каждого объекта **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="a4a44-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="a4a44-139">Requirements</span><span class="sxs-lookup"><span data-stu-id="a4a44-139">Requirements</span></span>

<span data-ttu-id="a4a44-140">Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="a4a44-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="a4a44-141">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="a4a44-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

