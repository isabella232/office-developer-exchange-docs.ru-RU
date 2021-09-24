---
title: Командная консоль Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Сведения о том, как использовать Exchange для разработки средств администрирования Exchange сервера.
ms.openlocfilehash: ee1cbcb174c7153ca6cd9bb089580b372bf9029b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516155"
---
# <a name="exchange-management-shell"></a>Командная консоль Exchange

Сведения о том, как использовать Exchange для разработки средств администрирования Exchange сервера.
  
**Применяется к:** Exchange Online | Exchange Server 2013 | Office 365
  
В Exchange Management Shell предоставляется богатый набор команд, основанных на платформе Windows PowerShell, для управления Exchange Online, Exchange Online в составе Office 365 или локальной версии Exchange начиная с Exchange 2013 г. С помощью Exchange командной оболочки можно создать два типа инструментов: скрипты командной строки, которые работают в среде Windows PowerShell, и средства, которые используют командлеты Exchange Management Shell с помощью управляемого интерфейса. Управляемые приложения можно использовать для создания стандартного пользовательского Windows или веб-интерфейса для администрирования Exchange сервера. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Что нужно знать о Exchange управленческой оболочки

|Если вам интересно,|Прочтите это|
|:-----|:-----|
|Доступность  <br/> |Exchange Команды команд команд командной оболочки управления устанавливаются на всех серверах, на Exchange начиная с Exchange 2007 года.<br/>Клиентские приложения можно развернуть на любом компьютере с Windows PowerShell 2.0.<br/> Сведения о доступе к оболочке см. в [Exchange Server PowerShell (Exchange Management Shell).](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)  <br/> |
|Языки и инструменты  <br/> |Вы можете создавать Exchange в любом текстовом редакторе.<br/>Вы можете использовать один из многих сторонних средств для создания Windows PowerShell сценариев, которые можно использовать с помощью Exchange Management Shell.  <br/> Объектная [модель Exchange Management Shell](exchange-management-shell-namespaces.md) основана на платформа .NET Framework.<br/>Вы можете использовать любой язык .NET для разработки Exchange приложений для управления shell.  <br/> |
|Доступные инструменты для тестирования и отладки  <br/> |Вы можете использовать одно из многих сторонних приложений для тестирования и отлаговки сценариев Exchange управления Shell.  <br/> Вы можете использовать Visual Studio и сторонние средства для тестирования и отламывки управляемых Exchange приложений управленческой оболочки.  <br/> |
|Требования к платформе сервера  <br/> |Вы можете использовать Exchange на любом сервере Exchange, на Windows PowerShell установлено 2.0.  <br/> |
|Требования к платформе клиента  <br/> |Exchange Клиентские приложения Management Shell требуют Windows PowerShell 2.0.  <br/> |
|Permissions  <br/> |Для Exchange приложения Management Shell требуется, чтобы пользователь мог управлять правами на управление доступом на основе ролей к затронутым данным в Exchange магазине.<br/>Дополнительные сведения о контроле доступа на основе ролей см. в см. в нем [Understanding Role Based Access Control.](https://technet.microsoft.com/library/dd298183.aspx)  <br/> |
   
В статьях в этом разделе описываются Exchange, важные для создания Exchange управления. Сведения о планировании, настройке или обслуживании Exchange [](https://docs.microsoft.com/exchange/) см. в Exchange сайте.
  
## <a name="in-this-section"></a>В этом разделе:

- [Создание инструментов командной консоли Exchange](create-exchange-management-shell-tools.md)
    
- [Пространства имен командной консоли Exchange](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>См. также
  
- [Windows PowerShell документации](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Сценарий PowerShell](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

