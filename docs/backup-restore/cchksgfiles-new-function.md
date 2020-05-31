---
title: Функция функция cchksgfiles. New
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
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: b40f8b1a95477715b29defb4addabfb333e92d04
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760914"
---
# <a name="cchksgfilesnew-function"></a>Функция функция cchksgfiles. New

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Создает новый экземпляр класса **функция cchksgfiles** . Эту функцию необходимо вызвать, прежде чем можно будет указать группу хранения и базы данных для проверки. 
  
```cs
Static CCheckSGFiles  * __stdcall New  ();

```

## <a name="parameters"></a>Параметры

Нет.
  
## <a name="return-value"></a>Возвращаемое значение

Ссылка (указатель) на только что созданный объект.
  
## <a name="remarks"></a>Примечания

**Новая** функция создает объект **кчекксгфилес** и возвращает в вызывающий объект ссылку (указатель) на этот объект. Эту функцию необходимо вызвать перед вызовом любой из других функций в классе **кчекксгфилес** . 
  
Если вы используете ЧКСГФИЛЕС в многопоточном приложении, необходимо вызвать функцию **New** в однопотоковой части приложения, и вы можете вызвать его только один раз для каждого объекта **кчекксгфилес** . 
  
## <a name="requirements"></a>Requirements

Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.
  
Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.
  

