---
title: Функция CChkSGFiles.Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: 5c41007a797e5a256692b2c4bdcb3cfae82c12ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760920"
---
# <a name="cchksgfilesdelete-function"></a>Функция CChkSGFiles.Delete

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Удаляет существующий экземпляр класса **CChkSGFiles** . После завершения работы с указанным объектом приложения, необходимо вызвать эту функцию. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Parameters

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
Входного параметра. Указатель на существующий объект **CCheckSGFiles** . Затем освободится память, связанную с объектом. 
    
## <a name="return-value"></a>Возвращаемое значение

Нет.
  
## <a name="remarks"></a>Замечания

Функция **Удаление** освобождает память, связанного с объектом **CCheckSGFiles** . После вызова **Удаление**указателя мыши, переданной в параметре *pcchecksgfiles* будет недопустимый и никакие другие операции, которые могут выполняться для этого объекта. 
  
Если приложение использует функцию **ErrCheckDbPages** , приложение должно освободить буфер памяти вручную; **Удаление** функции не освобождает его. 
  
Если вы используете многопоточного приложения CHKSGFILES, необходимо вызвать функцию **Удалить** в одном потоке часть приложения и его можно вызвать только один раз для каждого объекта **CCheckSGFiles** . 
  
## <a name="requirements"></a>Требования

Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.
  
Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.
  

