---
title: Справочник по классу CChkSGFiles
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 9347d5f6-95bb-4045-9c86-0dc0ded24fe8
description: В 2013 г. найдите справочные сведения для API CHKSGFILES Exchange 2013 г.
ms.openlocfilehash: 2daf31c41a47684b85ede196b415884335c3ca79
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510535"
---
# <a name="cchksgfiles-class-reference"></a>Справочник по классу CChkSGFiles

В 2013 г. найдите справочные сведения для API CHKSGFILES Exchange 2013 г.
  
**Применяется к:** Exchange Server 2013 г. 
  
API CHKSGFILES позволяет приложениям резервного копирования и восстановления проверять целостность файлов журналов транзакций 2013 Exchange Server 2013 г. программным образом. Этот API можно использовать в резервном копировании и восстановлении приложений, которые используют службу копирования теней тома (VSS).
  
> [!NOTE]
> служба хранилища группы недоступны в Exchange 2013 г. Поддержка групп хранения была удалена из версий Exchange начиная с Exchange Server 2010 г. Для обратной совместимости с базами данных и группами хранения в версиях Exchange до Exchange 2010 г. API CHKSGFILES позволяет указать группы хранения. При запуске CHKSGFILES Exchange баз данных 2013 года необходимо задать параметры, указывав идентификатор группы хранения на пустую строку. 
  
## <a name="file-location"></a>Расположение файла
<a name="bk_fileslocation"> </a>

API CHKSGFILES в рамках Exchange 2013 г. Этот API можно использовать на компьютере, где установлена роль сервера почтовых ящиков. 
  
По умолчанию DLL CHKSGFILES устанавливается в каталоге C:\Program Files\Microsoft\Exchange\V15\Bin.
  
Exchange 2013 включает только 64-битную (amd64) версию API CHKSGFILES. 
  
Вы можете скачать файл .zip, который включает библиотеку CHKSGFILE.lib и файлы заголовки CHKSGFILES.hxx для использования в настраиваемом приложении из Центра загрузки [Майкрософт.](https://www.microsoft.com/download/details.aspx?id=36802)
  
## <a name="development-languages"></a>Языки разработки
<a name="bk_developmentlanguages"> </a>

API CHKSGFILES предназначен для использования с версиями Visual Studio начиная с Visual Studio 2005 г. в родном C/C++. API CHKSGFILES не предназначен для использования в управляемом коде. Хотя вы можете создать сборку COM Interop с помощью CHKSGFILES, мы не отгрузим поддерживаемую сборку COM Interop Exchange 2013.
  
## <a name="in-this-section"></a>В этом разделе:
<a name="bk_inthissection"> </a>

- [Функция CChkSGFiles.CMaxDbPerSG](cchksgfiles-cmaxdbpersg-function.md)
    
- [Функция CChkSGFiles.Delete](cchksgfiles-delete-function.md)
    
- [Перечисление CChkSGFiles.ERR](cchksgfiles-err-enumeration.md)
    
- [Функция CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)
    
- [Функция CChkSGFiles.ErrCheckDbPages](cchksgfiles-errcheckdbpages-function.md)
    
- [Функция CChkSGFiles.ErrCheckLogs](cchksgfiles-errchecklogs-function.md)
    
- [Функция CChkSGFiles.ErrGetHeader (зарезервированная)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Функция CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md)
    
- [Функция CChkSGFiles.ErrTerm](cchksgfiles-errterm-function.md)
    
- [Перечисление CChkSGFiles.iDbInvalid](cchksgfiles-idbinvalid-enumeration.md)
    
- [Функция CChkSGFiles.New](cchksgfiles-new-function.md)
    
- [Перечисление CChkSGFiles.NO_FLAGS](cchksgfiles-no_flags-enumeration.md)
    
- [Структура CChkSGFiles.PAGE_INFO](cchksgfiles-page_info-struct.md)
    
- [Функция CChkSGFiles.PgnoFromFileOffset](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>См. также

- [Разработки для Exchange Online и Exchange](../exchange-server-development.md)
- [Резервное копирование, восстановление и аварийное восстановление](https://technet.microsoft.com/library/dd876874)
    

