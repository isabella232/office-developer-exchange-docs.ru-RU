---
title: Функция CChkSGFiles.ErrCheckDbHeaders
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ErrCheckDbHeaders
api_type:
- dllExport
ms.assetid: 75289cd2-35b1-4f75-a651-dce01f1ddda1
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: a407019063b34970e883a00ca4f4d730935d7cba
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760926"
---
# <a name="cchksgfileserrcheckdbheaders-function"></a>Функция CChkSGFiles.ErrCheckDbHeaders

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 
  
Проверяет заголовки файлов базы данных, которые были указаны с помощью функции **ErrInit** . Эта функция также возвращает размер страницы и число страниц в каждой указанной базы данных. 
  
```cs
Vitual ERRErrCheckDbHeaders  
(
        ULONG  * const pcbDbPageSize,
        ULONG  * const pcHeaderPagesPerDb,
        ULONG   const piDbErrorEncountered,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Parameters

### <a name="pcbdbpagesize"></a>pcbDbPageSize 
  
Выходной параметр. Размер страницы каждой указанной базы данных, в байтах.
    
### <a name="pcheaderpagesperdb"></a>pcHeaderPagesPerDb 
  
Выходной параметр. Число страниц в начале каждой указанной базы данных, зарезервированные ядро базы данных для внутреннего использования. Обратите внимание, что вы должны *прохода страницы заголовка в функцию **ErrCheckDbPages** для проверки* . 
    
### <a name="pidberrorencountered"></a>piDbErrorEncountered
  
Выходной параметр. Если возвращаемое значение функции, указывающий на ошибки, данный параметр будет индекса в массив **rgwszDb []** , переданное в функцию **ErrInit** . Индексированный элемент массива представляет базу данных, в котором возникла ошибка. Если функция не возвращает ошибку, значение этого параметра является недопустимым. 
    
### <a name="ulflags"></a>ulFlags 
  
Необязательный параметр ввода. Это значение зарезервировано для будущего использования. Значение, переданное должны быть нуль (0).
    
## <a name="return-value"></a>������������ ��������

Эта функция возвращает код ошибки из [перечисления CChkSGFiles.ERR](cchksgfiles-err-enumeration.md).
  
## <a name="remarks"></a>Замечания

**ErrCheckDbHeaders** проверяет, что все базы данных, зарегистрированные с **ErrInit** же журнала подписи и база данных размер страницы. Минимальное значение параметра **genMin** и наибольшее значение параметра **genMax** также можно использовать для определения набора файлов журнала, которые необходимо установить все зарегистрированные базы данных в состояние чистого отключения. 
  
Параметр **piDbErrorEncountered** имеет значение только в том случае, если обнаружена ошибка, как указано в отличное от нуля **ErrCheckDbHeaders** возвращаемое значение. 
  
При возникновении ошибки в этой функции, событие ошибки будут добавлены в журнал событий Windows ошибки.
  
Можно вызвать **ErrCheckDbHeaders** только после вызова **ErrInit**и его необходимо вызвать до вызова метода **ErrCheckDbPages** и **ErrCheckLogs**.
  
Если вы используете многопоточного приложения CHKSGFILES, необходимо вызвать функцию **ErrCheckDbHeaders** в части одного потока, и его можно вызвать только один раз для каждого объекта **CCheckSGFiles** . 
  
## <a name="requirements"></a>Требования

Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.
  
Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.
  

