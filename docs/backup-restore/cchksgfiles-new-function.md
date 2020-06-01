---
title: Функция функция cchksgfiles. New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: d18d3ef20890012a1d8c193ec87bdca10a1ed451
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455235"
---
# <a name="cchksgfilesnew-function"></a><span data-ttu-id="f20be-103">Функция функция cchksgfiles. New</span><span class="sxs-lookup"><span data-stu-id="f20be-103">CChkSGFiles.New function</span></span>

<span data-ttu-id="f20be-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="f20be-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="f20be-105">Создает новый экземпляр класса **функция cchksgfiles** .</span><span class="sxs-lookup"><span data-stu-id="f20be-105">Creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="f20be-106">Эту функцию необходимо вызвать, прежде чем можно будет указать группу хранения и базы данных для проверки.</span><span class="sxs-lookup"><span data-stu-id="f20be-106">You must call this function before you can specify the storage group and databases to be checked.</span></span> 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a><span data-ttu-id="f20be-107">Параметры</span><span class="sxs-lookup"><span data-stu-id="f20be-107">Parameters</span></span>

<span data-ttu-id="f20be-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="f20be-108">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="f20be-109">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="f20be-109">Return value</span></span>

<span data-ttu-id="f20be-110">Ссылка (указатель) на только что созданный объект.</span><span class="sxs-lookup"><span data-stu-id="f20be-110">A reference (pointer) to the newly created object.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f20be-111">Примечания</span><span class="sxs-lookup"><span data-stu-id="f20be-111">Remarks</span></span>

<span data-ttu-id="f20be-112">**Новая** функция создает объект **кчекксгфилес** и возвращает в вызывающий объект ссылку (указатель) на этот объект.</span><span class="sxs-lookup"><span data-stu-id="f20be-112">The **New** function creates a **CCheckSGFiles** object and returns to the caller a reference (pointer) to that object.</span></span> <span data-ttu-id="f20be-113">Эту функцию необходимо вызвать перед вызовом любой из других функций в классе **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="f20be-113">You must call this function before it calls any of the other functions in the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="f20be-114">Если вы используете ЧКСГФИЛЕС в многопоточном приложении, необходимо вызвать функцию **New** в однопотоковой части приложения, и вы можете вызвать его только один раз для каждого объекта **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="f20be-114">If you're using CHKSGFILES in a multithreaded application, you must call the **New** function in the single-threaded portion of the application, and you can call it only once for each **CCheckSGFiles** object.</span></span> 
  
## <a name="requirements"></a><span data-ttu-id="f20be-115">Requirements</span><span class="sxs-lookup"><span data-stu-id="f20be-115">Requirements</span></span>

<span data-ttu-id="f20be-116">Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="f20be-116">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="f20be-117">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="f20be-117">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

