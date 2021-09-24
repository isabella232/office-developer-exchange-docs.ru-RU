---
title: Функция CChkSGFiles.ErrInit
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ErrInit
api_type:
- dllExport
ms.assetid: 61bb3af1-8b51-4bae-8e25-90a4dc1226c5
description: 'Последнее изменение: 03 марта 2013 г.'
ms.openlocfilehash: ccb5293e35f20328181c4cf1cb5f0eddbb42e03f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516295"
---
# <a name="cchksgfileserrinit-function"></a>Функция CChkSGFiles.ErrInit
  
**Применяется к: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 г.
  
Инициализирует объект **CChkSGFiles,** указав проверяемую базу данных и путь и базовое имя файлов журнала транзакций. Приложения должны вызывать эту функцию сразу после успешного вызова **новой** функции. 
  
```cs
Vitual ERRErrInit  
(
    Const WCHAR  * const rgwszDb[],
    Const ULONGcDB,
    __in_z const WCHAR  * const wszLogPath,
    __in_z const WCHAR  * const wszBaseName,
    Const ULONGulFlags = NO_FLAGS
);

```

## <a name="parameters"></a>Параметры

### <a name="rgwszdb"></a>rgwszDb[]
  
Параметр входного ввода. Массив, который указывает проверяемую базу данных. Каждый элемент массива — это строка единого кода, которая содержит путь и имя файла базы данных, которые необходимо проверить.
    
### <a name="cdb"></a>cDB
  
Параметр входного ввода. Количество допустимого элемента пути базы данных в **массиве rgwszDb.** 
    
#### <a name="wszlogpath"></a>wszLogPath
  
Параметр входного ввода. Полный путь проверяемого файла журнала транзакций в виде строки Юникод с null-terminated.
    
### <a name="wszbasename"></a>wszBaseName
  
Параметр входного ввода. Базовая трех буква файлов журнала Exchange транзакций в виде строки Юникод с null-terminated.
    
### <a name="ulflags"></a>ulFlags
  
Необязательный параметр ввода. Это значение зарезервировано для использования в будущем. Значение, пройденного этим параметром, должно быть 0 (ноль).
    
## <a name="return-value"></a>Возвращаемое значение

Код ошибки из переумерия [ERR.](cchksgfiles-err-enumeration.md) 
  
## <a name="remarks"></a>Заметки

Функция **ErrInit** регистрирует базы данных и файлы журналов, которые необходимо проверить. Эта функция должна быть вызвана после того, как **вызвана** новая функция, но перед тем, как будет вызвана любая другая функция **ChkSGFiles.** 
  
Необходимо предоставить все имена баз данных, путь файла журнала и базовое имя в качестве null-terminated строк Юникод.
  
Вы можете проверять только файлы базы данных, только файлы журналов или как базы данных, так и файлы журналов. Однако при вызове этой функции приложение должно указать по крайней мере одну сущность, которая должна быть проверена. Передача 0 (ноль) для  **cDB**  и NULL для  **wszLogPath**  возвращает ошибку. 
  
Если значение  **cDB**  не превышает 0 (ноль), передача NULL для  **rgwszDb**  приведет к ошибке. Чтобы проверить файлы баз данных, приложение должно предоставить имена баз данных. 
  
Если NULL передается  **для wszBaseName,**  но  **wszLogPath**  не является NULL, ошибка возвращается. При проверке файлов журнала всегда требуется базовое имя файла журнала. 
  
Если вы используете CHKSGFILES в многопотоковом приложении, необходимо вызвать функцию **ErrInit** в однопотокой части приложения и вызвать ее можно только один раз для каждого объекта **CCheckSGFiles.** 
  
## <a name="requirements"></a>Requirements

Exchange 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой работает приложение, должна иметь разрешения на доступ к базе данных и файлы журналов, которые необходимо проверить.
  

