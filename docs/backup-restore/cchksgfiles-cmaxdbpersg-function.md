---
title: Функция функция cchksgfiles. Кмаксдбперсг
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Дата последнего изменения: 22 февраля 2013 г.'
ms.openlocfilehash: b7c3517779eb07ef053c1dd4fa25544310fb3343
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455263"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Функция функция cchksgfiles. Кмаксдбперсг

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Возвращает максимально допустимое число баз данных в одной группе хранения Exchange Server.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Параметры

Нет.
  
## <a name="return-value"></a>Возвращаемое значение

Максимальное число баз данных, разрешенных указанным сервером Exchange для каждой группы хранения. Так как группы хранения не входят в состав Exchange 2013, эта функция возвращает 1.
  
## <a name="remarks"></a>Примечания

Объект **кчекксгфилес** можно использовать для проверки баз данных (и файлов журнала транзакций) только в одной группе хранения, поэтому значение, возвращаемое функцией **кмаксдбперсг** , также представляет максимальное число баз данных, которые можно проверить с помощью экземпляра класса **кчекксгфилес** . 
  
Обратите внимание, что по умолчанию Exchange Server 2003 и Exchange Server 2007 допускают не более пяти баз данных на каждую группу хранения.
  
## <a name="requirements"></a>Requirements

Exchange 2013 включает только 64-разрядную версию API ЧКСГФИЛЕС.
  
Учетная запись, под которой выполняется приложение, должна иметь разрешения на чтение для базы данных и файлов журнала, которые необходимо проверить.
  

