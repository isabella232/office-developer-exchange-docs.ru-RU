---
title: Функция CChkSGFiles.ErrCheckLogs
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckLogs
api_type:
- dllExport
ms.assetid: cec0df4b-4679-4682-bacf-69b4f4aef343
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: 5b1070de73bc23ae09ddb7835bd72c8e8a71a95f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760922"
---
# <a name="cchksgfileserrchecklogs-function"></a><span data-ttu-id="ffaf7-103">Функция CChkSGFiles.ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="ffaf7-103">CChkSGFiles.ErrCheckLogs function</span></span>

<span data-ttu-id="ffaf7-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="ffaf7-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="ffaf7-105">Проверка файлов журнала всех файлов базы данных, которые были указаны в функции **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="ffaf7-105">Validates the log files of all the database files that were specified in the **ErrInit** function.</span></span> <span data-ttu-id="ffaf7-106">Проверенный журналы — это списки, находящихся в пути, а, у которых имя файла журнала базового трех букв, переданной в **ErrInit**.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-106">The validated logs are those that exist in the path, and that have the three-letter base log file name passed to **ErrInit**.</span></span>
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="ffaf7-107">Parameters</span><span class="sxs-lookup"><span data-stu-id="ffaf7-107">Parameters</span></span>

### <a name="pfonlyunnecessarylogscorrupt"></a><span data-ttu-id="ffaf7-108">pfOnlyUnnecessaryLogsCorrupt</span><span class="sxs-lookup"><span data-stu-id="ffaf7-108">pfOnlyUnnecessaryLogsCorrupt</span></span> 
  
<span data-ttu-id="ffaf7-109">Выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-109">Output parameter.</span></span> <span data-ttu-id="ffaf7-110">Если **значение true**, этот параметр указывает, что в файлы журнала транзакций, но эти ошибки обнаружены ошибки были все найденные в файлах журнала, которые не требуются для приведения базы данных в состояние чистого отключения без потери данных.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-110">When **true**, this parameter indicates that errors were found in the transaction log files, but those errors were all found in log files that are not needed to bring the database to a clean-shutdown state without data loss.</span></span> <span data-ttu-id="ffaf7-111">Значение **true** , возвращаемых в этот параметр действителен только в том случае, если **ErrCheckLogs** возвращает **errSuccess**.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-111">A **true** value returned in this parameter is valid only when **ErrCheckLogs** returns **errSuccess**.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="ffaf7-112">ulFlags</span><span class="sxs-lookup"><span data-stu-id="ffaf7-112">ulFlags</span></span>
  
<span data-ttu-id="ffaf7-113">Необязательный параметр ввода.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-113">Optional input parameter.</span></span> <span data-ttu-id="ffaf7-114">Это значение зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-114">This value is reserved for future use.</span></span> <span data-ttu-id="ffaf7-115">Значение, переданное в этом параметре должны быть нуль (0).</span><span class="sxs-lookup"><span data-stu-id="ffaf7-115">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="ffaf7-116">������������ ��������</span><span class="sxs-lookup"><span data-stu-id="ffaf7-116">Return value</span></span>

<span data-ttu-id="ffaf7-117">Код ошибки из перечисления [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="ffaf7-117">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
<span data-ttu-id="ffaf7-118">Важно помнить, что эта функция может вернуть **errSuccess** даже в том случае, если найдены ошибки в файлах журналов.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-118">It's important to remember that this function can return **errSuccess** even when errors are found in the log files.</span></span> <span data-ttu-id="ffaf7-119">Таким образом при возвращении **errSuccess** **ErrCheckLogs** приложения также должен проверить, возвращаемого параметра **pfOnlyUnnecessaryLogsCorrupt** .</span><span class="sxs-lookup"><span data-stu-id="ffaf7-119">Therefore, when **ErrCheckLogs** returns **errSuccess**, the application should also check the  **pfOnlyUnnecessaryLogsCorrupt** return parameter.</span></span> <span data-ttu-id="ffaf7-120">Если **pfOnlyUnnecessaryLogsCorrupts** имеет **значение true** , если **ErrCheckLogs** возвращает **errSuccess**, это указывает на то, что один или несколько были найдены ошибки, но только в файлы журналов не требуется, чтобы перевести базу данных.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-120">If **pfOnlyUnnecessaryLogsCorrupts** is **true** when **ErrCheckLogs** returns **errSuccess**, this indicates that one or more errors were found, but only in log files not needed to bring the database up-to-date.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ffaf7-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="ffaf7-121">Remarks</span></span>

<span data-ttu-id="ffaf7-122">Функция **ErrCheckDbHeaders** должна вызываться перед можно вызвать функцию **ErrCheckLogs** .</span><span class="sxs-lookup"><span data-stu-id="ffaf7-122">The **ErrCheckDbHeaders** function must be called before the **ErrCheckLogs** function can be called.</span></span> 
  
<span data-ttu-id="ffaf7-123">При извлечении файлы журнала транзакций базы данных Exchange, некоторые файлы журнала будет необходимые для обновления баз данных в группе хранения в состояние чистого отключения без потери данных, в то время как другие файлы журналов может не потребоваться.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-123">When Exchange database transaction log files are being checked, some of the log files will be necessary to bring the databases in the storage group to a clean-shutdown state without data loss, whereas other log files might not be needed.</span></span> <span data-ttu-id="ffaf7-124">Функция **ErrCheckLogs** определяет наиболее старых и новых файлы журнала, которые требуются для переноса базы данных в актуальном состоянии.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-124">The **ErrCheckLogs** function determines both the oldest and the newest log files that are needed to bring the databases up to date.</span></span> 
  
<span data-ttu-id="ffaf7-125">Функция **ErrCheckLogs** проверяет все файлы журналов в указанного пути, также имеют указанного трех букв базового имени файла, как переданных функции **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="ffaf7-125">The **ErrCheckLogs** function verifies all the log files in the specified paths that also have the specified three-letter base file name, as passed to the **ErrInit** function.</span></span> 
  
<span data-ttu-id="ffaf7-126">Если ошибок не найдено в файлах журналов, **ErrCheckLogs** возвращает **errSuccess**.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-126">If no errors are found in the log files, **ErrCheckLogs** returns **errSuccess**.</span></span> 
  
<span data-ttu-id="ffaf7-127">Если любой из файлов журналов найдены поврежден, **ErrCheckLogs** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-127">If any of the required log files are found to be corrupted, **ErrCheckLogs** returns an error.</span></span> 
  
<span data-ttu-id="ffaf7-128">При наличии ошибок только в файлах журнала, возраст которых превышает ранней из них требуется, функция возвращает **errSuccess** и задает возвращаемый параметр **pfOnlyUnnecessaryLogCorrupt** значение **true**.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-128">If errors are found only in log files that are older than the earliest ones needed, the function returns **errSuccess** and sets the return parameter **pfOnlyUnnecessaryLogCorrupt** to **true**.</span></span> <span data-ttu-id="ffaf7-129">Приложение должно распознавать, что в некоторых из этих старые файлы журнала ошибок, и если да, он будет уведомить пользователя.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-129">The application should recognize that there are errors in some of those old log files, and if so, it will possibly alert the user.</span></span> <span data-ttu-id="ffaf7-130">В любом случае эти ошибки не влияет на общее целостности базы данных или влияет на воспроизведение журналов переадресовывать будет выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-130">In any case, those errors should not affect the overall integrity of the database or affect whether playing the logs forward will succeed.</span></span>
  
<span data-ttu-id="ffaf7-131">При наличии ошибок в любом файле журнала, созданная после самая ранняя необходимые журнала, который определяет **ErrCheckLogs** , функция возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-131">If errors are found in any log file created after the earliest log that **ErrCheckLogs** determines is needed, the function returns an error.</span></span> <span data-ttu-id="ffaf7-132">Ошибки будут возвращены, даже если обнаружена ошибка файла журнала в файл журнала, который был создан более поздней версии, чем является необходимые для перевода базы данных в актуальном состоянии.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-132">The error will be returned even if the log file error was found in a log file that was generated later than what is needed to bring the database up to date.</span></span> <span data-ttu-id="ffaf7-133">Несмотря на то, что можно было бы для переноса баз данных в состояние чистого отключения с помощью файлов определенного журнала, операций, указанных в файлах позднее поврежденный журнал будет не применяется, что приводит к потере данных при восстановлении базы данных.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-133">Although it would be possible to bring the databases to a clean-shutdown state by using the identified log files, transactions specified in the later corrupted log files would not be applied, resulting in data loss when the database is restored.</span></span> 
  
<span data-ttu-id="ffaf7-134">Объект **CChkSGFiles** определяет, будет ли все файлы журнала, зарегистрированные с помощью функции **ErrInit** фактически были возвращены.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-134">The **CChkSGFiles** object determines whether all of the log files registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="ffaf7-135">Если не всех журналов были не установлен успешно, функция **ErrTerm** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-135">If not all of the logs were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="ffaf7-136">Если вы используете многопоточного приложения CHKSGFILES, можно вызвать функцию **ErrCheckLogs** в многопоточные части приложения, но его можно вызвать только один раз для каждого объекта **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="ffaf7-136">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckLogs** function in the multithreaded portion of the application, but you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="ffaf7-137">Требования</span><span class="sxs-lookup"><span data-stu-id="ffaf7-137">Requirements</span></span>

<span data-ttu-id="ffaf7-138">Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-138">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="ffaf7-139">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="ffaf7-139">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

