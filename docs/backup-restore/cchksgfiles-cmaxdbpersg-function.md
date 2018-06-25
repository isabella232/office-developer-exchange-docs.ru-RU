---
title: Функция CChkSGFiles.CMaxDbPerSG
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
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: bf09074bab6dee13e97e8a59a22ae1b19522a5e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761882"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Функция CChkSGFiles.CMaxDbPerSG

**Применимо к:** Exchange Server 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013
  
Возвращает максимальное количество баз данных, допустимых в одну группу хранилища сервера Exchange.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Параметры

Нет.
  
## <a name="return-value"></a>Возвращаемое значение

Максимальное число баз данных, указанный сервер Exchange позволяет группам хранилищ. Так как группы хранения не являющихся частью Exchange 2013, эта функция возвращает 1.
  
## <a name="remarks"></a>Замечания

Объект **CCheckSGFiles** можно использовать для проверки баз данных (и файлы журнала транзакций) в только одна группа хранения, поэтому значение, возвращаемое функцией **CMaxDbPerSG** также представляет максимальное число баз данных, которые можно проверить с помощью экземпляр класса **CCheckSGFiles** . 
  
Обратите внимание, что по умолчанию Exchange Server 2003 и Exchange Server 2007 позволяет не более пяти баз данных в группе хранения.
  
## <a name="requirements"></a>Требования

Exchange 2013 включает в себя только 64-разрядная версия CHKSGFILES API-интерфейса.
  
Учетная запись, приложения в разделе необходимо иметь разрешения доступ на чтение для файлов базы данных и журналов, которые требуется проверить.
  

