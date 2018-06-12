---
title: Перечисление CChkSGFiles.ERR
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
description: '���� ���������� ���������: 9 ����� 2015 �.'
ms.openlocfilehash: 20f10c43e3b92604bb51e1aa5f896a8bd7c4b335
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761865"
---
# <a name="cchksgfileserr-enumeration"></a><span data-ttu-id="b69f2-103">Перечисление CChkSGFiles.ERR</span><span class="sxs-lookup"><span data-stu-id="b69f2-103">CChkSGFiles.ERR enumeration</span></span> 
  
<span data-ttu-id="b69f2-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b69f2-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="b69f2-105">Указывает результаты вызываемой функции.</span><span class="sxs-lookup"><span data-stu-id="b69f2-105">Indicates the results of the called function.</span></span> <span data-ttu-id="b69f2-106">Это перечисление возвращается множество функций класса **CCheckSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="b69f2-106">This enumeration is returned by many functions of the **CCheckSGFiles** class.</span></span> 
  
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

## <a name="values"></a><span data-ttu-id="b69f2-107">Значения</span><span class="sxs-lookup"><span data-stu-id="b69f2-107">Values</span></span>

|<span data-ttu-id="b69f2-108">**Имя элемента**</span><span class="sxs-lookup"><span data-stu-id="b69f2-108">**Member name**</span></span>|<span data-ttu-id="b69f2-109">**Значение**</span><span class="sxs-lookup"><span data-stu-id="b69f2-109">**Value**</span></span>|<span data-ttu-id="b69f2-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b69f2-110">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b69f2-111">errSuccess</span><span class="sxs-lookup"><span data-stu-id="b69f2-111">errSuccess</span></span>  <br/> |<span data-ttu-id="b69f2-112">0</span><span class="sxs-lookup"><span data-stu-id="b69f2-112">0</span></span>  <br/> |<span data-ttu-id="b69f2-113">Функция завершена без ошибок.</span><span class="sxs-lookup"><span data-stu-id="b69f2-113">The function completed without any errors.</span></span>  <br/> |
|<span data-ttu-id="b69f2-114">errTaskDropped</span><span class="sxs-lookup"><span data-stu-id="b69f2-114">errTaskDropped</span></span>  <br/> |<span data-ttu-id="b69f2-115">-106</span><span class="sxs-lookup"><span data-stu-id="b69f2-115">-106</span></span>  <br/> |<span data-ttu-id="b69f2-116">Возвращаемый функцией **ErrTerm** для указания были возвращены, что не все страницы базы данных и файлы журнала транзакций или, что при проверке были обнаружены ошибки.</span><span class="sxs-lookup"><span data-stu-id="b69f2-116">Returned by the **ErrTerm** function to indicate that not all database pages and transaction log files were checked, or that errors were encountered during the verification.</span></span>  <br/> |
|<span data-ttu-id="b69f2-117">errRequiredLogFilesMissing</span><span class="sxs-lookup"><span data-stu-id="b69f2-117">errRequiredLogFilesMissing</span></span>  <br/> |<span data-ttu-id="b69f2-118">-543</span><span class="sxs-lookup"><span data-stu-id="b69f2-118">-543</span></span>  <br/> |<span data-ttu-id="b69f2-119">Один или несколько файлов журнала, которые необходимы для базы данных в состояние чистого отключения не найден в путь к файлу журнала или не имеет указанного базового имени трех букв.</span><span class="sxs-lookup"><span data-stu-id="b69f2-119">One or more log files that are required to bring the database to a clean-shutdown state was not found in the log file path, or did not have the specified three-letter base name.</span></span>  <br/> |
|<span data-ttu-id="b69f2-120">errInvalidParameter</span><span class="sxs-lookup"><span data-stu-id="b69f2-120">errInvalidParameter</span></span>  <br/> |<span data-ttu-id="b69f2-121">-1003</span><span class="sxs-lookup"><span data-stu-id="b69f2-121">-1003</span></span>  <br/> |<span data-ttu-id="b69f2-122">Неправильных один или несколько параметров, которые были переданы в функцию.</span><span class="sxs-lookup"><span data-stu-id="b69f2-122">One or more parameters that were passed to the function were invalid.</span></span>  <br/> |
|<span data-ttu-id="b69f2-123">errOutOfMemory</span><span class="sxs-lookup"><span data-stu-id="b69f2-123">errOutOfMemory</span></span>  <br/> |<span data-ttu-id="b69f2-124">-1011</span><span class="sxs-lookup"><span data-stu-id="b69f2-124">-1011</span></span>  <br/> |<span data-ttu-id="b69f2-125">Недостаточно памяти была доступна для выполнения запрошенной операции.</span><span class="sxs-lookup"><span data-stu-id="b69f2-125">Insufficient memory was available to complete the requested operation.</span></span>  <br/> |
|<span data-ttu-id="b69f2-126">errReadVerifyFailure</span><span class="sxs-lookup"><span data-stu-id="b69f2-126">errReadVerifyFailure</span></span>  <br/> |<span data-ttu-id="b69f2-127">-1018</span><span class="sxs-lookup"><span data-stu-id="b69f2-127">-1018</span></span>  <br/> |<span data-ttu-id="b69f2-128">Контрольная сумма, которая хранится на странице базы данных не соответствует ожидаемой контрольной сумме.</span><span class="sxs-lookup"><span data-stu-id="b69f2-128">The checksum that is stored on a database page does not match its expected checksum.</span></span>  <br/> |
|<span data-ttu-id="b69f2-129">errTooManyActiveUsers</span><span class="sxs-lookup"><span data-stu-id="b69f2-129">errTooManyActiveUsers</span></span>  <br/> |<span data-ttu-id="b69f2-130">-1059</span><span class="sxs-lookup"><span data-stu-id="b69f2-130">-1059</span></span>  <br/> |<span data-ttu-id="b69f2-131">Функция **ErrTerm** вызван при работе с объектом был по-прежнему.</span><span class="sxs-lookup"><span data-stu-id="b69f2-131">The **ErrTerm** function was called while the object was still being used.</span></span> <span data-ttu-id="b69f2-132">Это может произойти, если **ErrTerm** вызывается до **ErrCheckDbPages** или вернул **ErrCheckLogFiles** .</span><span class="sxs-lookup"><span data-stu-id="b69f2-132">This can occur if **ErrTerm** is called before **ErrCheckDbPages** or **ErrCheckLogFiles** has returned.</span></span>  <br/> |
   
## <a name="requirements"></a><span data-ttu-id="b69f2-133">Требования</span><span class="sxs-lookup"><span data-stu-id="b69f2-133">Requirements</span></span>

<span data-ttu-id="b69f2-134">Exchange Server 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.</span><span class="sxs-lookup"><span data-stu-id="b69f2-134">Exchange Server 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="b69f2-135">Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.</span><span class="sxs-lookup"><span data-stu-id="b69f2-135">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

