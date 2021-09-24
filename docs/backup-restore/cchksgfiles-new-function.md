---
title: Функция CChkSGFiles.New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: e50b41e761b8e46d778011b6bac3db4dbb624809
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516274"
---
# <a name="cchksgfilesnew-function"></a>Функция CChkSGFiles.New

**Применяется к: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 г.
  
Создает новый экземпляр класса **CChkSGFiles.** Необходимо вызвать эту функцию, прежде чем указать группу хранения и базы данных, которые необходимо проверить. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Параметры

Нет.
  
## <a name="return-value"></a>Возвращаемое значение

Ссылка (указатель) на вновь созданный объект.
  
## <a name="remarks"></a>Заметки

Новая **функция** создает объект **CCheckSGFiles** и возвращает звоняшему ссылку (указатель) на этот объект. Необходимо вызвать эту функцию, прежде чем она вызывает любые другие функции в **классе CCheckSGFiles.** 
  
Если вы используете CHKSGFILES в многопотоковом приложении, необходимо вызвать функцию **New** в однопотной части приложения, и вы можете вызвать ее только один раз для каждого объекта **CCheckSGFiles.** 
  
## <a name="requirements"></a>Requirements

Exchange 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой работает приложение, должна иметь разрешения на доступ к базе данных и файлы журналов, которые необходимо проверить.
  

