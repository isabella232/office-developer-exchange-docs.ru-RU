---
title: Функция CChkSGFiles.Delete
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Delete
api_type:
- dllExport
ms.assetid: 869e927f-7df2-4247-88ef-b8b05b29a700
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: cf1c23dd75442d73dfea49e0831d0859da321a40
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510542"
---
# <a name="cchksgfilesdelete-function"></a>Функция CChkSGFiles.Delete

**Применяется к: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 г.
  
Уничтожает существующий экземпляр **класса CChkSGFiles.** Эту функцию необходимо вызвать после завершения работы приложения с указанным объектом. 
  
```cs
Static VOID __stdcall Delete 
(
        CCheckSGFiles  * pcchecksgfiles
);

```

## <a name="parameters"></a>Параметры

### <a name="pcchecksgfiles"></a>pcchecksgfiles 
  
Параметр входного ввода. Указатель на существующий **объект CCheckSGFiles.** После этого память, связанная с объектом, будет освобождена. 
    
## <a name="return-value"></a>Возвращаемое значение

Нет.
  
## <a name="remarks"></a>Заметки

Функция **Delete** освободит память, связанную с **объектом CCheckSGFiles.** После вызова **Delete** указатель, переданный в  *параметре pcchecksgfiles,*  будет недействительным, и никакие другие операции не могут выполняться на этом объекте. 
  
Если приложение использует функцию **ErrCheckDbPages,** приложение должно освободить буфер памяти вручную; Функция **Delete** не освободит ее. 
  
Если вы используете CHKSGFILES в многопотоковом приложении, необходимо вызвать функцию **Удаление** в однопотной части приложения, и вы можете вызвать ее только один раз для каждого объекта **CCheckSGFiles.** 
  
## <a name="requirements"></a>Requirements

Exchange 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой работает приложение, должна иметь разрешения на доступ к базе данных и файлы журналов, которые необходимо проверить.
  

