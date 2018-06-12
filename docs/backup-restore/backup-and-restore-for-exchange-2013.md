---
title: Резервное копирование и восстановление для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 329902d9-0ecb-4cfb-86dd-5ce863deff3f
description: Найдите сведения о создании резервное копирование и восстановление приложений для Exchange 2013.
ms.openlocfilehash: 9eceb3d512a73ad9cb07a01864fb8b029d5b5772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760917"
---
# <a name="backup-and-restore-for-exchange"></a><span data-ttu-id="a7aa3-103">Резервное копирование и восстановление для Exchange</span><span class="sxs-lookup"><span data-stu-id="a7aa3-103">Backup and restore for Exchange</span></span>
  
<span data-ttu-id="a7aa3-104">Exchange Server 2013 предоставляет группы обеспечения доступности баз данных (DAGs), помогающий для хранения хранимых данных, безопасности и доступности и сократить потребность в пользовательских резервное копирование и восстановление приложений.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-104">Exchange Server 2013 provides Database Availability Groups (DAGs), which help to keep stored data secure and available, and reduce the need for custom backup and restore applications.</span></span> <span data-ttu-id="a7aa3-105">DAG обеспечения резервирования внешних данных для обеспечения потерю данных.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-105">DAGs enable off-site data redundancy to help ensure that you won't lose data.</span></span> <span data-ttu-id="a7aa3-106">Тем не менее многие планы аварийного восстановления продолжить включают более традиционный резервного копирования и восстановления системы, включая настраиваемые приложения, для обеспечения избыточности с доступности базы данных и методы.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-106">However, many disaster recovery plans continue to include more traditional backup and restore methods and systems, including custom applications, for redundancy with the DAG.</span></span> <span data-ttu-id="a7aa3-107">Чтобы обеспечить доступность данных и обеспечения избыточности в вашей организации, можно создать настраиваемые приложения, использующие технологии операционной системы Exchange Server и Windows Server для резервного копирования и восстановления данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-107">To help ensure data availability and redundancy in your organization, you can create custom applications that use Exchange Server and Windows Server operating system technologies to back up and restore your Exchange data.</span></span>

<span data-ttu-id="a7aa3-108"><a name="bk_plugin"> </a></span><span class="sxs-lookup"><span data-stu-id="a7aa3-108"></span></span>

## <a name="backup-technologies-in-exchange-2013"></a><span data-ttu-id="a7aa3-109">Технологии резервного копирования в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a7aa3-109">Backup technologies in Exchange 2013</span></span>

<span data-ttu-id="a7aa3-110">Exchange 2013 включает в себя подключаемый модуль для резервного копирования Windows Server, который администраторы могут использовать для создания на основе VSS резервной копии данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-110">Exchange 2013 includes a plug-in for Windows Server Backup that administrators can use to make VSS-based backups of Exchange data.</span></span> <span data-ttu-id="a7aa3-111">Администраторы могут также использовать резервного копирования Windows Server для резервного копирования и восстановления баз данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-111">Administrators can also use Windows Server Backup to back up and restore Exchange databases.</span></span> <span data-ttu-id="a7aa3-112">Если вы создаете резервного копирования и восстановления приложения для Exchange 2013, необходимо создать приложение с поддержкой Exchange, поддерживающего модуля записи VSS Exchange 2013 и использования CHKSGFILES API для проверки согласованности, резервного копирования.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-112">If you are creating a backup and restore application for Exchange 2013, you need to create an Exchange-aware application that supports the VSS writer for Exchange 2013, and use the CHKSGFILES API to validate the consistency of that backup.</span></span> <span data-ttu-id="a7aa3-113">Дополнительные сведения можно [проверить целостность резервной копии с помощью CHKSGFILES API в Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a7aa3-113">For more information, see [Validate backup integrity by using the CHKSGFILES API in Exchange 2013](how-to-validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange.md).</span></span>

<span data-ttu-id="a7aa3-114"><a name="bk_vsswriter"> </a></span><span class="sxs-lookup"><span data-stu-id="a7aa3-114"></span></span>

## <a name="vss-writer-in-exchange-2013"></a><span data-ttu-id="a7aa3-115">Модуль записи VSS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a7aa3-115">VSS writer in Exchange 2013</span></span>

<span data-ttu-id="a7aa3-116">Exchange 2013 представляется значительные изменения в архитектуре модуля записи VSS в Exchange Server 2010 и Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-116">Exchange 2013 introduces a significant change to the VSS writer architecture in Exchange Server 2010 and Exchange Server 2007.</span></span> <span data-ttu-id="a7aa3-117">Exchange 2010 и Exchange 2007 включают две записи VSS: один в службу банка данных Exchange (store.exe) и один в службе репликации Exchange (msexchangerepl.exe).</span><span class="sxs-lookup"><span data-stu-id="a7aa3-117">Exchange 2010 and Exchange 2007 include two VSS writers: one inside the Exchange Information Store service (store.exe) and one inside the Exchange Replication service (msexchangerepl.exe).</span></span> <span data-ttu-id="a7aa3-118">В Exchange 2013, функции модуля записи VSS находится в службе репликации Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-118">In Exchange 2013, the VSS writer functionality is located in the Exchange Replication service.</span></span> <span data-ttu-id="a7aa3-119">Резервное копирование и восстановление приложения с помощью нового модуля записи VSS, называется записи Microsoft Exchange, для резервного копирования базы данных активных и пассивных копий и восстановить резервные копии копий базы данных.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-119">Your backup and restore application uses the new VSS writer, called the Microsoft Exchange Writer, to back up active and passive database copies, and to restore backed up database copies.</span></span> <span data-ttu-id="a7aa3-120">Несмотря на то, что нового модуля записи VSS запускается в службе репликации Exchange, в порядке для модуля записи, чтобы оно было доступно должна быть запущена служба банка данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-120">Although the new VSS writer runs in the Exchange Replication service, the Exchange Information Store service must be running in order for the writer to be available.</span></span> <span data-ttu-id="a7aa3-121">В результате обе службы необходимы для резервного копирования или восстановления баз данных Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-121">As a result, both services are required to back up or restore Exchange databases.</span></span>
  
<span data-ttu-id="a7aa3-122">Несмотря на то, что архитектура модуля записи VSS были добавлены в Exchange 2013, базовой функциональности не был изменен.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-122">Although the VSS writer architecture was updated in Exchange 2013, the underlying functionality has not changed.</span></span> <span data-ttu-id="a7aa3-123">Если вы создали резервное копирование и восстановление приложений для Exchange 2010, вносить изменения в приложении для Exchange 2013 не требуется.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-123">If you created a backup and restore application for Exchange 2010, you do not need to make any changes to your application for Exchange 2013.</span></span> <span data-ttu-id="a7aa3-124">Необходимо перекомпилировать приложение с последние файлы для обеспечения совместимости.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-124">Be sure to recompile your application with the latest files to ensure compatibility.</span></span> <span data-ttu-id="a7aa3-125">Для резервного копирования и восстановления приложения, созданные для Exchange 2007 или более ранней версии необходимо будет переписать код, чтобы использовать новейшие CHKSGFILES API.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-125">For backup and restore applications created for Exchange 2007 or earlier versions, you will need to rewrite your code to use the latest CHKSGFILES API.</span></span>
  
## <a name="what-you-need-to-know-about-vss-backup-and-restore"></a><span data-ttu-id="a7aa3-126">Что нужно знать о служба теневого копирования ТОМОВ резервное копирование и восстановление</span><span class="sxs-lookup"><span data-stu-id="a7aa3-126">What you need to know about VSS backup and restore</span></span>

|<span data-ttu-id="a7aa3-127">Если вам интересно о...</span><span class="sxs-lookup"><span data-stu-id="a7aa3-127">If you're wondering about…</span></span>|<span data-ttu-id="a7aa3-128">Прочтите это</span><span class="sxs-lookup"><span data-stu-id="a7aa3-128">Read this</span></span>|
|:-----|:-----|
|<span data-ttu-id="a7aa3-129">Application architectures</span><span class="sxs-lookup"><span data-stu-id="a7aa3-129">Application architectures</span></span>  <br/> |<span data-ttu-id="a7aa3-130">Резервное копирование и восстановление приложений, использующих служба теневого копирования ТОМОВ для резервного копирования баз данных обычно состоят из службы фона, используемая для выполнения резервного копирования, планирования службы и приложения консоли графического интерфейса пользователя Windows, который определяет и настраивает резервного копирования и восстановления системы Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-130">Backup and restore applications that use VSS to back up Exchange databases typically consist of a background service that performs the backup, a scheduling service, and a Windows GUI application console that controls and configures the backup and restore system.</span></span>  <br/> |
|<span data-ttu-id="a7aa3-131">Remote usage</span><span class="sxs-lookup"><span data-stu-id="a7aa3-131">Remote usage</span></span>  <br/> |<span data-ttu-id="a7aa3-132">Приложения, использующие служба теневого копирования ТОМОВ для резервного копирования серверов Exchange необходимо выполнить на компьютере Windows Server 2008, на котором выполняется процесс хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-132">Applications that use VSS to back up Exchange servers must run on the Windows Server 2008 computer on which the Exchange store process is running.</span></span> <span data-ttu-id="a7aa3-133">Из-за гибкость систем с большим объемом памяти оборудования, размещения тома хранилища может не входить физически компьютера под управлением Windows Server 2008.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-133">Because of the flexibility in large storage systems, the hardware hosting the storage volumes might not physically be part of the computer running Windows Server 2008.</span></span>  <br/> |
|<span data-ttu-id="a7aa3-134">Languages and tools</span><span class="sxs-lookup"><span data-stu-id="a7aa3-134">Languages and tools</span></span>  <br/> |<span data-ttu-id="a7aa3-135">Можно использовать любой язык, совместимых с COM для использования службы VSS.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-135">You can use any COM-compatible language to use VSS.</span></span> <span data-ttu-id="a7aa3-136">Наиболее часто используется в приложениях, написанных на языке C++.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-136">It is most frequently used in applications written in C++.</span></span> <span data-ttu-id="a7aa3-137">Поскольку используется для создания теневой копии в хранилище Exchange в автономном режиме, резервного копирования приложения, обычно ограниченным временем, который в большинстве случаев упрощает использование таких языков, как Visual Basic или VBScript нецелесообразным.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-137">Because you have to take the Exchange store offline to create shadow copies, backup applications are typically time-sensitive, which in most cases makes using languages like Visual Basic or VBScript impractical.</span></span>  <br/> |
|<span data-ttu-id="a7aa3-138">Managed implementation</span><span class="sxs-lookup"><span data-stu-id="a7aa3-138">Managed implementation</span></span>  <br/> |<span data-ttu-id="a7aa3-139">Можно использовать API служба теневого копирования ТОМОВ в среде с управляемым кодом с помощью COM сборкой взаимодействия.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-139">You can use the VSS APIs in a managed code environment via a COM Interop Assembly.</span></span>  <br/> |
|<span data-ttu-id="a7aa3-140">Scriptable</span><span class="sxs-lookup"><span data-stu-id="a7aa3-140">Scriptable</span></span>  <br/> |<span data-ttu-id="a7aa3-141">Да, но это не рекомендуется.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-141">Yes, but not recommended.</span></span>  <br/> |
|<span data-ttu-id="a7aa3-142">Доступные инструменты для тестирования и отладки</span><span class="sxs-lookup"><span data-stu-id="a7aa3-142">Available test and debug tools</span></span>  <br/> |<span data-ttu-id="a7aa3-143">Специальные инструменты не требуются для отладки приложения, использующие Windows VSS.</span><span class="sxs-lookup"><span data-stu-id="a7aa3-143">No special tools are required to debug applications that use the Windows VSS.</span></span>  <br/> |
   
## <a name="in-this-section"></a><span data-ttu-id="a7aa3-144">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="a7aa3-144">In this section</span></span>

- [<span data-ttu-id="a7aa3-145">Основные понятия резервного копирования и восстановления для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a7aa3-145">Backup and restore concepts for Exchange 2013</span></span>](backup-and-restore-concepts-for-exchange-2013.md)
    
- [<span data-ttu-id="a7aa3-146">Построение резервное копирование и восстановление приложений для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="a7aa3-146">Build backup and restore applications for Exchange 2013</span></span>](build-backup-and-restore-applications-for-exchange-2013.md)
    
- [<span data-ttu-id="a7aa3-147">Справочник по CChkSGFiles классов</span><span class="sxs-lookup"><span data-stu-id="a7aa3-147">CChkSGFiles class reference</span></span>](cchksgfiles-class-reference.md)
    
## <a name="see-also"></a><span data-ttu-id="a7aa3-148">См. также</span><span class="sxs-lookup"><span data-stu-id="a7aa3-148">See also</span></span>

- [<span data-ttu-id="a7aa3-149">Службы теневого копирования томов (Windows)</span><span class="sxs-lookup"><span data-stu-id="a7aa3-149">Volume Shadow Copy Service (Windows)</span></span>](http://msdn.microsoft.com/en-us/library/windows/desktop/bb968832%28v=vs.85%29.aspx)   
- [<span data-ttu-id="a7aa3-150">Сведения об управляемом API EWS, EWS и веб-службах в Exchange</span><span class="sxs-lookup"><span data-stu-id="a7aa3-150">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)  
- [<span data-ttu-id="a7aa3-151">Командная консоль Exchange</span><span class="sxs-lookup"><span data-stu-id="a7aa3-151">Exchange Management Shell</span></span>](../management/exchange-management-shell.md)   
- [<span data-ttu-id="a7aa3-152">Агенты транспорта в Exchange</span><span class="sxs-lookup"><span data-stu-id="a7aa3-152">Transport agents in Exchange</span></span>](../transport-agents/transport-agents-in-exchange-2013.md) 
    
