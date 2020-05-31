---
title: Проверка целостности резервной копии с помощью API ЧКСГФИЛЕС в Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Узнайте, как использовать API ЧКСГФИЛЕС для проверки резервной копии хранилища Exchange в Exchange 2013.
ms.openlocfilehash: 968484cd5bb7439730685643683e1d850bec33ca
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760923"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Проверка целостности резервной копии с помощью API ЧКСГФИЛЕС в Exchange 2013

Узнайте, как использовать API ЧКСГФИЛЕС для проверки резервной копии хранилища Exchange в Exchange 2013.
  
**Применимо к:** Exchange Server 2013 
  
Во время операций резервного копирования, управляемых службой теневого копирования томов (VSS), Exchange Server 2013 не может прочитать каждый файл базы данных целиком и проверить его целостность. Поэтому может потребоваться, чтобы приложение для резервного копирования пробыло проверку целостности базы данных и файла журнала транзакций. Рекомендуется проверять физическую согласованность набора теневых копий до того, как вы информируете автора Exchange о завершении резервного копирования. После успешного резервного копирования хранилище Exchange обновляет заголовки баз данных с резервным копированием в соответствии со временем последней успешной резервного копирования и удаляет из сервера журналы транзакций, которые больше не требуются для перемотки от последней успешной резервной копии.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Необходимые условия для проверки целостности резервной копии

Прежде чем приложение сможет проверить целостность резервной копии, необходимо иметь доступ к следующим серверам:
  
- Файлы из резервной копии хранилища Exchange.
- Версия Visual Studio, начиная с Visual Studio 2010.
- Библиотека ЧКСГФИЛЕС и файлы заголовков. Вы можете скачать библиотеку и файлы заголовков из [центра загрузки Майкрософт](http://www.microsoft.com/en-us/download/details.aspx?id=36802).
    
## <a name="validate-backup-integrity"></a>Проверка целостности резервной копии

В следующей процедуре описывается проверка целостности данных в приложении резервного копирования и восстановления.
  
### <a name="to-validate-backup-integrity"></a>Проверка целостности резервной копии

1. Создайте новый экземпляр класса **функция cchksgfiles** . 
   
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

   Первые строки кода создают объект Error и задают для его начального значения значение Success и создают объект, проверяющий допустимость базы данных. Затем [функция функция cchksgfiles. New](cchksgfiles-new-function.md) создает новый экземпляр класса **функция cchksgfiles** . Быстрая проверка нового объекта указывает, возникли ли какие либо проблемы при создании нового экземпляра. 
    
2. Инициализация объекта **функция cchksgfiles** . 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Дополнительные сведения о параметрах можно найти в разделе [функция cchksgfiles. ерринит](cchksgfiles-errinit-function.md).
   
3. Используйте [функцию Функция cchksgfiles. еррчеккдбхеадерс](cchksgfiles-errcheckdbheaders-function.md) для проверки целостности базы данных путем проверки заголовков баз данных.
   
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
   
   Дополнительные сведения о параметрах можно найти в разделе [функция cchksgfiles. еррчеккдбхеадерс](cchksgfiles-errcheckdbheaders-function.md).
   
4. Обработка ошибок и использование [функции функция cchksgfiles. Delete](cchksgfiles-delete-function.md) для удаления класса **функция cchksgfiles** из памяти. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>См. также

- [Справочник по классу функция cchksgfiles](cchksgfiles-class-reference.md)
- [Создание приложений резервного копирования и восстановления для Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Основные понятия резервного копирования и восстановления для Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

