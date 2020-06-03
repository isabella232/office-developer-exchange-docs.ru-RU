---
title: Управление доступом пользователей с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Узнайте, какие параметры предназначены для управления доступом учетной записи пользователя к серверу Exchange.
ms.openlocfilehash: 476292d4db206f22cd84134ce2b46957e9fe85fc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456247"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Управление доступом пользователей с помощью EWS в Exchange

Узнайте, какие параметры предназначены для управления доступом учетной записи пользователя к серверу Exchange.
  
Веб-службы Exchange (EWS) и управляемый API EWS предоставляют ограниченное количество операций, которые можно использовать для управления учетными записями в Exchange Online, Exchange Online в составе Office 365 или версии Exchange, начиная с Exchange 2013. Вы можете использовать операции, показанные на следующем рисунке, для управления представителями и для задания разрешений на доступ к папкам для других учетных записей. 
  
**Операции EWS для делегирования и доступа к папкам**

![Параметры управления пользователями EWS.](media/Exchange_ManagingUserAccess_1.png)
  
Если приложению требуется дополнительный контроль над учетными записями на сервере Exchange Server, можно использовать командлеты командной консоли Exchange для управления учетными записями. Чтобы вызвать командлеты командной консоли Exchange, выполните одно из следующих действий.
  
- Написание приложения с помощью C# или Visual Basic, которое вызывает командлеты командной консоли Exchange. Чтобы узнать, как вызвать командлет, можно просмотреть пример кода в [документации по API командной консоли Exchange](../management/exchange-management-shell.md) . 
    
- Использование сценариев Windows PowerShell и Windows PowerShell для вызова командлетов командной консоли Exchange. Можно найти полный список [PowerShell для Exchange Server (Командная консоль Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), а также примеры, демонстрирующие их использование. 
    
## <a name="see-also"></a>См. также

- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)   
- [Командлеты Exchange 2013](https://docs.microsoft.com/powershell/exchange/?view=exchange-ps)  
    

