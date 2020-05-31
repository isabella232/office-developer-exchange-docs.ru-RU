---
title: Функция функция cchksgfiles. Еррчекклогс
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
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: 5b1070de73bc23ae09ddb7835bd72c8e8a71a95f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760922"
---
# <a name="cchksgfileserrchecklogs-function"></a><span data-ttu-id="b9d6b-103">Функция функция cchksgfiles. Еррчекклогс</span><span class="sxs-lookup"><span data-stu-id="b9d6b-103">CChkSGFiles.ErrCheckLogs function</span></span>

<span data-ttu-id="b9d6b-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b9d6b-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="b9d6b-105">Проверяет файлы журнала всех файлов базы данных, указанных в функции **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="b9d6b-105">Validates the log files of all the database files that were specified in the **ErrInit** function.</span></span> <span data-ttu-id="b9d6b-106">Проверенные журналы — это те, которые существуют в пути, и имя файла журнала из трех букв передается в **ерринит**.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-106">The validated logs are those that exist in the path, and that have the three-letter base log file name passed to **ErrInit**.</span></span>
  
```cs
Vitual ERRErrCheckLogs 
(
        BOOL  * const pfOnlyUnnecessaryLogsCorrup,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="b9d6b-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="b9d6b-107">Parameters</span></span>

### <a name="pfonlyunnecessarylogscorrupt"></a><span data-ttu-id="b9d6b-108">пфонлюннецессарилогскоррупт</span><span class="sxs-lookup"><span data-stu-id="b9d6b-108">pfOnlyUnnecessaryLogsCorrupt</span></span> 
  
<span data-ttu-id="b9d6b-109">Выходной параметр.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-109">Output parameter.</span></span> <span data-ttu-id="b9d6b-110">Если задано **значение true**, этот параметр указывает на то, что в файлах журнала транзакций обнаружены ошибки, но все эти ошибки были найдены в файлах журнала, которые не требовалось для переноса базы данных в состояние чистого отключения без потери данных.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-110">When **true**, this parameter indicates that errors were found in the transaction log files, but those errors were all found in log files that are not needed to bring the database to a clean-shutdown state without data loss.</span></span> <span data-ttu-id="b9d6b-111">Значение **true** , возвращаемое в этом параметре, допустимо только в том случае, если **еррчекклогс** возвращает **еррсукцесс**.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-111">A **true** value returned in this parameter is valid only when **ErrCheckLogs** returns **errSuccess**.</span></span> 
    
### <a name="ulflags"></a><span data-ttu-id="b9d6b-112">ulFlags</span><span class="sxs-lookup"><span data-stu-id="b9d6b-112">ulFlags</span></span>
  
<span data-ttu-id="b9d6b-113">Необязательный входной параметр.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-113">Optional input parameter.</span></span> <span data-ttu-id="b9d6b-114">Это значение зарезервировано для использования в будущем.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-114">This value is reserved for future use.</span></span> <span data-ttu-id="b9d6b-115">Значение, передаваемое этим параметром, должно быть равно 0 (нулю).</span><span class="sxs-lookup"><span data-stu-id="b9d6b-115">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="b9d6b-116">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="b9d6b-116">Return value</span></span>

<span data-ttu-id="b9d6b-117">Код ошибки из перечисления [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="b9d6b-117">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
<span data-ttu-id="b9d6b-118">Важно помнить, что эта функция может возвращать **еррсукцесс** , даже если в файлах журналов обнаружены ошибки.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-118">It's important to remember that this function can return **errSuccess** even when errors are found in the log files.</span></span> <span data-ttu-id="b9d6b-119">Таким образом, когда **еррчекклогс** возвращает **еррсукцесс**, приложение также должно проверить возвращаемый параметр **пфонлюннецессарилогскоррупт** .</span><span class="sxs-lookup"><span data-stu-id="b9d6b-119">Therefore, when **ErrCheckLogs** returns **errSuccess**, the application should also check the  **pfOnlyUnnecessaryLogsCorrupt** return parameter.</span></span> <span data-ttu-id="b9d6b-120">Если **пфонлюннецессарилогскорруптс** имеет **значение true** , когда **еррчекклогс** возвращает **еррсукцесс**, это указывает на то, что обнаружена одна или несколько ошибок, а не только те файлы журнала, которые не требуются для обновления базы данных.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-120">If **pfOnlyUnnecessaryLogsCorrupts** is **true** when **ErrCheckLogs** returns **errSuccess**, this indicates that one or more errors were found, but only in log files not needed to bring the database up-to-date.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b9d6b-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="b9d6b-121">Remarks</span></span>

<span data-ttu-id="b9d6b-122">Перед вызовом функции **еррчекклогс** необходимо вызвать функцию **еррчеккдбхеадерс** .</span><span class="sxs-lookup"><span data-stu-id="b9d6b-122">The **ErrCheckDbHeaders** function must be called before the **ErrCheckLogs** function can be called.</span></span> 
  
<span data-ttu-id="b9d6b-123">Когда проверяются файлы журналов транзакций базы данных Exchange, некоторые файлы журналов необходимы для переноса баз данных из группы хранения в состояние чистого отключения без потери данных, в то время как другие файлы журналов могут быть не нужны.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-123">When Exchange database transaction log files are being checked, some of the log files will be necessary to bring the databases in the storage group to a clean-shutdown state without data loss, whereas other log files might not be needed.</span></span> <span data-ttu-id="b9d6b-124">Функция **еррчекклогс** определяет как старейшие, так и самые новые файлы журналов, необходимые для обновления баз данных.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-124">The **ErrCheckLogs** function determines both the oldest and the newest log files that are needed to bring the databases up to date.</span></span> 
  
<span data-ttu-id="b9d6b-125">Функция **еррчекклогс** проверяет все файлы журналов по указанным путям, у которых также указано имя базового файла из трех букв, переданное в функцию **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="b9d6b-125">The **ErrCheckLogs** function verifies all the log files in the specified paths that also have the specified three-letter base file name, as passed to the **ErrInit** function.</span></span> 
  
<span data-ttu-id="b9d6b-126">Если в файлах журнала ошибок не обнаружено, **еррчекклогс** возвращает **еррсукцесс**.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-126">If no errors are found in the log files, **ErrCheckLogs** returns **errSuccess**.</span></span> 
  
<span data-ttu-id="b9d6b-127">Если один из необходимых файлов журнала поврежден, **еррчекклогс** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-127">If any of the required log files are found to be corrupted, **ErrCheckLogs** returns an error.</span></span> 
  
<span data-ttu-id="b9d6b-128">Если ошибки обнаружены только в файлах журнала, которые старше самых ранних требуемых, функция возвращает **еррсукцесс** и задает для параметра return **пфонлюннецессарилогкоррупт** **значение true**.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-128">If errors are found only in log files that are older than the earliest ones needed, the function returns **errSuccess** and sets the return parameter **pfOnlyUnnecessaryLogCorrupt** to **true**.</span></span> <span data-ttu-id="b9d6b-129">Приложение должно распознать наличие ошибок в некоторых старых файлах журнала и, если это так, может предупредить пользователя.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-129">The application should recognize that there are errors in some of those old log files, and if so, it will possibly alert the user.</span></span> <span data-ttu-id="b9d6b-130">В любом случае эти ошибки не повлияют на общую целостность базы данных или на то, могут ли успешно воспроизводиться журналы.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-130">In any case, those errors should not affect the overall integrity of the database or affect whether playing the logs forward will succeed.</span></span>
  
<span data-ttu-id="b9d6b-131">Если ошибки найдены в любом файле журнала, созданном после того, как будет определен самый ранний журнал, который **еррчекклогс** определяет, функция возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-131">If errors are found in any log file created after the earliest log that **ErrCheckLogs** determines is needed, the function returns an error.</span></span> <span data-ttu-id="b9d6b-132">Сообщение об ошибке возвращается даже в том случае, если в файле журнала, созданном позже, было обнаружено сообщение об ошибке файла журнала, которое было создано позже, чем требуется для обновления базы данных.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-132">The error will be returned even if the log file error was found in a log file that was generated later than what is needed to bring the database up to date.</span></span> <span data-ttu-id="b9d6b-133">Несмотря на то, что вы сможете перевести базы данных в состояние чистого отключения с помощью указанных файлов журнала, не будут применены транзакции, указанные в последующих поврежденных файлах журнала, что приведет к потере данных при восстановлении базы данных.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-133">Although it would be possible to bring the databases to a clean-shutdown state by using the identified log files, transactions specified in the later corrupted log files would not be applied, resulting in data loss when the database is restored.</span></span> 
  
<span data-ttu-id="b9d6b-134">Объект **функция cchksgfiles** определяет, действительно ли проверены все файлы журналов, зарегистрированные с помощью функции **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="b9d6b-134">The **CChkSGFiles** object determines whether all of the log files registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="b9d6b-135">Если не все журналы не были успешно проверены, функция **ерртерм** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-135">If not all of the logs were not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="b9d6b-136">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, вы можете вызвать функцию **еррчекклогс** в многопоточной части приложения, но вы можете вызвать ее только один раз для каждого объекта **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="b9d6b-136">If you're using CHKSGFILES in a multithreaded application, you can call the **ErrCheckLogs** function in the multithreaded portion of the application, but you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="b9d6b-137">Requirements</span><span class="sxs-lookup"><span data-stu-id="b9d6b-137">Requirements</span></span>

<span data-ttu-id="b9d6b-138">Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-138">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="b9d6b-139">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="b9d6b-139">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

