---
title: Функция CChkSGFiles.ErrTerm
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
description: 'Последнее изменение: 25 февраля 2013 г.'
ms.openlocfilehash: 099ec33663baa2414a0c28b90364523b6191c697
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760924"
---
# <a name="cchksgfileserrterm-function"></a><span data-ttu-id="add39-103">Функция CChkSGFiles.ErrTerm</span><span class="sxs-lookup"><span data-stu-id="add39-103">CChkSGFiles.ErrTerm function</span></span>
  
<span data-ttu-id="add39-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="add39-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="add39-105">Содержит общее состояние проверки базы данных и журналов, который указывает, будет ли страниц базы данных и журналов были успешно проверено.</span><span class="sxs-lookup"><span data-stu-id="add39-105">Provides an overall status of the database and log verification, which indicates whether all the database pages and logs were successfully verified.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="add39-106">Группы хранения, недоступны в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="add39-106">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="add39-107">Для обеспечения обратной совместимости с базами данных и группы хранения в версии Exchange, предшествующие Exchange Server 2010 CHKSGFILES API позволяет указать группы хранения.</span><span class="sxs-lookup"><span data-stu-id="add39-107">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange Server 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="add39-108">При выполнении CHKSGFILES баз данных Exchange 2013, необходимо настроить параметры, укажите идентификатор группы хранения пустую строку.</span><span class="sxs-lookup"><span data-stu-id="add39-108">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
```cs
Vitual ERRErrTerm 
(
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a><span data-ttu-id="add39-109">Parameters</span><span class="sxs-lookup"><span data-stu-id="add39-109">Parameters</span></span>

### <a name="ulflags"></a><span data-ttu-id="add39-110">ulFlags</span><span class="sxs-lookup"><span data-stu-id="add39-110">ulFlags</span></span>
  
<span data-ttu-id="add39-111">Необязательный параметр ввода.</span><span class="sxs-lookup"><span data-stu-id="add39-111">Optional input parameter.</span></span> <span data-ttu-id="add39-112">Это значение зарезервировано для будущего использования.</span><span class="sxs-lookup"><span data-stu-id="add39-112">This value is reserved for future use.</span></span> <span data-ttu-id="add39-113">Значение, переданное в этом параметре должны быть нуль (0).</span><span class="sxs-lookup"><span data-stu-id="add39-113">The value passed by this parameter should be 0 (zero).</span></span>
    
## <a name="return-value"></a><span data-ttu-id="add39-114">������������ ��������</span><span class="sxs-lookup"><span data-stu-id="add39-114">Return value</span></span>

<span data-ttu-id="add39-115">Код ошибки из перечисления [ERR](cchksgfiles-err-enumeration.md) .</span><span class="sxs-lookup"><span data-stu-id="add39-115">An error code from the [ERR](cchksgfiles-err-enumeration.md) enumeration.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="add39-116">Замечания</span><span class="sxs-lookup"><span data-stu-id="add39-116">Remarks</span></span>

<span data-ttu-id="add39-117">Объект **CChkSGFiles** определяет проверены ли все базы данных, зарегистрированные с помощью функции **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="add39-117">The **CChkSGFiles** object determines whether all the databases registered with the **ErrInit** function were actually checked.</span></span> <span data-ttu-id="add39-118">Этот объект используется функция **ErrCheckDbPages** чтобы убедиться, что такое же число базы данных, которые фактически было проверено страниц, обнаруженных с помощью функции **ErrCheckDbHeaders** .</span><span class="sxs-lookup"><span data-stu-id="add39-118">This object uses the **ErrCheckDbPages** function to verify that the same number of database pages identified by the **ErrCheckDbHeaders** function were actually verified.</span></span> <span data-ttu-id="add39-119">Если не будут возвращены правильное число страниц в каждой базе данных, функция **ErrTerm** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="add39-119">If the correct number of pages in each database are not successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="add39-120">Если число страниц базы данных, проверяются с **ErrCheckDbPages** меньше значения, указанный в параметре **ErrCheckDbHeaders**, эта функция создает ошибку в журнал событий Windows и **ErrTerm** возвращает сообщение об ошибке.</span><span class="sxs-lookup"><span data-stu-id="add39-120">If the number of database pages checked with **ErrCheckDbPages** is less than that indicated by **ErrCheckDbHeaders**, this function creates an error in the Windows Event log, and **ErrTerm** returns an error.</span></span> 
  
<span data-ttu-id="add39-121">Если число страниц базы данных, проверяются с **ErrCheckDbPages** больше, указанный в параметре **ErrCheckDbHeaders**, эта функция создает предупреждение в журнал событий Windows, чтобы указать, что приложение может быть без необходимости проверки некоторые несколько раз страниц базы данных.</span><span class="sxs-lookup"><span data-stu-id="add39-121">If the number of database pages checked with **ErrCheckDbPages** is greater than that indicated by **ErrCheckDbHeaders**, this function creates a warning in the Windows Event log to indicate that the application might be unnecessarily checking some database pages more than once.</span></span> <span data-ttu-id="add39-122">В данном случае тем не менее, функция **ErrTerm** успешно.</span><span class="sxs-lookup"><span data-stu-id="add39-122">In this case, however, the **ErrTerm** function succeeds.</span></span> 
  
<span data-ttu-id="add39-123">Объект **CChkSGFiles** также определяет проверены ли файлы журнала, зарегистрированных в **ErrInit** .</span><span class="sxs-lookup"><span data-stu-id="add39-123">The **CChkSGFiles** object also determines whether the log files registered with **ErrInit** were actually checked.</span></span> <span data-ttu-id="add39-124">Если не все журналы успешно установлен, функция **ErrTerm** возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="add39-124">If not all the logs were successfully checked, the **ErrTerm** function returns an error.</span></span> 
  
<span data-ttu-id="add39-125">Если **ErrTerm** возвращает ошибку, оно будет первую ошибку, найденную, несмотря на то, что проверяет состояние проверки для всех баз данных, зарегистрированных в **ErrInit**.</span><span class="sxs-lookup"><span data-stu-id="add39-125">When **ErrTerm** returns an error, it will be the first error it finds, even though it checks the verification status for all databases registered with **ErrInit**.</span></span>
  
<span data-ttu-id="add39-126">Если вы используете многопоточного приложения CHKSGFILES, необходимо вызвать функцию **ErrTerm** в одном потоке часть приложения и его можно вызвать не более чем один раз для каждого объекта **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="add39-126">If you're using CHKSGFILES in a multithreaded application, you must call the **ErrTerm** function in the single-threaded portion of the application, and you can call it no more than once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="add39-127">Требования</span><span class="sxs-lookup"><span data-stu-id="add39-127">Requirements</span></span>

<span data-ttu-id="add39-128">Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="add39-128">Exchange 2013 only includes a 64-bit version of CHKSGFILES.</span></span>
  
<span data-ttu-id="add39-129">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="add39-129">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

