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
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Проверка целостности резервного копирования с помощью API CHKSGFILES в Exchange 2013

Узнайте, как использовать API CHKSGFILES для проверки резервной копии магазина Exchange в Exchange 2013.
  
**Применимо к:** Exchange Server 2013 
  
Во время операций резервного копирования, управляемых службой теневого копирования томов (VSS), Exchange Server 2013 не может полностью прочитать каждый файл базы данных и проверить его целостность контрольных контрольных объемов. Поэтому может потребоваться, чтобы приложение резервного копирования проверило целостность файлов базы данных и журнала транзакций. Перед тем как сообщить записи Exchange о том, что резервное копирование завершено, приложению резервного копирования рекомендуется проверить физическую согласованность набора теневых копий. После успешного резервного копирования хранилище Exchange обновляет заглавные данные резервных копий баз данных с учетом времени последнего успешного резервного копирования и удаляет журналы транзакций с сервера, которые больше не требуются для отката из последней успешной резервной копии.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Необходимые условия для проверки целостности резервного копирования

Прежде чем приложение сможет проверить целостность резервной копии, необходимо иметь доступ к следующим данным:
  
- Файлы из резервной копии магазина Exchange.
- Версия Visual Studio начиная с Visual Studio 2010.
- Файлы библиотеки и заголовок CHKSGFILES. Вы можете скачать библиотеку и файлы заголовок из [Центра загрузки Майкрософт.](https://www.microsoft.com/download/details.aspx?id=36802)
    
## <a name="validate-backup-integrity"></a>Проверка целостности резервного копирования

В следующей процедуре описывается проверка целостности данных в приложении резервного копирования и восстановления.
  
### <a name="to-validate-backup-integrity"></a>Проверка целостности резервного копирования

1. Создайте новый экземпляр класса **CChkSGFiles.** 
   
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

   Первые строки кода создают объект ошибки и устанавливают его начальное значение успешно, а также создают объект, который проверяет правильность базы данных. Затем функция [CChkSGFiles.New](cchksgfiles-new-function.md) создает новый экземпляр класса **CChkSGFiles.** Быстрая проверка нового объекта указывает, произошли ли проблемы при его создания. 
    
2. Инициализация **объекта CChkSGFiles.** 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Дополнительные сведения о параметрах см. в функции [CChkSGFiles.ErrInit.](cchksgfiles-errinit-function.md)
   
3. Используйте [функцию CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) для проверки целостности базы данных, проверяя их заголовок.
   
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
   
   Дополнительные сведения о параметрах см. в функции [CChkSGFiles.ErrCheckDbHeaders.](cchksgfiles-errcheckdbheaders-function.md)
   
4. Обработать ошибки и использовать функцию [CChkSGFiles.Delete,](cchksgfiles-delete-function.md) чтобы удалить класс **CChkSGFiles** из памяти. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>См. также

- [Справочник по классу CChkSGFiles](cchksgfiles-class-reference.md)
- [Создание приложений резервного копирования и восстановления для Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Концепции резервного копирования и восстановления для Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

