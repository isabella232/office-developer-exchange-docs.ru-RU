---
title: Перечисление CChkSGFiles.ERR
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: '���� ���������� ���������: 9 ����� 2015 �.'
ms.openlocfilehash: 20f10c43e3b92604bb51e1aa5f896a8bd7c4b335
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761865"
---
# <a name="cchksgfileserr-enumeration"></a>Перечисление CChkSGFiles.ERR 
  
**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Указывает результаты вызываемой функции. Это перечисление возвращается множество функций класса **CCheckSGFiles** . 
  
```cs
Enum ERR  
{
        errSuccess = 0,
        errTaskDropped = -106,
        errRequiredLogFilesMissing = -543,
        errInvalidParameter = -1003,
        errOutOfMemory = -1011,
        errReadVerifyFailure = -1018,
        errTooManyActiveUsers = -1059,
        errDatabaseCorrupted = -1206
}

```

## <a name="values"></a>Значения

|**Имя элемента**|**Значение**|**Описание**|
|:-----|:-----|:-----|
|errSuccess  <br/> |0  <br/> |Функция завершена без ошибок.  <br/> |
|errTaskDropped  <br/> |-106  <br/> |Возвращаемый функцией **ErrTerm** для указания были возвращены, что не все страницы базы данных и файлы журнала транзакций или, что при проверке были обнаружены ошибки.  <br/> |
|errRequiredLogFilesMissing  <br/> |-543  <br/> |Один или несколько файлов журнала, которые необходимы для базы данных в состояние чистого отключения не найден в путь к файлу журнала или не имеет указанного базового имени трех букв.  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |Неправильных один или несколько параметров, которые были переданы в функцию.  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |Недостаточно памяти была доступна для выполнения запрошенной операции.  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |Контрольная сумма, которая хранится на странице базы данных не соответствует ожидаемой контрольной сумме.  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |Функция **ErrTerm** вызван при работе с объектом был по-прежнему. Это может произойти, если **ErrTerm** вызывается до **ErrCheckDbPages** или вернул **ErrCheckLogFiles** .  <br/> |
   
## <a name="requirements"></a>Требования

Exchange Server 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.
  
Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.
  

