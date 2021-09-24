---
title: Перечисление CChkSGFiles.ERR
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ERR
api_type:
- dllExport
ms.assetid: f0efe195-91c3-4f3a-8c7d-e5dba336465a
description: 'Дата последнего изменения: 9 марта 2015 г.'
ms.openlocfilehash: 12cfff44a6dacbb07ee5518d0008092fbfb644d1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510465"
---
# <a name="cchksgfileserr-enumeration"></a>Перечисление CChkSGFiles.ERR 
  
**Применяется к: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 г.
  
Указывает результаты называемой функции. Это переумежение возвращается многими функциями **класса CCheckSGFiles.** 
  
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
|errSuccess  <br/> |0  <br/> |Функция выполнена без ошибок.  <br/> |
|errTaskDropped  <br/> |-106  <br/> |Возвращено функцией **ErrTerm,** чтобы указать, что не все страницы баз данных и файлы журналов транзакций были проверены или что во время проверки были допущены ошибки.  <br/> |
|errRequiredLogFilesMissing  <br/> |-543  <br/> |Один или несколько файлов журнала, необходимых для приведения базы данных в состояние очистки, не найдены в пути файла журнала или не имеют указанного базового имени из трех букв.  <br/> |
|errInvalidParameter  <br/> |-1003  <br/> |Один или несколько параметров, переданных функции, были недействительными.  <br/> |
|errOutOfMemory  <br/> |-1011  <br/> |Для выполнения запрашиваемой операции была недостаточна память.  <br/> |
|errReadVerifyFailure  <br/> |-1018  <br/> |Контрольный лист, хранимый на странице базы данных, не соответствует ожидаемому.  <br/> |
|errTooManyActiveUsers  <br/> |-1059  <br/> |Функция **ErrTerm** была вызвана во время использования объекта. Это может произойти, если **ErrTerm вызван** до возвращения **ErrCheckDbPages** или **ErrCheckLogFiles.**  <br/> |
   
## <a name="requirements"></a>Requirements

Exchange Server 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой работает приложение, должна иметь разрешения на доступ к базе данных и файлы журналов, которые необходимо проверить.
  

