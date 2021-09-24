---
title: Проверка целостности резервного копирования с помощью API CHKSGFILES в Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 607cbeb9-0a02-4079-8a4d-34bdeb560224
description: Узнайте, как использовать API CHKSGFILES для проверки резервного копирования Exchange магазина в Exchange 2013 г.
ms.openlocfilehash: 7a12a0a8f66128970a782da50ba59f41767c60d3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516232"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Проверка целостности резервного копирования с помощью API CHKSGFILES в Exchange 2013 г.

Узнайте, как использовать API CHKSGFILES для проверки резервного копирования Exchange магазина в Exchange 2013 г.
  
**Применяется к:** Exchange Server 2013 г. 
  
Во время операций резервного копирования, управляемых Службой копирования теней тома (VSS), Exchange Server 2013 г. не может полностью прочитать каждый файл базы данных и проверить его целостность. Поэтому может потребоваться, чтобы приложение резервного копирования проверило целостность файлов базы данных и журнала транзакций. Мы рекомендуем приложению резервного копирования проверить физическую последовательность набора теневых копий перед тем, как сообщить Exchange, что резервное копирование завершено. После успешного резервного копирования Exchange обновляет заглавные главы резервной базы данных, чтобы отразить последнее успешное время резервного копирования и удаляет журналы транзакций с сервера, которые больше не требуются для перекатки из последнего успешного резервного копирования.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Необходимые условия для проверки целостности резервного копирования

Прежде чем приложение сможет проверить целостность резервного копирования, необходимо получить доступ к следующим данным:
  
- Файлы из резервного Exchange хранения.
- Версия Visual Studio начиная с Visual Studio 2010 г.
- Файлы библиотеки и заголовки CHKSGFILES. Вы можете скачать файлы библиотеки и заголовки из [Центра загрузки Майкрософт.](https://www.microsoft.com/download/details.aspx?id=36802)
    
## <a name="validate-backup-integrity"></a>Проверка целостности резервного копирования

Следующая процедура описывает проверку целостности данных в резервном копировании и восстановлении приложения.
  
### <a name="to-validate-backup-integrity"></a>Проверка целостности резервного копирования

1. Создание нового экземпляра **класса CChkSGFiles.** 
   
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

   Первые строки кода создают объект ошибки и устанавливают его начальное значение для успешности, а также создают объект, проверяя достоверность базы данных. Затем функция [CChkSGFiles.New](cchksgfiles-new-function.md) создает новый экземпляр класса **CChkSGFiles.** Быстрая проверка нового объекта указывает, произошли ли какие-либо проблемы при создания нового экземпляра. 
    
2. Инициализация **объекта CChkSGFiles.** 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Дополнительные сведения о параметрах см. в [функции CChkSGFiles.ErrInit.](cchksgfiles-errinit-function.md)
   
3. Используйте [функцию CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) для проверки целостности базы данных, проверяя заголовок баз данных.
   
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
   
4. Обработка ошибок и использование [функции CChkSGFiles.Delete](cchksgfiles-delete-function.md) для удаления класса **CChkSGFiles** из памяти. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>См. также

- [Справочник по классу CChkSGFiles](cchksgfiles-class-reference.md)
- [Создание приложений резервного копирования и восстановления для Exchange 2013 г.](build-backup-and-restore-applications-for-exchange-2013.md)
- [Концепции резервного копирования и восстановления Exchange 2013 г.](backup-and-restore-concepts-for-exchange-2013.md)
    

