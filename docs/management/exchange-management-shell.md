---
title: Командная консоль Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Найдите сведения о том, как использовать консоль управления Exchange для разработки средств для администрирования Exchange server.
ms.openlocfilehash: 1cb0328bdb0eebda0ce4eda929e1bfb21be451f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761254"
---
# <a name="exchange-management-shell"></a>Командная консоль Exchange

Найдите сведения о том, как использовать консоль управления Exchange для разработки средств для администрирования Exchange server.
  
**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365
  
Командная консоль Exchange предоставляет набор команд, вычисленное на платформе Windows PowerShell для управления Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange 2013. Можно использовать консоль управления Exchange для создания два типа средств: сценарии командной строки, которые работают в среде Windows PowerShell и средства, с помощью командлетов командной консоли Exchange через управляемый интерфейс. Управляемых приложений можно использовать для создания стандартных Windows или веб-Интерфейс для администрирования сервера Exchange. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Что нужно знать о командной консоли Exchange

|Если вам интересно о|Прочтите это|
|:-----|:-----|
|Availability  <br/> |Команды командной консоли Exchange установлены на всех серверах с версии Exchange, начиная с Exchange 2007.<br/>Клиентские приложения можно развернуть на любом компьютере под управлением Windows PowerShell 2.0.<br/> Сведения о доступе к командной консоли [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)см.  <br/> |
|Languages and tools  <br/> |Командная консоль Exchange сценарии можно создать в любом текстовом редакторе.<br/>Можно использовать один из многих средств сторонних производителей для создания скриптов Windows PowerShell, которые могут использоваться с командной консолью Exchange.  <br/> [Командная консоль Exchange объектной модели](exchange-management-shell-namespaces.md) основано на .NET Framework.<br/>Можно использовать любой язык .NET для разработки приложений Командная консоль Exchange.  <br/> |
|Доступные инструменты для тестирования и отладки  <br/> |Тестирование и отладка скриптов Командная консоль Exchange, можно использовать один из многих приложений сторонних производителей.  <br/> Можно использовать Visual Studio и средств сторонних производителей для тестирования и отладки управляемых приложений Командная консоль Exchange.  <br/> |
|Server platform requirements  <br/> |Можно использовать консоль управления Exchange на любом сервере Exchange с Windows PowerShell 2.0 установлены.  <br/> |
|Client platform requirements  <br/> |Командная консоль Exchange клиентских приложений требуется Windows PowerShell 2.0.  <br/> |
|Разрешения  <br/> |Для выполнения Командная консоль Exchange приложения необходимо, чтобы пользователь имел права управления доступом на основе ролей на затронутых данных в хранилище Exchange.<br/>Дополнительные сведения об управлении доступом на основе ролей [Управления доступом на основе ролей общее представление о](http://technet.microsoft.com/en-us/library/dd298183.aspx)см.  <br/> |
   
В статьях в данном разделе описываются функции Командная консоль Exchange, которые важны для создания средства управления Exchange. Сведения о планирования, настройке и обслуживанию Exchange посетите веб-узел [Exchange](https://docs.microsoft.com/en-us/exchange/) .
  
## <a name="in-this-section"></a>В этом разделе

- [Создание средств управления Exchange](create-exchange-management-shell-tools.md)
    
- [Пространства имен Командная консоль Exchange](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>См. также
  
- [Документация по Windows PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Создание сценариев PowerShell](https://docs.microsoft.com/en-us/powershell/scripting/powershell-scripting?view=powershell-6)
    

