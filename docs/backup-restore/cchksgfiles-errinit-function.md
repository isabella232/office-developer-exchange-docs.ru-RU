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
ms.openlocfilehash: c881691e7c1ba83a396e659f6aac0328625e49a5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457013"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="f2049-103">Функция функция cchksgfiles. Ерринит</span><span class="sxs-lookup"><span data-stu-id="f2049-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="f2049-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="f2049-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="f2049-105">Инициализирует объект **функция cchksgfiles** , указывая проверяемые базы данных и путь и базовое имя файлов журнала транзакций, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="f2049-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="f2049-106">Приложения должны вызывать эту функцию сразу после успешного вызова **новой** функции.</span><span class="sxs-lookup"><span data-stu-id="f2049-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="f2049-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="f2049-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="f2049-108">Ргвсздб []</span><span class="sxs-lookup"><span data-stu-id="f2049-108">rgwszDb[]</span></span>
  
<span data-ttu-id="f2049-109">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="f2049-109">Input parameter.</span></span> <span data-ttu-id="f2049-110">Массив, указывающий базы данных, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="f2049-110">An array that specifies the databases to be checked.</span></span> <span data-ttu-id="f2049-111">Каждый элемент массива — это строка Юникода с завершающим нулем, которая содержит путь и имя файла проверяемой базы данных.</span><span class="sxs-lookup"><span data-stu-id="f2049-111">Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="f2049-112">cDB</span><span class="sxs-lookup"><span data-stu-id="f2049-112">cDB</span></span>
  
<span data-ttu-id="f2049-113">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="f2049-113">Input parameter.</span></span> <span data-ttu-id="f2049-114">Число допустимых элементов пути к базе данных в массиве **ргвсздб** .</span><span class="sxs-lookup"><span data-stu-id="f2049-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="f2049-115">всзлогпас</span><span class="sxs-lookup"><span data-stu-id="f2049-115">wszLogPath</span></span>
  
<span data-ttu-id="f2049-116">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="f2049-116">Input parameter.</span></span> <span data-ttu-id="f2049-117">Полный путь к файлам журнала транзакций, которые необходимо проверить, в виде строки Юникод с завершающим нулем.</span><span class="sxs-lookup"><span data-stu-id="f2049-117">The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="f2049-118">всзбасенаме</span><span class="sxs-lookup"><span data-stu-id="f2049-118">wszBaseName</span></span>
  
<span data-ttu-id="f2049-119">Входной параметр.</span><span class="sxs-lookup"><span data-stu-id="f2049-119">Input parameter.</span></span> <span data-ttu-id="f2049-120">3 – строчное имя файлов журнала транзакций Exchange в виде строки Юникода, заканчивающейся нулем.</span><span class="sxs-lookup"><span data-stu-id="f2049-120">The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="f2049-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="f2049-121">ulFlags</span></span>
  
<span data-ttu-id="f2049-122">Необязательный входной параметр.</span><span class="sxs-lookup"><span data-stu-id="f2049-122">Optional input parameter.</span></span> <span data-ttu-id="f2049-123">Это значение зарезервировано для использования в будущем.</span><span class="sxs-lookup"><span data-stu-id="f2049-123">This value is reserved for future use.</span></span> <span data-ttu-id="f2049-124">Значение, передаваемое этим параметром, должно быть равно 0 (нулю).</span><span class="sxs-lookup"><span data-stu-id="f2049-124">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="f2049-125">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="f2049-125">Return value</span></span>

<span data-ttu-id="f2049-126">Код ошибки из перечисления [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="f2049-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f2049-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="f2049-127">Remarks</span></span>

<span data-ttu-id="f2049-128">Функция **ерринит** регистрирует базы данных и файлы журналов, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="f2049-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="f2049-129">Эту функцию необходимо вызвать после вызова функции **New** , но перед вызовом любой другой функции **чксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="f2049-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="f2049-130">Необходимо указать все имена баз данных, путь к файлу журнала и базовое имя как строки Юникод, заканчивающиеся нулем.</span><span class="sxs-lookup"><span data-stu-id="f2049-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="f2049-131">Вы можете проверять только файлы баз данных, файлы журнала или базы данных и файлы журналов.</span><span class="sxs-lookup"><span data-stu-id="f2049-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="f2049-132">Однако при вызове этой функции приложение должно указать по крайней мере одну сущность для проверки.</span><span class="sxs-lookup"><span data-stu-id="f2049-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="f2049-133">Если передать значение 0 (ноль) для **cDB** и NULL для **всзлогпас** , будет возвращена ошибка.</span><span class="sxs-lookup"><span data-stu-id="f2049-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="f2049-134">Если значение **cDB** отлично от 0 (ноль), то при передаче значения NULL для **ргвсздб** будет возникать ошибка.</span><span class="sxs-lookup"><span data-stu-id="f2049-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="f2049-135">Для проверки файлов базы данных приложение должно предоставить имена баз данных.</span><span class="sxs-lookup"><span data-stu-id="f2049-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="f2049-136">Если для **всзбасенаме** передается значение null, но **всзлогпас** не NULL, возвращается ошибка.</span><span class="sxs-lookup"><span data-stu-id="f2049-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="f2049-137">При проверке файлов журнала всегда необходимо указывать базовое имя файла журнала.</span><span class="sxs-lookup"><span data-stu-id="f2049-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="f2049-138">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, необходимо вызвать функцию **ерринит** в однопотоковой части приложения, и вы можете вызвать его только один раз для каждого объекта **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="f2049-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="f2049-139">Requirements</span><span class="sxs-lookup"><span data-stu-id="f2049-139">Requirements</span></span>

<span data-ttu-id="f2049-140">Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="f2049-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="f2049-141">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="f2049-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

