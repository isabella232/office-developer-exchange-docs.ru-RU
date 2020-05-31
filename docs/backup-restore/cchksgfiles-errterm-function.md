---
title: Функция функция cchksgfiles. Ерртерм
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrTerm
api_type:
- dllExport
ms.assetid: eea20a55-4a2a-4209-ae79-dc1ee1cd631b
description: 'Дата последнего изменения: 25 февраля 2013 г.'
ms.openlocfilehash: 099ec33663baa2414a0c28b90364523b6191c697
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760924"
---
# <a name="cchksgfileserrterm-function"></a><span data-ttu-id="59441-103">Функция функция cchksgfiles. Ерртерм</span><span class="sxs-lookup"><span data-stu-id="59441-103">CChkSGFiles.ErrTerm function</span></span>
  
<span data-ttu-id="59441-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="59441-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="59441-105">Предоставляет общий статус проверки базы данных и журнала, которая указывает, успешно ли проверены все страницы базы данных и журналы.</span><span class="sxs-lookup"><span data-stu-id="59441-105">Provides an overall status of the database and log verification, which indicates whether all the database pages and logs were successfully verified.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="59441-106">Группы хранения недоступны в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="59441-106">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="59441-107">Для обеспечения обратной совместимости с базами данных и группами хранения в более ранних версиях Exchange, чем Exchange Server 2010, API ЧКСГФИЛЕС позволяет указать группы хранения.</span><span class="sxs-lookup"><span data-stu-id="59441-107">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange Server 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="59441-108">При запуске ЧКСГФИЛЕС для баз данных Exchange 2013 необходимо задать параметры, указывающие идентификатор группы хранения, в пустую строку.</span><span class="sxs-lookup"><span data-stu-id="59441-108">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="59441-109">Параметры</span><span class="sxs-lookup"><span data-stu-id="59441-109">Parameters</span></span>

### <a name="ulflags"></a><span data-ttu-id="59441-110">ulFlags</span><span class="sxs-lookup"><span data-stu-id="59441-110">ulFlags</span></span>
  
<span data-ttu-id="59441-111">Необязательный входной параметр.</span><span class="sxs-lookup"><span data-stu-id="59441-111">Optional input parameter.</span></span> <span data-ttu-id="59441-112">Это значение зарезервировано для использования в будущем.</span><span class="sxs-lookup"><span data-stu-id="59441-112">This value is reserved for future use.</span></span> <span data-ttu-id="59441-113">Значение, передаваемое этим параметром, должно быть равно 0 (нулю).</span><span class="sxs-lookup"><span data-stu-id="59441-113">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="59441-114">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="59441-114">Return value</span></span>

<span data-ttu-id="59441-115">Код ошибки из перечисления [Err](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="59441-115">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="59441-116">Примечания</span><span class="sxs-lookup"><span data-stu-id="59441-116">Remarks</span></span>

<span data-ttu-id="59441-117">Объект **функция cchksgfiles** определяет, действительно ли проверены все базы данных, зарегистрированные с помощью функции **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="59441-117">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="59441-118">Этот объект использует функцию **еррчеккдбпажес** для проверки того, что количество страниц базы данных, идентифицируемых функцией **еррчеккдбхеадерс** , фактически проверено.</span><span class="sxs-lookup"><span data-stu-id="59441-118">This object uses the **ErrCheckDbPages** function to verify that the same number of database pages identified by the **ErrCheckDbHeaders** function were actually verified.</span></span> <span data-ttu-id="59441-119">Если правильное количество страниц в каждой базе данных не прошло проверку, функция **ерртерм** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="59441-119">If the correct number of pages in each database are not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="59441-120">Если количество страниц базы данных, проверенных с помощью **еррчеккдбпажес** , меньше, чем указано в **еррчеккдбхеадерс**, эта функция создает ошибку в журнале событий Windows, а **ерртерм** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="59441-120">If the number of database pages checked with **ErrCheckDbPages** is less than that indicated by **ErrCheckDbHeaders**, this function creates an error in the Windows Event log, and **ErrTerm** returns an error.</span></span> 
  
<span data-ttu-id="59441-121">Если количество страниц базы данных, проверенных с помощью **еррчеккдбпажес** , больше, чем указано в **еррчеккдбхеадерс**, эта функция создает предупреждение в журнале событий Windows, чтобы указать, что приложение может необязательно проверить некоторые страницы базы данных более одного раза.</span><span class="sxs-lookup"><span data-stu-id="59441-121">If the number of database pages checked with **ErrCheckDbPages** is greater than that indicated by **ErrCheckDbHeaders**, this function creates a warning in the Windows Event log to indicate that the application might be unnecessarily checking some database pages more than once.</span></span> <span data-ttu-id="59441-122">Однако в этом случае функция **ерртерм** успешно выполнена.</span><span class="sxs-lookup"><span data-stu-id="59441-122">In this case, however, the **ErrTerm** function succeeds.</span></span> 
  
<span data-ttu-id="59441-123">Объект **функция cchksgfiles** также определяет, действительно ли проверены файлы журнала, зарегистрированные с помощью **ерринит** .</span><span class="sxs-lookup"><span data-stu-id="59441-123">The **CChkSGFiles** object also determines whether the log files registered with **ErrInit** were actually checked.</span></span> <span data-ttu-id="59441-124">Если не все журналы были успешно проверены, функция **ерртерм** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="59441-124">If not all the logs were successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="59441-125">Когда **ерртерм** возвращает ошибку, она будет первой найденной ошибкой, несмотря на то, что она проверяет состояние проверки для всех баз данных, зарегистрированных с помощью **ерринит**.</span><span class="sxs-lookup"><span data-stu-id="59441-125">When **ErrTerm** returns an error, it will be the first error it finds, even though it checks the verification status for all databases registered with **ErrInit**.</span></span>
  
<span data-ttu-id="59441-126">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, необходимо вызвать функцию **ерртерм** в однопотоковой части приложения, и вы можете вызвать его не более одного раза для каждого объекта **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="59441-126">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrTerm** function in the single-threaded portion of the application, and you can call it no more than once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="59441-127">Requirements</span><span class="sxs-lookup"><span data-stu-id="59441-127">Requirements</span></span>

<span data-ttu-id="59441-128">Exchange 2013 включает только 64 — разрядную версию ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="59441-128">Exchange 2013 only includes a 64-bit version of CHKSGFILES.</span></span>
  
<span data-ttu-id="59441-129">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="59441-129">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

