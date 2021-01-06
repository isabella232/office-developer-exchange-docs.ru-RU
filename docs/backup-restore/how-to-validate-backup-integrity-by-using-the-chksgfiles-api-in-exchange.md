---
title: Проверка целостности резервного копирования с помощью API CHKSGFILES в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Узнайте, как использовать API CHKSGFILES для проверки резервной копии магазина Exchange в Exchange 2013.
ms.openlocfilehash: c101413793cf3b952d3db3e0f792c8bcf2dd9fc9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452862"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a><span data-ttu-id="b3630-103">Проверка целостности резервного копирования с помощью API CHKSGFILES в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b3630-103">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>

<span data-ttu-id="b3630-104">Узнайте, как использовать API CHKSGFILES для проверки резервной копии магазина Exchange в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="b3630-104">Find out how to use the CHKSGFILES API to validate a backup of the Exchange store in Exchange 2013.</span></span>
  
<span data-ttu-id="b3630-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="b3630-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="b3630-106">Во время операций резервного копирования, управляемых службой теневого копирования томов (VSS), Exchange Server 2013 не может полностью прочитать каждый файл базы данных и проверить его целостность контрольных контрольных объемов.</span><span class="sxs-lookup"><span data-stu-id="b3630-106">During backup operations managed by the Volume Shadow Copy Service (VSS), Exchange Server 2013 cannot read each database file in its entirety and verify its checksum integrity.</span></span> <span data-ttu-id="b3630-107">Поэтому может потребоваться, чтобы приложение резервного копирования проверило целостность файлов базы данных и журнала транзакций.</span><span class="sxs-lookup"><span data-stu-id="b3630-107">Therefore, you might want your backup application to verify database and transaction log file integrity.</span></span> <span data-ttu-id="b3630-108">Перед тем как сообщить записи Exchange о том, что резервное копирование завершено, приложению резервного копирования рекомендуется проверить физическую согласованность набора теневых копий.</span><span class="sxs-lookup"><span data-stu-id="b3630-108">We recommend that your backup application verify the physical consistency of the shadow copy set prior to informing the Exchange writer that the backup is complete.</span></span> <span data-ttu-id="b3630-109">После успешного резервного копирования хранилище Exchange обновляет заглавные данные резервных копий баз данных с учетом времени последнего успешного резервного копирования и удаляет журналы транзакций с сервера, которые больше не требуются для отката из последней успешной резервной копии.</span><span class="sxs-lookup"><span data-stu-id="b3630-109">After a successful backup, the Exchange store updates the headers of the backed-up databases to reflect the last successful backup times and removes transaction logs from the server that are no longer required to roll forward from the last successful backup.</span></span>
  
## <a name="prerequisites-for-validating-backup-integrity"></a><span data-ttu-id="b3630-110">Необходимые условия для проверки целостности резервного копирования</span><span class="sxs-lookup"><span data-stu-id="b3630-110">Prerequisites for validating backup integrity</span></span>

<span data-ttu-id="b3630-111">Прежде чем приложение сможет проверить целостность резервной копии, необходимо иметь доступ к следующим данным:</span><span class="sxs-lookup"><span data-stu-id="b3630-111">Before your application can validate the integrity of your backup, you must have access to the following:</span></span>
  
- <span data-ttu-id="b3630-112">Файлы из резервной копии магазина Exchange.</span><span class="sxs-lookup"><span data-stu-id="b3630-112">Files from your Exchange store backup.</span></span>
- <span data-ttu-id="b3630-113">Версия Visual Studio начиная с Visual Studio 2010.</span><span class="sxs-lookup"><span data-stu-id="b3630-113">A version of Visual Studio starting with Visual Studio 2010.</span></span>
- <span data-ttu-id="b3630-114">Файлы библиотеки и заголовок CHKSGFILES.</span><span class="sxs-lookup"><span data-stu-id="b3630-114">The CHKSGFILES library and header files.</span></span> <span data-ttu-id="b3630-115">Вы можете скачать библиотеку и файлы заголовок из [Центра загрузки Майкрософт.](https://www.microsoft.com/download/details.aspx?id=36802)</span><span class="sxs-lookup"><span data-stu-id="b3630-115">You can download the library and header files from the [Microsoft Download Center](https://www.microsoft.com/download/details.aspx?id=36802).</span></span>
    
## <a name="validate-backup-integrity"></a><span data-ttu-id="b3630-116">Проверка целостности резервного копирования</span><span class="sxs-lookup"><span data-stu-id="b3630-116">Validate backup integrity</span></span>

<span data-ttu-id="b3630-117">В следующей процедуре описывается проверка целостности данных в приложении резервного копирования и восстановления.</span><span class="sxs-lookup"><span data-stu-id="b3630-117">The following procedure describes how to validate data integrity in your backup and restore application.</span></span>
  
### <a name="to-validate-backup-integrity"></a><span data-ttu-id="b3630-118">Проверка целостности резервного копирования</span><span class="sxs-lookup"><span data-stu-id="b3630-118">To validate backup integrity</span></span>

1. <span data-ttu-id="b3630-119">Создайте новый экземпляр класса **CChkSGFiles.**</span><span class="sxs-lookup"><span data-stu-id="b3630-119">Create a new instance of the **CChkSGFiles** class.</span></span> 
   
   ```cpp
   CCheckSGFiles::ERRerr = CCheckSGFiles::errSuccess;
   ULONGiDbError = (ULONG)CCheckSGFiles::iDbInvalid;
   CCheckSGFiles * const pcchecksgfiles = CCheckSGFiles::New();
   if ( NULL == pcchecksgfiles )
   {
     err = CCheckSGFiles::errOutOfMemory;
     printf( "ERROR: Could not allocate CCheckSGFiles object.\n" );
     goto HandleError;
   }
   ```

   <span data-ttu-id="b3630-120">Первые строки кода создают объект ошибки и устанавливают его начальное значение успешно, а также создают объект, который проверяет правильность базы данных.</span><span class="sxs-lookup"><span data-stu-id="b3630-120">The first lines of code create an error object and set its initial value to success, and create an object that checks the validity of the database.</span></span> <span data-ttu-id="b3630-121">Затем функция [CChkSGFiles.New](cchksgfiles-new-function.md) создает новый экземпляр класса **CChkSGFiles.**</span><span class="sxs-lookup"><span data-stu-id="b3630-121">Then, the [CChkSGFiles.New function](cchksgfiles-new-function.md) creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="b3630-122">Быстрая проверка нового объекта указывает, произошли ли проблемы при его создания.</span><span class="sxs-lookup"><span data-stu-id="b3630-122">A quick check of the new object indicates whether any issues occurred when the new instance was created.</span></span> 
    
2. <span data-ttu-id="b3630-123">Инициализация **объекта CChkSGFiles.**</span><span class="sxs-lookup"><span data-stu-id="b3630-123">Initialize the **CChkSGFiles** object.</span></span> 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   <span data-ttu-id="b3630-124">Дополнительные сведения о параметрах см. в функции [CChkSGFiles.ErrInit.](cchksgfiles-errinit-function.md)</span><span class="sxs-lookup"><span data-stu-id="b3630-124">For more information about the parameters, see [CChkSGFiles.ErrInit function](cchksgfiles-errinit-function.md).</span></span>
   
3. <span data-ttu-id="b3630-125">Используйте [функцию CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) для проверки целостности базы данных, проверяя их заголовок.</span><span class="sxs-lookup"><span data-stu-id="b3630-125">Use the [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md) to validate database integrity by checking the database headers.</span></span>
   
   ```cpp
   err = pcchecksgfiles->ErrCheckDbHeaders(
   &amp;cbDbPageSize,
   &amp;cDbHeaderPages,
   &amp;iDbError );
   if ( CCheckSGFiles::errSuccess != err )
   {
   if ( CCheckSGFiles::iDbInvalid != iDbError )
   {
   printf(
   "ERROR: Database header validation for '%S' failed with error %d (0x%x)\n",
   rgwszDb[ iDbError ],
   err,
   err );
   }
   goto HandleError;
   }
   ```
   
   <span data-ttu-id="b3630-126">Дополнительные сведения о параметрах см. в функции [CChkSGFiles.ErrCheckDbHeaders.](cchksgfiles-errcheckdbheaders-function.md)</span><span class="sxs-lookup"><span data-stu-id="b3630-126">For more information about the parameters, see [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md).</span></span>
   
4. <span data-ttu-id="b3630-127">Обработать ошибки и использовать функцию [CChkSGFiles.Delete,](cchksgfiles-delete-function.md) чтобы удалить класс **CChkSGFiles** из памяти.</span><span class="sxs-lookup"><span data-stu-id="b3630-127">Handle errors, and use the [CChkSGFiles.Delete function](cchksgfiles-delete-function.md) to remove the **CChkSGFiles** class from memory.</span></span> 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a><span data-ttu-id="b3630-128">См. также</span><span class="sxs-lookup"><span data-stu-id="b3630-128">See also</span></span>

- [<span data-ttu-id="b3630-129">Справочник по классу CChkSGFiles</span><span class="sxs-lookup"><span data-stu-id="b3630-129">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="b3630-130">Создание приложений резервного копирования и восстановления для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b3630-130">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="b3630-131">Концепции резервного копирования и восстановления для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="b3630-131">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

