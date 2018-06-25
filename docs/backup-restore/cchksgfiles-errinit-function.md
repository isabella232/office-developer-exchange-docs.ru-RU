---
title: Функция CChkSGFiles.ErrInit
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
description: 'Последнее изменение: 03 марта 2013 г.'
ms.openlocfilehash: d4b76933a747fe4bf084061cf080bc68264132ed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760918"
---
# <a name="cchksgfileserrinit-function"></a><span data-ttu-id="f7d97-103">Функция CChkSGFiles.ErrInit</span><span class="sxs-lookup"><span data-stu-id="f7d97-103">CChkSGFiles.ErrInit function</span></span>
  
<span data-ttu-id="f7d97-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="f7d97-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="f7d97-105">Инициализирует объект **CChkSGFiles** путем указания баз данных для проверки, а также путь и базовое имя файлы журнала транзакций для проверки.</span><span class="sxs-lookup"><span data-stu-id="f7d97-105">Initializes the **CChkSGFiles** object by specifying the databases to be checked and the path and base name of the transaction log files to be checked.</span></span> <span data-ttu-id="f7d97-106">Приложения должны вызвать эту функцию сразу же после успешного вызова функции **New** .</span><span class="sxs-lookup"><span data-stu-id="f7d97-106">Applications should call this function immediately after successfully calling the **New** function.</span></span> 
  
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

## <a name="parameters"></a><span data-ttu-id="f7d97-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="f7d97-107">Parameters</span></span>

### <a name="rgwszdb"></a><span data-ttu-id="f7d97-108">[rgwszDb]</span><span class="sxs-lookup"><span data-stu-id="f7d97-108">rgwszDb[]</span></span>
  
<span data-ttu-id="f7d97-109">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="f7d97-109">Input parameter.</span></span> <span data-ttu-id="f7d97-110">Массив, который определяет баз данных для проверки.</span><span class="sxs-lookup"><span data-stu-id="f7d97-110">An array that specifies the databases to be checked.</span></span> <span data-ttu-id="f7d97-111">Каждый элемент массива является символом null строки Юникод в строку, содержащую путь и имя базы данных для проверки.</span><span class="sxs-lookup"><span data-stu-id="f7d97-111">Each array element is a null-terminated Unicode string that contains the path and file name of a database to be checked.</span></span>
    
### <a name="cdb"></a><span data-ttu-id="f7d97-112">cDB</span><span class="sxs-lookup"><span data-stu-id="f7d97-112">cDB</span></span>
  
<span data-ttu-id="f7d97-113">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="f7d97-113">Input parameter.</span></span> <span data-ttu-id="f7d97-114">Число элементов путь допустимый базы данных в массиве **rgwszDb** .</span><span class="sxs-lookup"><span data-stu-id="f7d97-114">The number of valid database path elements in the **rgwszDb** array.</span></span> 
    
#### <a name="wszlogpath"></a><span data-ttu-id="f7d97-115">wszLogPath</span><span class="sxs-lookup"><span data-stu-id="f7d97-115">wszLogPath</span></span>
  
<span data-ttu-id="f7d97-116">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="f7d97-116">Input parameter.</span></span> <span data-ttu-id="f7d97-117">Полный путь должен быть установлен, в формате Юникод, идентифицирующий файлы журнала транзакций.</span><span class="sxs-lookup"><span data-stu-id="f7d97-117">The full path of the transaction log files to be checked, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="wszbasename"></a><span data-ttu-id="f7d97-118">wszBaseName</span><span class="sxs-lookup"><span data-stu-id="f7d97-118">wszBaseName</span></span>
  
<span data-ttu-id="f7d97-119">Входного параметра.</span><span class="sxs-lookup"><span data-stu-id="f7d97-119">Input parameter.</span></span> <span data-ttu-id="f7d97-120">Базовое имя трехсимвольный, файлы журнала транзакций Exchange, в формате строки Юникод символом null.</span><span class="sxs-lookup"><span data-stu-id="f7d97-120">The three-letter base name of the Exchange transaction log files, in the form of a null-terminated Unicode string.</span></span>
    
### <a name="ulflags"></a><span data-ttu-id="f7d97-121">ulFlags</span><span class="sxs-lookup"><span data-stu-id="f7d97-121">ulFlags</span></span>
  
<span data-ttu-id="f7d97-122">Необязательный параметр ввода.</span><span class="sxs-lookup"><span data-stu-id="f7d97-122">Optional input parameter.</span></span> <span data-ttu-id="f7d97-123">Это значение зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="f7d97-123">This value is reserved for future use.</span></span> <span data-ttu-id="f7d97-124">Значение, переданное в этом параметре должны быть нуль (0).</span><span class="sxs-lookup"><span data-stu-id="f7d97-124">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="f7d97-125">������������ ��������</span><span class="sxs-lookup"><span data-stu-id="f7d97-125">Return value</span></span>

<span data-ttu-id="f7d97-126">Код ошибки из перечисления [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="f7d97-126">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f7d97-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="f7d97-127">Remarks</span></span>

<span data-ttu-id="f7d97-128">Функция **ErrInit** регистрирует баз данных и файлов журнала, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="f7d97-128">The **ErrInit** function registers the databases and log files that are to be checked.</span></span> <span data-ttu-id="f7d97-129">Эта функция должна вызываться после вызова функции **New** , но до любые другие **ChkSGFiles** вызова функции.</span><span class="sxs-lookup"><span data-stu-id="f7d97-129">This function must be called after the **New** function is called but before any other **ChkSGFiles** function is called.</span></span> 
  
<span data-ttu-id="f7d97-130">Как символом null строки Юникод, необходимо предоставить все имена баз данных, базовое имя и путь к файлу журнала.</span><span class="sxs-lookup"><span data-stu-id="f7d97-130">You must provide all the database names, the log file path, and the base name as null-terminated Unicode strings.</span></span>
  
<span data-ttu-id="f7d97-131">Чтобы проверить только файлы базы данных, только файлы журнала или файлы базы данных и журналов.</span><span class="sxs-lookup"><span data-stu-id="f7d97-131">You can check only the database files, only the log files, or both the database and log files.</span></span> <span data-ttu-id="f7d97-132">Тем не менее при вызове этой функции приложения необходимо указать хотя бы один объект для проверки.</span><span class="sxs-lookup"><span data-stu-id="f7d97-132">However, when calling this function, the application must specify at least one entity to be checked.</span></span> <span data-ttu-id="f7d97-133">Передача нуль (0) для **cDB** и NULL для **wszLogPath** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="f7d97-133">Passing 0 (zero) for  **cDB**  and NULL for  **wszLogPath**  will return an error.</span></span> 
  
<span data-ttu-id="f7d97-134">Если значение **cDB** отличный от 0 (ноль), указать значение NULL для **rgwszDb** приведет к ошибке.</span><span class="sxs-lookup"><span data-stu-id="f7d97-134">If the value of  **cDB**  is other than 0 (zero), passing NULL for  **rgwszDb**  will result in an error.</span></span> <span data-ttu-id="f7d97-135">Чтобы проверить файлы базы данных, приложение должно предоставлять имена баз данных.</span><span class="sxs-lookup"><span data-stu-id="f7d97-135">To check the database files, the application must provide the database names.</span></span> 
  
<span data-ttu-id="f7d97-136">Если передается **wszBaseName** , но **wszLogPath** не имеет значение NULL, будут возвращены ошибку.</span><span class="sxs-lookup"><span data-stu-id="f7d97-136">If NULL is passed for  **wszBaseName**  but  **wszLogPath**  is not NULL, an error will be returned.</span></span> <span data-ttu-id="f7d97-137">Базовое имя файла журнала всегда является обязательным при проверке файлов журнала.</span><span class="sxs-lookup"><span data-stu-id="f7d97-137">A log file base name is always required when checking log files.</span></span> 
  
<span data-ttu-id="f7d97-138">Если вы используете многопоточного приложения CHKSGFILES, необходимо вызвать функцию **ErrInit** в одном потоке части приложения и его можно вызвать только один раз для каждого объекта **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="f7d97-138">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrInit** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="f7d97-139">Требования</span><span class="sxs-lookup"><span data-stu-id="f7d97-139">Requirements</span></span>

<span data-ttu-id="f7d97-140">Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="f7d97-140">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="f7d97-141">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="f7d97-141">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

