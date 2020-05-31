---
title: Справочник по классу функция cchksgfiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Здесь вы найдете справочные сведения по API ЧКСГФИЛЕС в Exchange 2013.
ms.openlocfilehash: 583ac5e16ab60d119c3028bf81123e9f60a58ff4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760921"
---
# <a name="cchksgfiles-class-reference"></a><span data-ttu-id="3edad-103">Справочник по классу функция cchksgfiles</span><span class="sxs-lookup"><span data-stu-id="3edad-103">CChkSGFiles class reference</span></span>

<span data-ttu-id="3edad-104">Здесь вы найдете справочные сведения по API ЧКСГФИЛЕС в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="3edad-104">Find reference information for the CHKSGFILES API in Exchange 2013.</span></span>
  
<span data-ttu-id="3edad-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="3edad-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="3edad-106">API ЧКСГФИЛЕС позволяет приложениям резервного копирования и восстановления проверять целостность файлов журнала транзакций и баз данных Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3edad-106">The CHKSGFILES API enables backup and restore applications to verify the integrity of Exchange Server 2013 transaction log files and databases programmatically.</span></span> <span data-ttu-id="3edad-107">Этот API можно использовать в приложениях для резервного копирования и восстановления, использующих службу теневого копирования томов (VSS).</span><span class="sxs-lookup"><span data-stu-id="3edad-107">You can use this API in backup and restore applications that use the Volume Shadow Copy Service (VSS).</span></span>
  
> [!NOTE]
> <span data-ttu-id="3edad-108">Группы хранения недоступны в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="3edad-108">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="3edad-109">Поддержка групп хранения была удалена из версий Exchange, начиная с Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="3edad-109">Support for storage groups was removed from versions of Exchange starting with Exchange Server 2010.</span></span> <span data-ttu-id="3edad-110">Для обеспечения обратной совместимости с базами данных и группами хранения в более ранних версиях Exchange, чем Exchange 2010, API ЧКСГФИЛЕС позволяет указать группы хранения.</span><span class="sxs-lookup"><span data-stu-id="3edad-110">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="3edad-111">При запуске ЧКСГФИЛЕС для баз данных Exchange 2013 необходимо задать параметры, указывающие идентификатор группы хранения, в пустую строку.</span><span class="sxs-lookup"><span data-stu-id="3edad-111">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
## <a name="file-location"></a><span data-ttu-id="3edad-112">Расположение файла</span><span class="sxs-lookup"><span data-stu-id="3edad-112">File location</span></span>
<span data-ttu-id="3edad-113"><a name="bk_fileslocation"> </a></span><span class="sxs-lookup"><span data-stu-id="3edad-113"><a name="bk_fileslocation"> </a></span></span>

<span data-ttu-id="3edad-114">API ЧКСГФИЛЕС поставляется в составе Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="3edad-114">The CHKSGFILES API ships as part of Exchange 2013.</span></span> <span data-ttu-id="3edad-115">Этот API можно использовать на компьютере, на котором установлена роль сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="3edad-115">You can use this API on a computer that has the Mailbox server role installed.</span></span> 
  
<span data-ttu-id="3edad-116">По умолчанию библиотека DLL ЧКСГФИЛЕС устанавливается в папку C:\Program Files\Microsoft\Exchange\V15\Bin.</span><span class="sxs-lookup"><span data-stu-id="3edad-116">By default, the CHKSGFILES DLL is installed in the C:\Program Files\Microsoft\Exchange\V15\Bin directory.</span></span>
  
<span data-ttu-id="3edad-117">Exchange 2013 включает только 64-разрядную (AMD64) версию API ЧКСГФИЛЕС.</span><span class="sxs-lookup"><span data-stu-id="3edad-117">Exchange 2013 includes only a 64-bit (amd64) version of the CHKSGFILES API.</span></span> 
  
<span data-ttu-id="3edad-118">Вы можете скачать ZIP-файл, который включает библиотеку ЧКСГФИЛЕ. lib и файлы заголовков ЧКСГФИЛЕС. хкскс для использования в пользовательском приложении, в [центре загрузки Майкрософт](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="3edad-118">You can download a .zip file that includes the CHKSGFILE.lib library and CHKSGFILES.hxx header files for use in your custom application from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
  
## <a name="development-languages"></a><span data-ttu-id="3edad-119">Языки разработки</span><span class="sxs-lookup"><span data-stu-id="3edad-119">Development languages</span></span>
<span data-ttu-id="3edad-120"><a name="bk_developmentlanguages"> </a></span><span class="sxs-lookup"><span data-stu-id="3edad-120"><a name="bk_developmentlanguages"> </a></span></span>

<span data-ttu-id="3edad-121">API ЧКСГФИЛЕС предназначен для использования с версиями Visual Studio, начиная с Visual Studio 2005 в машинном C/C++.</span><span class="sxs-lookup"><span data-stu-id="3edad-121">The CHKSGFILES API is intended for use with versions of Visual Studio starting with Visual Studio 2005 in native C/C++.</span></span> <span data-ttu-id="3edad-122">API ЧКСГФИЛЕС не предназначен для использования в управляемом коде.</span><span class="sxs-lookup"><span data-stu-id="3edad-122">The CHKSGFILES API is not intended for use in managed code.</span></span> <span data-ttu-id="3edad-123">Несмотря на то, что вы можете создать сборку COM-взаимодействия с ЧКСГФИЛЕС, мы не доставлять поддерживаемую сборку COM-взаимодействия с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="3edad-123">Although you can create a COM Interop assembly with CHKSGFILES, we do not ship a supported COM Interop assembly with Exchange 2013.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="3edad-124">В этом разделе:</span><span class="sxs-lookup"><span data-stu-id="3edad-124">In this section</span></span>
<span data-ttu-id="3edad-125"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="3edad-125"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="3edad-126">Функция функция cchksgfiles. Кмаксдбперсг</span><span class="sxs-lookup"><span data-stu-id="3edad-126">CChkSGFiles.CMaxDbPerSG function</span></span>](cchksgfiles-cmaxdbpersg-function.md)
    
- [<span data-ttu-id="3edad-127">Функция функция cchksgfiles. Delete</span><span class="sxs-lookup"><span data-stu-id="3edad-127">CChkSGFiles.Delete function</span></span>](cchksgfiles-delete-function.md)
    
- [<span data-ttu-id="3edad-128">Перечисление функция cchksgfiles. ERR</span><span class="sxs-lookup"><span data-stu-id="3edad-128">CChkSGFiles.ERR enumeration</span></span>](cchksgfiles-err-enumeration.md)
    
- [<span data-ttu-id="3edad-129">Функция функция cchksgfiles. Еррчеккдбхеадерс</span><span class="sxs-lookup"><span data-stu-id="3edad-129">CChkSGFiles.ErrCheckDbHeaders function</span></span>](cchksgfiles-errcheckdbheaders-function.md)
    
- [<span data-ttu-id="3edad-130">Функция функция cchksgfiles. Еррчеккдбпажес</span><span class="sxs-lookup"><span data-stu-id="3edad-130">CChkSGFiles.ErrCheckDbPages function</span></span>](cchksgfiles-errcheckdbpages-function.md)
    
- [<span data-ttu-id="3edad-131">Функция функция cchksgfiles. Еррчекклогс</span><span class="sxs-lookup"><span data-stu-id="3edad-131">CChkSGFiles.ErrCheckLogs function</span></span>](cchksgfiles-errchecklogs-function.md)
    
- [<span data-ttu-id="3edad-132">Функция функция cchksgfiles. Ерржесеадер (зарезервированная)</span><span class="sxs-lookup"><span data-stu-id="3edad-132">CChkSGFiles.ErrGetHeader function (reserved)</span></span>](cchksgfiles-errgetheader-function-reserved.md)
    
- [<span data-ttu-id="3edad-133">Функция функция cchksgfiles. Ерринит</span><span class="sxs-lookup"><span data-stu-id="3edad-133">CChkSGFiles.ErrInit function</span></span>](cchksgfiles-errinit-function.md)
    
- [<span data-ttu-id="3edad-134">Функция функция cchksgfiles. Ерртерм</span><span class="sxs-lookup"><span data-stu-id="3edad-134">CChkSGFiles.ErrTerm function</span></span>](cchksgfiles-errterm-function.md)
    
- [<span data-ttu-id="3edad-135">Перечисление функция cchksgfiles. Идбинвалид</span><span class="sxs-lookup"><span data-stu-id="3edad-135">CChkSGFiles.iDbInvalid enumeration</span></span>](cchksgfiles-idbinvalid-enumeration.md)
    
- [<span data-ttu-id="3edad-136">Функция функция cchksgfiles. New</span><span class="sxs-lookup"><span data-stu-id="3edad-136">CChkSGFiles.New function</span></span>](cchksgfiles-new-function.md)
    
- [<span data-ttu-id="3edad-137">Перечисление функция cchksgfiles. NO_FLAGS</span><span class="sxs-lookup"><span data-stu-id="3edad-137">CChkSGFiles.NO_FLAGS enumeration</span></span>](cchksgfiles-no_flags-enumeration.md)
    
- [<span data-ttu-id="3edad-138">Структура функция cchksgfiles. PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="3edad-138">CChkSGFiles.PAGE_INFO struct</span></span>](cchksgfiles-page_info-struct.md)
    
- [<span data-ttu-id="3edad-139">Функция функция cchksgfiles. Пгнофромфилеоффсет</span><span class="sxs-lookup"><span data-stu-id="3edad-139">CChkSGFiles.PgnoFromFileOffset function</span></span>](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a><span data-ttu-id="3edad-140">См. также</span><span class="sxs-lookup"><span data-stu-id="3edad-140">See also</span></span>

- [<span data-ttu-id="3edad-141">Разработки для Exchange Online и Exchange</span><span class="sxs-lookup"><span data-stu-id="3edad-141">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)
- [<span data-ttu-id="3edad-142">Резервное копирование, восстановление и аварийное восстановление</span><span class="sxs-lookup"><span data-stu-id="3edad-142">Backup, Restore, and Disaster Recovery</span></span>](http://technet.microsoft.com/en-us/library/dd876874)
    

