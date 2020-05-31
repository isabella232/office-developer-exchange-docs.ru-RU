---
title: Функция функция cchksgfiles. Кмаксдбперсг
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: bf09074bab6dee13e97e8a59a22ae1b19522a5e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761882"
---
# <a name="cchksgfilescmaxdbpersg-function"></a><span data-ttu-id="ff80e-103">Функция функция cchksgfiles. Кмаксдбперсг</span><span class="sxs-lookup"><span data-stu-id="ff80e-103">CChkSGFiles.CMaxDbPerSG function</span></span>

<span data-ttu-id="ff80e-104">**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="ff80e-104">**Applies to:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013</span></span>
  
<span data-ttu-id="ff80e-105">Возвращает максимально допустимое число баз данных в одной группе хранения Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="ff80e-105">Returns the maximum number of databases allowed in a single Exchange server storage group.</span></span>
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a><span data-ttu-id="ff80e-106">Параметры</span><span class="sxs-lookup"><span data-stu-id="ff80e-106">Parameters</span></span>

<span data-ttu-id="ff80e-107">Нет.</span><span class="sxs-lookup"><span data-stu-id="ff80e-107">None.</span></span>
  
## <a name="return-value"></a><span data-ttu-id="ff80e-108">Возвращаемое значение</span><span class="sxs-lookup"><span data-stu-id="ff80e-108">Return value</span></span>

<span data-ttu-id="ff80e-109">Максимальное число баз данных, разрешенных указанным сервером Exchange для каждой группы хранения.</span><span class="sxs-lookup"><span data-stu-id="ff80e-109">The maximum number of databases that the specified Exchange server allows per storage group.</span></span> <span data-ttu-id="ff80e-110">Так как группы хранения не входят в состав Exchange 2013, эта функция возвращает 1.</span><span class="sxs-lookup"><span data-stu-id="ff80e-110">Because storage groups are not part of Exchange 2013, this function returns 1.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ff80e-111">Примечания</span><span class="sxs-lookup"><span data-stu-id="ff80e-111">Remarks</span></span>

<span data-ttu-id="ff80e-112">Объект **кчекксгфилес** можно использовать для проверки баз данных (и файлов журнала транзакций) только в одной группе хранения, поэтому значение, возвращаемое функцией **кмаксдбперсг** , также представляет максимальное число баз данных, которые можно проверить с помощью экземпляра класса **кчекксгфилес** .</span><span class="sxs-lookup"><span data-stu-id="ff80e-112">You can use the **CCheckSGFiles** object to validate databases (and transaction log files) in only one storage group, so the value returned by the **CMaxDbPerSG** function also represents the maximum number of databases that you can check by using an instance of the **CCheckSGFiles** class.</span></span> 
  
<span data-ttu-id="ff80e-113">Обратите внимание, что по умолчанию Exchange Server 2003 и Exchange Server 2007 допускают не более пяти баз данных на каждую группу хранения.</span><span class="sxs-lookup"><span data-stu-id="ff80e-113">Note that by default, Exchange Server 2003 and Exchange Server 2007 allow a maximum of five databases per storage group.</span></span>
  
## <a name="requirements"></a><span data-ttu-id="ff80e-114">Requirements</span><span class="sxs-lookup"><span data-stu-id="ff80e-114">Requirements</span></span>

<span data-ttu-id="ff80e-115">Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="ff80e-115">Exchange 2013 only includes a 64-bit version of the CHKSGFILES API.</span></span>
  
<span data-ttu-id="ff80e-116">Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.</span><span class="sxs-lookup"><span data-stu-id="ff80e-116">The account that the application is running under must have read access permissions to the database and log files that are to be checked.</span></span>
  

