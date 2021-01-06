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
description: 'Last modified: February 22, 2013'
ms.openlocfilehash: 3c8f749a03b4aa251bf9312eba5d7e2d46c91fae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44452897"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>Функция CChkSGFiles.PgnoFromFileOffset

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Возвращает номер страницы логической базы данных, соответствующий указанному индексу в физическом файле базы данных. Если смещение файла недопустимо или функция **ErrCheckDbHeaders** не была вызвана для баз данных, эта функция возвращает 0 (ноль). 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Параметры

### <a name="ibfileoffset"></a>ibFileOffset
  
Входной параметр. Смещение в файл базы данных в ветвях.
    
## <a name="return-value"></a>Возвращаемое значение

Логический номер страницы файла базы данных, который включает указанное смещение.
  
## <a name="remarks"></a>Примечания

Если параметр **ibFileOffset** недействителен, функция **PgnoFromFileOffset** возвращает значение 0 (ноль). 
  
**PgnoFromFileOffset** также возвращает 0 (ноль), если вы не вызвали функцию **ErrCheckDbHeaders** в экземпляре **CCheckSGFiles.** Необходимо вызвать **ErrCheckDbHeaders,** чтобы инициализировать размер страницы базы данных и количество страниц, выделенных для headers базы данных. 
  
**PgnoFromFileOffset** следует использовать для заполнения элементов структуры **PAGE \_ INFO** при подготовке к вызову **ErrCheckDbPages.** Параметр **rgPageInfo** для **ErrCheckDbPages** требует, чтобы каждый  элемент в массиве был PAGE_INFO структурой с правильно инициализированными значениями членов **ulPgno.** 
  
Если вы используете CHKSGFILES в многопрочитаном приложении, вы можете вызвать функцию **PgnoFromFileOffset** в многопрочитаной части приложения. Обратите внимание, что обычно эта функция вызывалась несколько раз для каждой проверяемой базы данных. 
  
## <a name="requirements"></a>Требования

Exchange Server 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой запущено приложение, должна иметь разрешение на чтение базы данных и файлов журналов, которые необходимо проверить.
  

