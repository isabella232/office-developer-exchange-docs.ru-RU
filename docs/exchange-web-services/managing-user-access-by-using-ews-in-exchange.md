---
title: Управление доступом пользователей с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 48f0170c-8786-405f-86cb-568b7314a425
description: Узнайте, какие существуют возможности для управления доступом к учетной записи пользователя с сервером Exchange.
ms.openlocfilehash: d93f521f08f93b44b4ecc1f258b03ed24ebdd3dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761147"
---
# <a name="managing-user-access-by-using-ews-in-exchange"></a>Управление доступом пользователей с помощью веб-служб Exchange в Exchange

Узнайте, какие существуют возможности для управления доступом к учетной записи пользователя с сервером Exchange.
  
Веб-служб Exchange (EWS) и веб-служб Exchange с управляемым API предоставляют ограниченное количество операций, которые можно использовать для управления учетными записями в Exchange Online, Exchange Online в составе Office 365 или версии Exchange, начиная с Exchange 2013. Управление представителями и задавать права доступа к папкам для других учетных записей можно использовать операции, показано на следующем рисунке. 
  
**Операции веб-служб Exchange для доступа делегата и папки**

![Параметры управления пользователями EWS.](media/Exchange_ManagingUserAccess_1.png)
  
Если приложению дополнительные контроль учетных записей на сервере Exchange, можно использовать командлеты командной консоли Exchange к управлению учетными записями. Можно вызвать командлетов командной консоли Exchange, выполнив одно из следующих:
  
- Создание приложения с помощью C# или Visual Basic, который вызывает командлетов командной консоли Exchange. Можно просмотреть пример кода на [Документация по API -интерфейса командной консоли управления Exchange](../management/exchange-management-shell.md) , чтобы узнать, как для вызова командлета. 
    
- С помощью Windows PowerShell и сценарии Windows PowerShell для вызова командлетов командной консоли Exchange. Можно найти полный список [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps), а также примеры, показывающие, как их использовать. 
    
## <a name="see-also"></a>См. также

- [Настройка приложения веб-служб Exchange](setting-up-your-ews-application.md)   
- [Командлеты Exchange 2013](https://docs.microsoft.com/en-us/powershell/exchange/?view=exchange-ps)  
    

