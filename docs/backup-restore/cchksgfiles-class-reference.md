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
# <a name="cchksgfiles-class-reference"></a>Справочник по классу функция cchksgfiles

Здесь вы найдете справочные сведения по API ЧКСГФИЛЕС в Exchange 2013.
  
**Применимо к:** Exchange Server 2013 
  
API ЧКСГФИЛЕС позволяет приложениям резервного копирования и восстановления проверять целостность файлов журнала транзакций и баз данных Exchange Server 2013. Этот API можно использовать в приложениях для резервного копирования и восстановления, использующих службу теневого копирования томов (VSS).
  
> [!NOTE]
> Группы хранения недоступны в Exchange 2013. Поддержка групп хранения была удалена из версий Exchange, начиная с Exchange Server 2010. Для обеспечения обратной совместимости с базами данных и группами хранения в более ранних версиях Exchange, чем Exchange 2010, API ЧКСГФИЛЕС позволяет указать группы хранения. При запуске ЧКСГФИЛЕС для баз данных Exchange 2013 необходимо задать параметры, указывающие идентификатор группы хранения, в пустую строку. 
  
## <a name="file-location"></a>Расположение файла
<a name="bk_fileslocation"> </a>

API ЧКСГФИЛЕС поставляется в составе Exchange 2013. Этот API можно использовать на компьютере, на котором установлена роль сервера почтовых ящиков. 
  
По умолчанию библиотека DLL ЧКСГФИЛЕС устанавливается в папку C:\Program Files\Microsoft\Exchange\V15\Bin.
  
Exchange 2013 включает только 64-разрядную (AMD64) версию API ЧКСГФИЛЕС. 
  
Вы можете скачать ZIP-файл, который включает библиотеку ЧКСГФИЛЕ. lib и файлы заголовков ЧКСГФИЛЕС. хкскс для использования в пользовательском приложении, в [центре загрузки Майкрософт](http://www.microsoft.com/en-us/download/details.aspx?id=36802).
  
## <a name="development-languages"></a>Языки разработки
<a name="bk_developmentlanguages"> </a>

API ЧКСГФИЛЕС предназначен для использования с версиями Visual Studio, начиная с Visual Studio 2005 в машинном C/C++. API ЧКСГФИЛЕС не предназначен для использования в управляемом коде. Несмотря на то, что вы можете создать сборку COM-взаимодействия с ЧКСГФИЛЕС, мы не доставлять поддерживаемую сборку COM-взаимодействия с Exchange 2013.
  
## <a name="in-this-section"></a>В этом разделе:
<a name="bk_inthissection"> </a>

- [Функция функция cchksgfiles. Кмаксдбперсг](cchksgfiles-cmaxdbpersg-function.md)
    
- [Функция функция cchksgfiles. Delete](cchksgfiles-delete-function.md)
    
- [Перечисление функция cchksgfiles. ERR](cchksgfiles-err-enumeration.md)
    
- [Функция функция cchksgfiles. Еррчеккдбхеадерс](cchksgfiles-errcheckdbheaders-function.md)
    
- [Функция функция cchksgfiles. Еррчеккдбпажес](cchksgfiles-errcheckdbpages-function.md)
    
- [Функция функция cchksgfiles. Еррчекклогс](cchksgfiles-errchecklogs-function.md)
    
- [Функция функция cchksgfiles. Ерржесеадер (зарезервированная)](cchksgfiles-errgetheader-function-reserved.md)
    
- [Функция функция cchksgfiles. Ерринит](cchksgfiles-errinit-function.md)
    
- [Функция функция cchksgfiles. Ерртерм](cchksgfiles-errterm-function.md)
    
- [Перечисление функция cchksgfiles. Идбинвалид](cchksgfiles-idbinvalid-enumeration.md)
    
- [Функция функция cchksgfiles. New](cchksgfiles-new-function.md)
    
- [Перечисление функция cchksgfiles. NO_FLAGS](cchksgfiles-no_flags-enumeration.md)
    
- [Структура функция cchksgfiles. PAGE_INFO](cchksgfiles-page_info-struct.md)
    
- [Функция функция cchksgfiles. Пгнофромфилеоффсет](cchksgfiles-pgnofromfileoffset-function.md)
    
## <a name="see-also"></a>См. также

- [Разработки для Exchange Online и Exchange](../exchange-server-development.md)
- [Резервное копирование, восстановление и аварийное восстановление](http://technet.microsoft.com/en-us/library/dd876874)
    

