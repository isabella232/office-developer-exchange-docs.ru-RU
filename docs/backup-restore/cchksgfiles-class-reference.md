---
title: Справочник по CChkSGFiles классов
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: Найдите справочные сведения для CHKSGFILES API в Exchange 2013.
ms.openlocfilehash: 583ac5e16ab60d119c3028bf81123e9f60a58ff4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760921"
---
# <a name="cchksgfiles-class-reference"></a><span data-ttu-id="14e1a-103">Справочник по CChkSGFiles классов</span><span class="sxs-lookup"><span data-stu-id="14e1a-103">CChkSGFiles class reference</span></span>

<span data-ttu-id="14e1a-104">Найдите справочные сведения для CHKSGFILES API в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="14e1a-104">Find reference information for the CHKSGFILES API in Exchange 2013.</span></span>
  
<span data-ttu-id="14e1a-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="14e1a-105">**Applies to:** Exchange Server 2013</span></span> 
  
<span data-ttu-id="14e1a-106">CHKSGFILES API позволяет приложениям резервного копирования и восстановления для проверки целостности базы данных и файлы журнала транзакций Exchange Server 2013 программными средствами.</span><span class="sxs-lookup"><span data-stu-id="14e1a-106">The CHKSGFILES API enables backup and restore applications to verify the integrity of Exchange Server 2013 transaction log files and databases programmatically.</span></span> <span data-ttu-id="14e1a-107">Можно использовать этот интерфейс API в резервного копирования и восстановления приложений, использующих тома теневой копии Service (VSS).</span><span class="sxs-lookup"><span data-stu-id="14e1a-107">You can use this API in backup and restore applications that use the Volume Shadow Copy Service (VSS).</span></span>
  
> [!NOTE]
> <span data-ttu-id="14e1a-108">Группы хранения, недоступны в Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="14e1a-108">Storage groups are not available in Exchange 2013.</span></span> <span data-ttu-id="14e1a-109">Поддержка групп хранения был удален из версии Exchange, начиная с Exchange Server 2010.</span><span class="sxs-lookup"><span data-stu-id="14e1a-109">Support for storage groups was removed from versions of Exchange starting with Exchange Server 2010.</span></span> <span data-ttu-id="14e1a-110">Для обеспечения обратной совместимости с базами данных и группы хранения в версиях Exchange до Exchange 2010 CHKSGFILES API позволяет указать группы хранения.</span><span class="sxs-lookup"><span data-stu-id="14e1a-110">For backward compatibility with databases and storage groups in versions of Exchange earlier than Exchange 2010, the CHKSGFILES API enables you to specify storage groups.</span></span> <span data-ttu-id="14e1a-111">При выполнении CHKSGFILES баз данных Exchange 2013, необходимо настроить параметры, укажите идентификатор группы хранения пустую строку.</span><span class="sxs-lookup"><span data-stu-id="14e1a-111">When you run CHKSGFILES against Exchange 2013 databases, you should set parameters that specify a storage group identifier to an empty string.</span></span> 
  
## <a name="file-location"></a><span data-ttu-id="14e1a-112">Расположение файлов</span><span class="sxs-lookup"><span data-stu-id="14e1a-112">File location</span></span>
<span data-ttu-id="14e1a-113"><a name="bk_fileslocation"> </a></span><span class="sxs-lookup"><span data-stu-id="14e1a-113"></span></span>

<span data-ttu-id="14e1a-114">CHKSGFILES API входит в состав Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="14e1a-114">The CHKSGFILES API ships as part of Exchange 2013.</span></span> <span data-ttu-id="14e1a-115">Этот интерфейс API можно использовать на компьютере с установленной ролью сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="14e1a-115">You can use this API on a computer that has the Mailbox server role installed.</span></span> 
  
<span data-ttu-id="14e1a-116">По умолчанию CHKSGFILES DLL устанавливается в каталог C:\Program Files\Microsoft\Exchange\V15\Bin.</span><span class="sxs-lookup"><span data-stu-id="14e1a-116">By default, the CHKSGFILES DLL is installed in the C:\Program Files\Microsoft\Exchange\V15\Bin directory.</span></span>
  
<span data-ttu-id="14e1a-117">Exchange 2013 включает в себя только (amd64) 64-разрядная версия CHKSGFILES API.</span><span class="sxs-lookup"><span data-stu-id="14e1a-117">Exchange 2013 includes only a 64-bit (amd64) version of the CHKSGFILES API.</span></span> 
  
<span data-ttu-id="14e1a-118">Вы можете загрузить ZIP-файл, который включает в себя библиотеки CHKSGFILE.lib и CHKSGFILES.hxx файлы заголовков для использования в своем приложении из [Центра загрузки Майкрософт](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span><span class="sxs-lookup"><span data-stu-id="14e1a-118">You can download a .zip file that includes the CHKSGFILE.lib library and CHKSGFILES.hxx header files for use in your custom application from the [Microsoft Download Center](http://www.microsoft.com/en-us/download/details.aspx?id=36802).</span></span>
  
## <a name="development-languages"></a><span data-ttu-id="14e1a-119">Языков разработки</span><span class="sxs-lookup"><span data-stu-id="14e1a-119">Development languages</span></span>
<span data-ttu-id="14e1a-120"><a name="bk_developmentlanguages"> </a></span><span class="sxs-lookup"><span data-stu-id="14e1a-120"></span></span>

<span data-ttu-id="14e1a-121">CHKSGFILES API предназначен для использования с версии Visual Studio, начиная с Visual Studio 2005 на C/C++.</span><span class="sxs-lookup"><span data-stu-id="14e1a-121">The CHKSGFILES API is intended for use with versions of Visual Studio starting with Visual Studio 2005 in native C/C++.</span></span> <span data-ttu-id="14e1a-122">CHKSGFILES API не предназначен для использования в управляемом коде.</span><span class="sxs-lookup"><span data-stu-id="14e1a-122">The CHKSGFILES API is not intended for use in managed code.</span></span> <span data-ttu-id="14e1a-123">Хотя вы можете создать сборкой COM-взаимодействие с CHKSGFILES, мы не поставляются поддерживаемые сборки COM-взаимодействие с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="14e1a-123">Although you can create a COM Interop assembly with CHKSGFILES, we do not ship a supported COM Interop assembly with Exchange 2013.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="14e1a-124">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="14e1a-124">In this section</span></span>
<span data-ttu-id="14e1a-125"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="14e1a-125"></span></span>

- [<span data-ttu-id="14e1a-126">Функция CChkSGFiles.CMaxDbPerSG</span><span class="sxs-lookup"><span data-stu-id="14e1a-126">CChkSGFiles.CMaxDbPerSG function</span></span>](cchksgfiles-cmaxdbpersg-function.md)
    
- [<span data-ttu-id="14e1a-127">Функция CChkSGFiles.Delete</span><span class="sxs-lookup"><span data-stu-id="14e1a-127">CChkSGFiles.Delete function</span></span>](cchksgfiles-delete-function.md)
    
- [<span data-ttu-id="14e1a-128">Перечисление CChkSGFiles.ERR</span><span class="sxs-lookup"><span data-stu-id="14e1a-128">CChkSGFiles.ERR enumeration</span></span>](cchksgfiles-err-enumeration.md)
    
- [<span data-ttu-id="14e1a-129">Функция CChkSGFiles.ErrCheckDbHeaders</span><span class="sxs-lookup"><span data-stu-id="14e1a-129">CChkSGFiles.ErrCheckDbHeaders function</span></span>](cchksgfiles-errcheckdbheaders-function.md)
    
- [<span data-ttu-id="14e1a-130">Функция CChkSGFiles.ErrCheckDbPages</span><span class="sxs-lookup"><span data-stu-id="14e1a-130">CChkSGFiles.ErrCheckDbPages function</span></span>](cchksgfiles-errcheckdbpages-function.md)
    
- [<span data-ttu-id="14e1a-131">Функция CChkSGFiles.ErrCheckLogs</span><span class="sxs-lookup"><span data-stu-id="14e1a-131">CChkSGFiles.ErrCheckLogs function</span></span>](cchksgfiles-errchecklogs-function.md)
    
- [<span data-ttu-id="14e1a-132">Функция CChkSGFiles.ErrGetHeader (зарезервировано)</span><span class="sxs-lookup"><span data-stu-id="14e1a-132">CChkSGFiles.ErrGetHeader function (reserved)</span></span>](cchksgfiles-errgetheader-function-reserved.md)
    
- [<span data-ttu-id="14e1a-133">Функция CChkSGFiles.ErrInit</span><span class="sxs-lookup"><span data-stu-id="14e1a-133">CChkSGFiles.ErrInit function</span></span>](cchksgfiles-errinit-function.md)
    
- [<span data-ttu-id="14e1a-134">Функция CChkSGFiles.ErrTerm</span><span class="sxs-lookup"><span data-stu-id="14e1a-134">CChkSGFiles.ErrTerm function</span></span>](cchksgfiles-errterm-function.md)
    
- [<span data-ttu-id="14e1a-135">Перечисление CChkSGFiles.iDbInvalid</span><span class="sxs-lookup"><span data-stu-id="14e1a-135">CChkSGFiles.iDbInvalid enumeration</span></span>](cchksgfiles-idbinvalid-enumeration.md)
    
- [<span data-ttu-id="14e1a-136">Функция CChkSGFiles.New</span><span class="sxs-lookup"><span data-stu-id="14e1a-136">CChkSGFiles.New function</span></span>](cchksgfiles-new-function.md)
    
- [<span data-ttu-id="14e1a-137">Перечисление CChkSGFiles.NO_FLAGS</span><span class="sxs-lookup"><span data-stu-id="14e1a-137">CChkSGFiles.NO_FLAGS enumeration</span></span>](cchksgfiles-no_flags-enumeration.md)
    
- [<span data-ttu-id="14e1a-138">Структура CChkSGFiles.PAGE_INFO</span><span class="sxs-lookup"><span data-stu-id="14e1a-138">CChkSGFiles.PAGE_INFO struct</span></span>](cchksgfiles-page_info-struct.md)
    
- [<span data-ttu-id="14e1a-139">Функция CChkSGFiles.PgnoFromFileOffset</span><span class="sxs-lookup"><span data-stu-id="14e1a-139">CChkSGFiles.PgnoFromFileOffset function</span></span>](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a><span data-ttu-id="14e1a-140">См. также</span><span class="sxs-lookup"><span data-stu-id="14e1a-140">See also</span></span>

- [<span data-ttu-id="14e1a-141">Exchange Online и Exchange (en)</span><span class="sxs-lookup"><span data-stu-id="14e1a-141">Exchange Online and Exchange development</span></span>](../exchange-server-development.md)
- [<span data-ttu-id="14e1a-142">Резервное копирование, восстановление и аварийное восстановление</span><span class="sxs-lookup"><span data-stu-id="14e1a-142">Backup, Restore, and Disaster Recovery</span></span>](http://technet.microsoft.com/en-us/library/dd876874)
    

