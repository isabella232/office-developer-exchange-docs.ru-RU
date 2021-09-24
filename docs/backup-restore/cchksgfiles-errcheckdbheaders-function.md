---
title: Функция CChkSGFiles.ErrCheckDbHeaders
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: 215a0d1126fce48b7e3800016619b0c52915312b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510472"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>Функция CChkSGFiles.ErrCheckDbHeaders

**Применяется к: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 г. 
  
Проверяет заглавные главы файлов баз данных, указанных функцией **ErrInit.** Эта функция также возвращает размер страницы и количество страниц в каждой из указанных баз данных. 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Параметры

### <a name="pcbdbpagesize"></a>pcbDbPageSize 
  
Параметр вывода. Размер страницы каждой из указанных баз данных в bytes.
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
Параметр вывода. Количество страниц в начале каждой указанной базы данных, зарезервированных механизмом базы данных для внутреннего использования. Обратите внимание, *что для* проверки не следует передавать страницы заглавных страниц в функцию **ErrCheckDbPages.** 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
Параметр вывода. Если возвращаемая величина функции указывает на ошибку, этот параметр будет индексом в **массиве rgwszDb[]** переданной функции **ErrInit.** Элемент индексирования массива представляет базу данных, в которой произошла ошибка. Если функция не возвращает значение ошибки, это значение параметра является недействительным. 
    
### <a name="ulflags"></a>ulFlags 
  
Необязательный параметр ввода. Это значение зарезервировано для использования в будущем. Пройдено значение должно быть 0 (ноль).
    
## <a name="return-value"></a>Возвращаемое значение

Эта функция возвращает код ошибки из переумерия [CChkSGFiles.ERR.](cchksgfiles-err-enumeration.md)
  
## <a name="remarks"></a>Заметки

**ErrCheckDbHeaders** проверяет, что все базы данных, зарегистрированные **в ErrInit,** имеют одинаковый размер подписи журнала и страницы базы данных. Для определения набора файлов журналов, необходимых для приведения всех зарегистрированных баз данных в состояние очистки, можно также использовать самое низкое значение параметров **genMin** и самое высокое значение параметра **genMax.** 
  
Параметр **piDbErrorEncountered** устанавливается только при обнаружении ошибки, как указывает значение возврата **ненулевых ErrCheckDbHeaders.** 
  
При ошибке в этой функции событие ошибки будет добавлено в журнал событий Windows ошибки.
  
Вызвать **ErrCheckDbHeaders** можно только после вызова **ErrInit,** и перед вызовом **ErrCheckDbPages** и **ErrCheckLogs.**
  
Если вы используете CHKSGFILES в многопотоковом приложении, необходимо вызвать функцию **ErrCheckDbHeaders** в однопотокой части и вызвать ее можно только один раз для каждого объекта **CCheckSGFiles.** 
  
## <a name="requirements"></a>Requirements

Exchange 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой работает приложение, должна иметь разрешения на доступ к базе данных и файлы журналов, которые необходимо проверить.
  

