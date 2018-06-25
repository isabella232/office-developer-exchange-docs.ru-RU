---
title: Проверка целостности резервной копии с помощью CHKSGFILES API в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Узнайте, как использовать CHKSGFILES API для проверки резервной копии в хранилище Exchange в Exchange 2013.
ms.openlocfilehash: 968484cd5bb7439730685643683e1d850bec33ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760923"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a><span data-ttu-id="75ea2-103">Проверка целостности резервной копии с помощью CHKSGFILES API в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75ea2-103">Validate backup integrity by using the CHKSGFILES API in Exchange 2013</span></span>

<span data-ttu-id="75ea2-104">Узнайте, как использовать CHKSGFILES API для проверки резервной копии в хранилище Exchange в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="75ea2-104">Find out how to use the CHKSGFILES API to validate a backup of the Exchange store in Exchange 2013.</span></span>
  
<span data-ttu-id="75ea2-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="75ea2-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="75ea2-106">Во время операции резервного копирования, управляемых с службы теневого копирования томов (VSS) Exchange Server 2013 не могут прочитать каждый файл базы данных полностью и проверить его контрольную.</span><span class="sxs-lookup"><span data-stu-id="75ea2-106">During backup operations managed by the Volume Shadow Copy Service (VSS), Exchange Server 2013 cannot read each database file in its entirety and verify its checksum integrity.</span></span> <span data-ttu-id="75ea2-107">Таким образом вы можете резервной копии приложения для проверки целостности файла журнала базы данных и операций.</span><span class="sxs-lookup"><span data-stu-id="75ea2-107">Therefore, you might want your backup application to verify database and transaction log file integrity.</span></span> <span data-ttu-id="75ea2-108">Мы рекомендуем, убедитесь, что приложение резервного копирования физической согласованности set теневой копии до модуля записи Exchange о том, что резервного копирования завершен.</span><span class="sxs-lookup"><span data-stu-id="75ea2-108">We recommend that your backup application verify the physical consistency of the shadow copy set prior to informing the Exchange writer that the backup is complete.</span></span> <span data-ttu-id="75ea2-109">После успешного создания резервной копии в хранилище Exchange обновляет заголовки резервные копии баз данных в соответствии с время последней успешной резервной копии и удаляет журналы транзакций с сервера, которые больше не требуются для отката вперед от последней успешной резервной копии.</span><span class="sxs-lookup"><span data-stu-id="75ea2-109">After a successful backup, the Exchange store updates the headers of the backed-up databases to reflect the last successful backup times and removes transaction logs from the server that are no longer required to roll forward from the last successful backup.</span></span>
  
## <a name="prerequisites-for-validating-backup-integrity"></a><span data-ttu-id="75ea2-110">Необходимые условия для проверки целостности резервной копии</span><span class="sxs-lookup"><span data-stu-id="75ea2-110">Prerequisites for validating backup integrity</span></span>

<span data-ttu-id="75ea2-111">Перед приложения можно проверить целостность резервной копии, необходимо иметь доступ к таким компонентам:</span><span class="sxs-lookup"><span data-stu-id="75ea2-111">Before your application can validate the integrity of your backup, you must have access to the following:</span></span>
  
- <span data-ttu-id="75ea2-112">Файлы из резервной копии хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="75ea2-112">Files from your Exchange store backup.</span></span>
- <span data-ttu-id="75ea2-113">Версия Visual Studio, начиная с помощью Visual Studio 2010.</span><span class="sxs-lookup"><span data-stu-id="75ea2-113">A version of Visual Studio starting with Visual Studio 2010.</span></span>
- <span data-ttu-id="75ea2-114">CHKSGFILES библиотеки и файл заголовка.</span><span class="sxs-lookup"><span data-stu-id="75ea2-114">The CHKSGFILES library and header files.</span></span> <span data-ttu-id="75ea2-115">Библиотеки и заголовок файлы можно загрузить из [Центра загрузки Майкрософт](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="75ea2-115">You can download the library and header files from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
    
## <a name="validate-backup-integrity"></a><span data-ttu-id="75ea2-116">Проверка целостности резервной копии</span><span class="sxs-lookup"><span data-stu-id="75ea2-116">Validate backup integrity</span></span>

<span data-ttu-id="75ea2-117">Ниже описывается, как проверить целостность данных в набор резервного копирования и восстановления приложения.</span><span class="sxs-lookup"><span data-stu-id="75ea2-117">The following procedure describes how to validate data integrity in your backup and restore application.</span></span>
  
### <a name="to-validate-backup-integrity"></a><span data-ttu-id="75ea2-118">Для проверки целостности резервной копии</span><span class="sxs-lookup"><span data-stu-id="75ea2-118">To validate backup integrity</span></span>

1. <span data-ttu-id="75ea2-119">Создайте новый экземпляр класса **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="75ea2-119">Create a new instance of the **CChkSGFiles** class.</span></span> 
   
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

   <span data-ttu-id="75ea2-120">Первой строки кода создайте объект error и задать его начальное значение для успеха и создать объект, который проверяет допустимость базы данных.</span><span class="sxs-lookup"><span data-stu-id="75ea2-120">The first lines of code create an error object and set its initial value to success, and create an object that checks the validity of the database.</span></span> <span data-ttu-id="75ea2-121">Затем с помощью [функции CChkSGFiles.New](cchksgfiles-new-function.md) создает новый экземпляр класса **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="75ea2-121">Then, the [CChkSGFiles.New function](cchksgfiles-new-function.md) creates a new instance of the **CChkSGFiles** class.</span></span> <span data-ttu-id="75ea2-122">Быстрой проверки новый объект указывает, будет ли найденные проблемы произошла при создании нового экземпляра.</span><span class="sxs-lookup"><span data-stu-id="75ea2-122">A quick check of the new object indicates whether any issues occurred when the new instance was created.</span></span> 
    
2. <span data-ttu-id="75ea2-123">Инициализируйте объект **CChkSGFiles** .</span><span class="sxs-lookup"><span data-stu-id="75ea2-123">Initialize the **CChkSGFiles** object.</span></span> 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   <span data-ttu-id="75ea2-124">Дополнительные сведения о параметрах [функции CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md)см.</span><span class="sxs-lookup"><span data-stu-id="75ea2-124">For more information about the parameters, see [CChkSGFiles.ErrInit function](cchksgfiles-errinit-function.md).</span></span>
   
3. <span data-ttu-id="75ea2-125">Используйте [функцию CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) для проверки целостности базы данных, проверив заголовки базы данных.</span><span class="sxs-lookup"><span data-stu-id="75ea2-125">Use the [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md) to validate database integrity by checking the database headers.</span></span>
   
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
   
   <span data-ttu-id="75ea2-126">Дополнительные сведения о параметрах [функции CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)см.</span><span class="sxs-lookup"><span data-stu-id="75ea2-126">For more information about the parameters, see [CChkSGFiles.ErrCheckDbHeaders function](cchksgfiles-errcheckdbheaders-function.md).</span></span>
   
4. <span data-ttu-id="75ea2-127">Обработка ошибок и [функция CChkSGFiles.Delete](cchksgfiles-delete-function.md) используется для удаления класса **CChkSGFiles** из памяти.</span><span class="sxs-lookup"><span data-stu-id="75ea2-127">Handle errors, and use the [CChkSGFiles.Delete function](cchksgfiles-delete-function.md) to remove the **CChkSGFiles** class from memory.</span></span> 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a><span data-ttu-id="75ea2-128">См. также</span><span class="sxs-lookup"><span data-stu-id="75ea2-128">See also</span></span>

- [<span data-ttu-id="75ea2-129">Справочник по CChkSGFiles классов</span><span class="sxs-lookup"><span data-stu-id="75ea2-129">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
- [<span data-ttu-id="75ea2-130">Построение резервное копирование и восстановление приложений для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75ea2-130">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
- [<span data-ttu-id="75ea2-131">Основные понятия резервного копирования и восстановления для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="75ea2-131">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    

