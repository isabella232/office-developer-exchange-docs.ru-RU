---
title: Функция CChkSGFiles.CMaxDbPerSG
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CMaxDbPerSG
api_type:
- dllExport
ms.assetid: 5871988b-a5d7-42cc-9b83-8fededb5072f
description: 'Последнее изменение: 22 февраля 2013 г.'
ms.openlocfilehash: 1a82e71afde4766734d0875f68d7932a9fd9f26a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510527"
---
# <a name="cchksgfilescmaxdbpersg-function"></a>Функция CChkSGFiles.CMaxDbPerSG

**Применяется к: Exchange Server** 2003 | Exchange Server 2007 | Exchange Server 2010 | Exchange Server 2013 г.
  
Возвращает максимальное количество баз данных, разрешенных в одной группе Exchange серверов.
  
```cs
Static ULONG  __stdcall CMaxDbPerSG  ();

```

## <a name="parameters"></a>Параметры

Нет.
  
## <a name="return-value"></a>Возвращаемое значение

Максимальное количество баз данных, которые указанный Exchange позволяет для одной группы хранения. Поскольку группы хранения не являются частью Exchange 2013 г., эта функция возвращает 1.
  
## <a name="remarks"></a>Заметки

Объект **CCheckSGFiles** можно использовать для проверки баз данных (и файлов журналов транзакций) только в одной группе хранения, поэтому значение, возвращенное функцией **CMaxDbPerSG,** также представляет максимальное количество баз данных, которые можно проверить с помощью экземпляра класса **CCheckSGFiles.** 
  
Обратите внимание, что по умолчанию Exchange Server 2003 и Exchange Server 2007 года позволяют использовать не более пяти баз данных на одну группу хранения.
  
## <a name="requirements"></a>Requirements

Exchange 2013 включает только 64-битную версию API CHKSGFILES.
  
Учетная запись, в которой работает приложение, должна иметь разрешения на доступ к базе данных и файлы журналов, которые необходимо проверить.
  

