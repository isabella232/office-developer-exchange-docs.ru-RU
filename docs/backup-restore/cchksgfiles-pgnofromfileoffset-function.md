---
title: Функция CChkSGFiles.PgnoFromFileOffset
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PgnoFromFileOffset
api_type:
- dllExport
ms.assetid: 3d69ca6d-5ed1-4038-859e-106e776eeec1
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: 3e2845cc326520ad875dc8bda52bac3d7c2e2cfa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516246"
---
# <a name="cchksgfilespgnofromfileoffset-function"></a>Функция CChkSGFiles.PgnoFromFileOffset

**Применяется к: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 г.
  
Возвращает логический номер страницы базы данных, соответствующий указанному индексу byte в физическом файле базы данных. Если смещение файла является недействительным или если функция **ErrCheckDbHeaders** не была вызвана для баз данных, эта функция возвращает 0 (ноль). 
  
```cs
Vitual ULONGPgnoFromFileOffset  
(
    Const ULONGLONGibFileOffset
);

```

## <a name="parameters"></a>Параметры

### <a name="ibfileoffset"></a>ibFileOffset
  
Параметр входного ввода. Смещение в файл базы данных в bytes.
    
## <a name="return-value"></a>Возвращаемое значение

Логический номер страницы файла базы данных, который включает указанный смещение.
  
## <a name="remarks"></a>Заметки

Если параметр **ibFileOffset** недействителен, функция **PgnoFromFileOffset** возвращает 0 (ноль). 
  
**PgnoFromFileOffset** также возвращает 0 (ноль), если вы не вызвали функцию **ErrCheckDbHeaders** в экземпляре **CCheckSGFiles.** Чтобы инициализировать размер страницы базы данных и количество страниц, выделенных для заголовоков баз данных, необходимо вызвать **ErrCheckDbHeaders.** 
  
Для заполнения элементов структуры **PAGE \_ INFO** для подготовки к вызову **ErrCheckDbPages** необходимо использовать **PgnoFromFileOffset.** Параметр **rgPageInfo** для **ErrCheckDbPages** требует, чтобы каждый  элемент массива был структурой PAGE_INFO, при этом значения члена **ulPgno** были правильно инициализированы. 
  
Если вы используете CHKSGFILES в многоуровневом приложении, вы можете вызвать функцию **PgnoFromFileOffset** в многоуровневой части приложения. Обратите внимание, что эта функция обычно вызывалась несколько раз для каждой проверяемой базы данных. 
  
## <a name="requirements"></a>Requirements

Exchange Server 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой работает приложение, должна иметь разрешение на чтение в базу данных и файлы журналов, которые необходимо проверить.
  

