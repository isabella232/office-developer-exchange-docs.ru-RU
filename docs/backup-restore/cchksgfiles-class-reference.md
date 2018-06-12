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
# <a name="cchksgfiles-class-reference"></a>Справочник по CChkSGFiles классов

Найдите справочные сведения для CHKSGFILES API в Exchange 2013.
  
**Применимо к:** Exchange Server 2013 
  
CHKSGFILES API позволяет приложениям резервного копирования и восстановления для проверки целостности базы данных и файлы журнала транзакций Exchange Server 2013 программными средствами. Можно использовать этот интерфейс API в резервного копирования и восстановления приложений, использующих тома теневой копии Service (VSS).
  
> [!NOTE]
> Группы хранения, недоступны в Exchange 2013. Поддержка групп хранения был удален из версии Exchange, начиная с Exchange Server 2010. Для обеспечения обратной совместимости с базами данных и группы хранения в версиях Exchange до Exchange 2010 CHKSGFILES API позволяет указать группы хранения. При выполнении CHKSGFILES баз данных Exchange 2013, необходимо настроить параметры, укажите идентификатор группы хранения пустую строку. 
  
## <a name="file-location"></a>Расположение файлов
<a name="bk_fileslocation"> </a>

CHKSGFILES API входит в состав Exchange 2013. Этот интерфейс API можно использовать на компьютере с установленной ролью сервера почтовых ящиков. 
  
По умолчанию CHKSGFILES DLL устанавливается в каталог C:\Program Files\Microsoft\Exchange\V15\Bin.
  
Exchange 2013 включает в себя только (amd64) 64-разрядная версия CHKSGFILES API. 
  
Вы можете загрузить ZIP-файл, который включает в себя библиотеки CHKSGFILE.lib и CHKSGFILES.hxx файлы заголовков для использования в своем приложении из [Центра загрузки Майкрософт](http://www.microsoft.com/en-us/download/details.aspx?id=36802).
  
## <a name="development-languages"></a>Языков разработки
<a name="bk_developmentlanguages"> </a>

CHKSGFILES API предназначен для использования с версии Visual Studio, начиная с Visual Studio 2005 на C/C++. CHKSGFILES API не предназначен для использования в управляемом коде. Хотя вы можете создать сборкой COM-взаимодействие с CHKSGFILES, мы не поставляются поддерживаемые сборки COM-взаимодействие с Exchange 2013.
  
## <a name="in-this-section"></a>В этом разделе
<a name="bk_inthissection"> </a>

- [Функция CChkSGFiles.CMaxDbPerSG](cchksgfiles-cmaxdbpersg-function.md)
    
- [Функция CChkSGFiles.Delete](cchksgfiles-delete-function.md)
    
- [Перечисление CChkSGFiles.ERR](cchksgfiles-err-enumeration.md)
    
- [Функция CChkSGFiles.ErrCheckDbHeaders](cchksgfiles-errcheckdbheaders-function.md)
    
- [Функция CChkSGFiles.ErrCheckDbPages](cchksgfiles-errcheckdbpages-function.md)
    
- [Функция CChkSGFiles.ErrCheckLogs](cchksgfiles-errchecklogs-function.md)
    
- [Функция CChkSGFiles.ErrGetHeader (зарезервировано)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Функция CChkSGFiles.ErrInit](cchksgfiles-errinit-function.md)
    
- [Функция CChkSGFiles.ErrTerm](cchksgfiles-errterm-function.md)
    
- [Перечисление CChkSGFiles.iDbInvalid](cchksgfiles-idbinvalid-enumeration.md)
    
- [Функция CChkSGFiles.New](cchksgfiles-new-function.md)
    
- [Перечисление CChkSGFiles.NO_FLAGS](cchksgfiles-no_flags-enumeration.md)
    
- [Структура CChkSGFiles.PAGE_INFO](cchksgfiles-page_info-struct.md)
    
- [Функция CChkSGFiles.PgnoFromFileOffset](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>См. также

- [Exchange Online и Exchange (en)](../exchange-server-development.md)
- [Резервное копирование, восстановление и аварийное восстановление](http://technet.microsoft.com/en-us/library/dd876874)
    

