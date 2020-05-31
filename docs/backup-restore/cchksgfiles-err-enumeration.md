---
title: Перечисление функция cchksgfiles. ERR
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: 'Дата последнего изменения: 9 марта 2015 г.'
ms.openlocfilehash: 20f10c43e3b92604bb51e1aa5f896a8bd7c4b335
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761865"
---
# <a name="cchksgfileserr-enumeration"></a><span data-ttu-id="33fbc-103">Перечисление функция cchksgfiles. ERR</span><span class="sxs-lookup"><span data-stu-id="33fbc-103">CChkSGFiles.ERR enumeration</span></span> 
  
<span data-ttu-id="33fbc-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="33fbc-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="33fbc-105">Показывает результаты вызываемой функции.</span><span class="sxs-lookup"><span data-stu-id="33fbc-105">Indicates the results of the called function.</span></span> <span data-ttu-id="33fbc-106">Это перечисление возвращается многими функциями класса **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="33fbc-106">This enumeration is returned by many functions of the **CCheckSGFiles** class.</span></span> 
  
```cs
Enum ERR  
{
        errSuccess = 0,
        errTaskDropped = -106,
        errRequiredLogFilesMissing = -543,
        errInvalidParameter = -1003,
        errOutOfMemory = -1011,
        errReadVerifyFailure = -1018,
        errTooManyActiveUsers = -1059,
        errDatabaseCorrupted = -1206
}

```

## <a name="values"></a><span data-ttu-id="33fbc-107">Values</span><span class="sxs-lookup"><span data-stu-id="33fbc-107">Values</span></span>

|<span data-ttu-id="33fbc-108">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="33fbc-108">**Member name**</span></span>|<span data-ttu-id="33fbc-109">**Значение**</span><span class="sxs-lookup"><span data-stu-id="33fbc-109">**Value**</span></span>|<span data-ttu-id="33fbc-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33fbc-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="33fbc-111">еррсукцесс</span><span class="sxs-lookup"><span data-stu-id="33fbc-111">errSuccess</span></span>  <br/> |<span data-ttu-id="33fbc-112">нуль</span><span class="sxs-lookup"><span data-stu-id="33fbc-112">0</span></span>  <br/> |<span data-ttu-id="33fbc-113">Функция завершена без ошибок.</span><span class="sxs-lookup"><span data-stu-id="33fbc-113">The function completed without any errors.</span></span>  <br/> |
|<span data-ttu-id="33fbc-114">ерртаскдроппед</span><span class="sxs-lookup"><span data-stu-id="33fbc-114">errTaskDropped</span></span>  <br/> |<span data-ttu-id="33fbc-115">— 106</span><span class="sxs-lookup"><span data-stu-id="33fbc-115">-106</span></span>  <br/> |<span data-ttu-id="33fbc-116">Возвращается функцией **ерртерм** , чтобы указать, что были проверены не все страницы базы данных и файлы журнала транзакций, а также обнаружены ошибки во время проверки.</span><span class="sxs-lookup"><span data-stu-id="33fbc-116">Returned by the **ErrTerm** function to indicate that not all database pages and transaction log files were checked, or that errors were encountered during the verification.</span></span>  <br/> |
|<span data-ttu-id="33fbc-117">ерррекуиредлогфилесмиссинг</span><span class="sxs-lookup"><span data-stu-id="33fbc-117">errRequiredLogFilesMissing</span></span>  <br/> |<span data-ttu-id="33fbc-118">— 543</span><span class="sxs-lookup"><span data-stu-id="33fbc-118">-543</span></span>  <br/> |<span data-ttu-id="33fbc-119">Один или несколько файлов журнала, необходимых для переноса базы данных в состояние чистого отключения, не найдены в пути к файлу журнала или не имеют указанного имени из трех букв.</span><span class="sxs-lookup"><span data-stu-id="33fbc-119">One or more log files that are required to bring the database to a clean-shutdown state was not found in the log file path, or did not have the specified three-letter base name.</span></span>  <br/> |
|<span data-ttu-id="33fbc-120">ерринвалидпараметер</span><span class="sxs-lookup"><span data-stu-id="33fbc-120">errInvalidParameter</span></span>  <br/> |<span data-ttu-id="33fbc-121">— 1003</span><span class="sxs-lookup"><span data-stu-id="33fbc-121">-1003</span></span>  <br/> |<span data-ttu-id="33fbc-122">Один или несколько параметров, переданных функции, являются недопустимыми.</span><span class="sxs-lookup"><span data-stu-id="33fbc-122">One or more parameters that were passed to the function were invalid.</span></span>  <br/> |
|<span data-ttu-id="33fbc-123">ерраутофмемори</span><span class="sxs-lookup"><span data-stu-id="33fbc-123">errOutOfMemory</span></span>  <br/> |<span data-ttu-id="33fbc-124">— 1011</span><span class="sxs-lookup"><span data-stu-id="33fbc-124">-1011</span></span>  <br/> |<span data-ttu-id="33fbc-125">Недостаточно памяти для выполнения запрошенной операции.</span><span class="sxs-lookup"><span data-stu-id="33fbc-125">Insufficient memory was available to complete the requested operation.</span></span>  <br/> |
|<span data-ttu-id="33fbc-126">еррреадверифифаилуре</span><span class="sxs-lookup"><span data-stu-id="33fbc-126">errReadVerifyFailure</span></span>  <br/> |<span data-ttu-id="33fbc-127">— 1018</span><span class="sxs-lookup"><span data-stu-id="33fbc-127">-1018</span></span>  <br/> |<span data-ttu-id="33fbc-128">Контрольная сумма, хранящаяся на странице базы данных, не соответствует ожидаемой контрольной сумме.</span><span class="sxs-lookup"><span data-stu-id="33fbc-128">The checksum that is stored on a database page does not match its expected checksum.</span></span>  <br/> |
|<span data-ttu-id="33fbc-129">ерртуманяктивеусерс</span><span class="sxs-lookup"><span data-stu-id="33fbc-129">errTooManyActiveUsers</span></span>  <br/> |<span data-ttu-id="33fbc-130">— 1059</span><span class="sxs-lookup"><span data-stu-id="33fbc-130">-1059</span></span>  <br/> |<span data-ttu-id="33fbc-131">Функция **ерртерм** вызвана во время использования объекта.</span><span class="sxs-lookup"><span data-stu-id="33fbc-131">The **ErrTerm** function was called while the object was still being used.</span></span> <span data-ttu-id="33fbc-132">Это может произойти, если **ерртерм** вызывается до возвращения **еррчеккдбпажес** или **еррчекклогфилес** .</span><span class="sxs-lookup"><span data-stu-id="33fbc-132">This can occur if **ErrTerm** is called before **ErrCheckDbPages** or **ErrCheckLogFiles** has returned.</span></span>  <br/> |
   
## <a name="requirements"></a><span data-ttu-id="33fbc-133">Requirements</span><span class="sxs-lookup"><span data-stu-id="33fbc-133">Requirements</span></span>

<span data-ttu-id="33fbc-134">Exchange Server 2013 включает в себя только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="33fbc-134">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="33fbc-135">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="33fbc-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

