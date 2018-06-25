---
title: Функция CChkSGFiles.PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: d42ba7c8178c6fccdddec0b5da88a972f51184c6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760927"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>Функция CChkSGFiles.PgnoFromFileOffset

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Возвращает номер страницы в логической базы данных, соответствующий индекса указанного байта в файле физической базы данных. Если смещение файла является недопустимым или функция **ErrCheckDbHeaders** не был вызван для баз данных, эта функция возвращает нуль (0). 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Parameters

### <a name="ibfileoffset"></a>ibFileOffset
  
Входного параметра. Смещение в файле базы данных, в байтах.
    
## <a name="return-value"></a>������������ ��������

Номер логической страницы файла базы данных, которая включает в себя указанное смещение.
  
## <a name="remarks"></a>Замечания

Если параметр **ibFileOffset** является недопустимым, функция **PgnoFromFileOffset** возвращает нуль (0). 
  
Если еще не вызов функции **ErrCheckDbHeaders** в экземпляре **CCheckSGFiles** **PgnoFromFileOffset** также возвращает нуль (0). Необходимо вызвать **ErrCheckDbHeaders** для инициализации размер страницы базы данных и число страниц, выделенных заголовков базы данных. 
  
**PgnoFromFileOffset** следует использовать для заполнения **Страница\_INFO** структура элементов при подготовке вызов **ErrCheckDbPages**. Параметр **rgPageInfo** для **ErrCheckDbPages** требуется каждого элемента в массиве структуру **PAGE_INFO** значениями членов **ulPgno** правильно инициализировать. 
  
Если вы используете многопоточного приложения CHKSGFILES, можно вызвать функцию **PgnoFromFileOffset** в многопоточные части приложения. Обратите внимание на то, что обычно вызов этой функции несколько раз для каждой базы данных проверки. 
  
## <a name="requirements"></a>Требования

Exchange Server 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.
  
Учетная запись, приложения в разделе должен иметь разрешение на чтение базы данных и журналов файлов, которые должны быть возвращены.
  

