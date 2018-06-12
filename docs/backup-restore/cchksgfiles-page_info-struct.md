---
title: Структура CChkSGFiles.PAGE_INFO
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PAGE_INFO
api_type:
- dllExport
ms.assetid: 408335e1-6977-441f-bfad-ede791d1630c
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: fa66d253b4fc6bd5c29a39c5323f59bf323a906f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761859"
---
# <a name="cchksgfilespageinfo-struct"></a>Структура CChkSGFiles.PAGE_INFO

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Содержит сведения о странице базы данных Exchange. Эта структура используется с функцией **ErrCheckDbPages** . 
  
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

## <a name="members"></a>Элементы

### <a name="ulpgno"></a>ulPgNo
  
Длинное целое без знака. Число страниц базы данных для проверки логической страницы. Это значение должно быть задано до вызова метода **ErrCheckDbPages**. Если приложение читает файл на основании файла смещения и поэтому необходимо сопоставить смещения этих файлов логические номера страниц, вы найдете метод **PgnoFromFileOffset** полезен для определения значения для этого поля. **ErrCheckDbPages** не изменяет это значение. 
    
### <a name="fpageisinitialized"></a>fPageIsInitialized 
  
Логическое значение. Значение TRUE означает, что страница база данных содержит данные. Значение FALSE указывает, что страница содержит только нули. Это значение устанавливается **ErrCheckDbPages** . 
    
### <a name="fcorrectableerror"></a>fCorrectableError
  
Логическое значение. Значение TRUE указывает, что произошла ошибка контрольной суммы, обнаруженных в странице базы данных, но, что это Исправимая ошибка. Это значение устанавливается **ErrCheckDbPages** . 
    
### <a name="checksumactual"></a>checksumActual
  
Неподписанные 64-разрядное целое число. Указывает значение контрольной суммой, хранящиеся в базе данных для этой логической страницы. Это значение устанавливается **ErrCheckDbPages** . 
    
### <a name="checksumexpected"></a>checksumExpected
  
Неподписанные 64-разрядное целое число. Это значение ожидаемой, вычисленные для страницы базы данных; оно установлено по **ErrCheckDbPages**. Если это значение отличается от, хранящиеся на странице базы данных (то есть, значение, возвращаемое в **checksumActual**), **ErrCheckDbPages** появится сообщение о том, что на этой странице базы данных обнаружены ошибки. 
    
### <a name="dbtime"></a>dbTime
  
Неподписанные 64-разрядное целое число. **ErrCheckDbPages** устанавливает этот член метка времени на странице базы данных. 
    
### <a name="checksumpagestructure"></a>checksumPageStructure 
  
Целое 64-bt. **ErrCheckDbPages** задает этот член со значением вычисляемые содержимого страницы, за исключением данных, который не требуется, при определении эквивалентности логической страницы. Например нет необходимости необходимо рассмотреть значений данных в место неиспользуемых базы данных. Этот член допустимо только в том случае, если значения **checksumActual** и **checksumExpected** равны друг с другом. 
    
### <a name="ulflags"></a>ulFlags
  
Неподписанные 64-разрядное целое число. Зарезервировано для последующего использования. Значение в этом поле должно иметь значение нуль (0) до вызова метода **ErrCheckDbPages**.
    
## <a name="remarks"></a>Замечания

При вызове функции **ErrCheckDbPages** , параметр **rgPageInfo** представляет собой массив из **Страница\_INFO** структуры. Должно быть одно **Страница\_INFO** структуры для каждой страницы базы данных для проверки. 
  
Приложение необходимо присвоить член **ulPgno** правильное значение и необходимо также установить член **ulFlags** в нуль (0) до вызова метода **ErrCheckDbPages**. 
  
## <a name="requirements"></a>Требования

Exchange Server 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.
  
Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.
  

