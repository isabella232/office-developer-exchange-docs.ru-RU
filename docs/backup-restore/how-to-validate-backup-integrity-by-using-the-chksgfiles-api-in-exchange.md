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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760923"
---
# <a name="validate-backup-integrity-by-using-the-chksgfiles-api-in-exchange-2013"></a>Проверка целостности резервной копии с помощью CHKSGFILES API в Exchange 2013

Узнайте, как использовать CHKSGFILES API для проверки резервной копии в хранилище Exchange в Exchange 2013.
  
**Применимо к:** Exchange Server 2013 
  
Во время операции резервного копирования, управляемых с службы теневого копирования томов (VSS) Exchange Server 2013 не могут прочитать каждый файл базы данных полностью и проверить его контрольную. Таким образом вы можете резервной копии приложения для проверки целостности файла журнала базы данных и операций. Мы рекомендуем, убедитесь, что приложение резервного копирования физической согласованности set теневой копии до модуля записи Exchange о том, что резервного копирования завершен. После успешного создания резервной копии в хранилище Exchange обновляет заголовки резервные копии баз данных в соответствии с время последней успешной резервной копии и удаляет журналы транзакций с сервера, которые больше не требуются для отката вперед от последней успешной резервной копии.
  
## <a name="prerequisites-for-validating-backup-integrity"></a>Необходимые условия для проверки целостности резервной копии

Перед приложения можно проверить целостность резервной копии, необходимо иметь доступ к таким компонентам:
  
- Файлы из резервной копии хранилища Exchange.
- Версия Visual Studio, начиная с помощью Visual Studio 2010.
- CHKSGFILES библиотеки и файл заголовка. Библиотеки и заголовок файлы можно загрузить из [Центра загрузки Майкрософт](http://www.microsoft.com/en-us/download/details.aspx?id=36802).
    
## <a name="validate-backup-integrity"></a>Проверка целостности резервной копии

Ниже описывается, как проверить целостность данных в набор резервного копирования и восстановления приложения.
  
### <a name="to-validate-backup-integrity"></a>Для проверки целостности резервной копии

1. Создайте новый экземпляр класса **CChkSGFiles** . 
   
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

   Первой строки кода создайте объект error и задать его начальное значение для успеха и создать объект, который проверяет допустимость базы данных. Затем с помощью [функции CChkSGFiles.New](cchksgfiles-new-function.md) создает новый экземпляр класса **CChkSGFiles** . Быстрой проверки новый объект указывает, будет ли найденные проблемы произошла при создании нового экземпляра. 
    
2. Инициализируйте объект **CChkSGFiles** . 
   
   ```cpp
   Call( pcchecksgfiles->ErrInit(
   rgwszDb,
   cDb,
   wszLogPath,
   wszBaseName ) );
   ```
   
   Дополнительные сведения о параметрах [функции CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md)см.
   
3. Используйте [функцию CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md) для проверки целостности базы данных, проверив заголовки базы данных.
   
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
   
   Дополнительные сведения о параметрах [функции CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)см.
   
4. Обработка ошибок и [функция CChkSGFiles.Delete](cchksgfiles-delete-function.md) используется для удаления класса **CChkSGFiles** из памяти. 
   
   ```cpp
   HandleError:
   CCheckSGFiles::Delete( pcchecksgfiles );  
   ```

## <a name="see-also"></a>См. также

- [Справочник по CChkSGFiles классов](cchksgfiles-class-reference.md)
- [Построение резервное копирование и восстановление приложений для Exchange 2013](build-backup-and-restore-applications-for-exchange-2013.md)
- [Основные понятия резервного копирования и восстановления для Exchange 2013](backup-and-restore-concepts-for-exchange-2013.md)
    

