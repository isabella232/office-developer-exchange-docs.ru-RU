---
title: Функция CChkSGFiles.New
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- New
api_type:
- dllExport
ms.assetid: 588d8c74-c9ce-4d5e-8a79-a2a68676e858
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: b40f8b1a95477715b29defb4addabfb333e92d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760914"
---
# <a name="cchksgfilesnew-function"></a>Функция CChkSGFiles.New

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Создает новый экземпляр класса **CChkSGFiles** . Перед можно указать группы хранения и базы данных для проверки, необходимо вызвать эту функцию. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Параметры

Нет.
  
## <a name="return-value"></a>Возвращаемое значение

Ссылка (указатель) на только что созданный объект.
  
## <a name="remarks"></a>Замечания

Функция **New** создает объект **CCheckSGFiles** и возвращает вызывающему (указатель) ссылку на этот объект. Эта функция необходимо вызвать до вызова любой из других функций в классе **CCheckSGFiles** . 
  
Если вы используете многопоточного приложения CHKSGFILES, необходимо вызвать функцию **New** в одном потоке часть приложения и его можно вызвать только один раз для каждого объекта **CCheckSGFiles** . 
  
## <a name="requirements"></a>Требования

Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.
  
Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.
  

