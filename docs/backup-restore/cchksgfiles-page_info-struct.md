---
title: Структура CChkSGFiles.PAGE_INFO
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: f324ec9aca6f94911041c227ce039139292a10aa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516260"
---
# <a name="cchksgfilespage_info-struct"></a>Структура CChkSGFiles.PAGE_INFO

**Применяется к: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 г.
  
Содержит сведения для Exchange базы данных. Эта структура используется с функцией **ErrCheckDbPages.** 
  
```cs
Struct PAGE_INFO  
{
        ULONGulPgno;
        BOOLfPageIsInitialized : 1;
        BOOLfCorrectableError : 1;
        ULONGLONGchecksumActual;
        ULONGLONGchecksumExpected;
        ULONGLONGdbTime;
        ULONGLONGchecksumPageStructure;
        ULONGLONGulFlags;
}

```

## <a name="members"></a>Members

### <a name="ulpgno"></a>ulPgNo
  
Unsigned Long. Логический номер страницы страницы базы данных, которая должна быть проверена. Это значение необходимо установить перед вызовом **ErrCheckDbPages.** Если приложение читает файл на основе смещений файлов и поэтому должно соотносить эти смещения с логическими номерами страниц, вы найдете метод **PgnoFromFileOffset** полезным для определения значения для этого поля. **ErrCheckDbPages** не изменит это значение. 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
Boolean. Значение TRUE указывает, что страница базы данных содержит данные. Значение FALSE указывает, что страница содержит только нули. **ErrCheckDbPages** задает это значение. 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
Boolean. Значение TRUE указывает на то, что на странице базы данных обнаружено несоответствие проверки, но это исправленная ошибка. **ErrCheckDbPages** задает это значение. 
    
### <a name="checksumactual"></a>checksumActual
  
Unsigned 64-bit integer. Указывает значение checksum, хранимые в базе данных для этой логической страницы. **ErrCheckDbPages** задает это значение. 
    
### <a name="checksumexpected"></a>checksumExpected
  
Unsigned 64-bit integer. Это ожидаемое значение checksum, рассчитанное для страницы базы данных; она устанавливается **ErrCheckDbPages**. Если это значение отличается от значения, хранимого на странице базы данных (т. е. возвращаемого в **checksumActual),** **ErrCheckDbPages** указывает, что на этой странице базы данных обнаружена ошибка. 
    
### <a name="dbtime"></a>dbTime
  
Unsigned 64-bit integer. **ErrCheckDbPages** задает этому члену время на странице базы данных. 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Незаверяемая 64-bt-integer. **ErrCheckDbPages** задает этому члену рассчитанное значение checksum содержимого страницы, исключая данные, которые не нужны при определении логической эквивалентности страницы. Например, нет необходимости рассматривать значения данных в неиспользованом пространстве страниц базы данных. Этот член действителен только в том случае, если **значения checksumActual**  и  **checksumExpected**  равны друг другу. 
    
### <a name="ulflags"></a>ulFlags
  
Unsigned 64-bit integer. Зарезервировано для последующего использования. Перед вызовом **ErrCheckDbPages** значение этого поля должно быть установлено до 0 (ноль).
    
## <a name="remarks"></a>Заметки

При вызове **функции ErrCheckDbPages** параметр **rgPageInfo** — это массив структур **PAGE \_ INFO.** Для каждой страницы базы данных должна быть одна структура PAGE **\_ INFO.** 
  
Приложение должно задать **члену ulPgno**  соответствующее значение, а также задать  **члену ulFlags**  значение 0 (ноль) перед вызовом **ErrCheckDbPages**. 
  
## <a name="requirements"></a>Requirements

Exchange Server 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой работает приложение, должна иметь разрешения на доступ к базе данных и файлы журналов, которые необходимо проверить.
  

