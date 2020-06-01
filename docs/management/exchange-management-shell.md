---
title: Командная консоль Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8cc0c4fa-9e13-45cb-88da-0486f2ac1bd0
description: Сведения о том, как использовать командную консоль Exchange для разработки средств для администрирования Exchange Server.
ms.openlocfilehash: 38e75339a4ad97cf8ff99e1cbe9c01059e157941
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435809"
---
# <a name="exchange-management-shell"></a>Командная консоль Exchange

Сведения о том, как использовать командную консоль Exchange для разработки средств для администрирования Exchange Server.
  
**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365
  
Командная консоль Exchange предоставляет богатый набор команд, основанный на платформе Windows PowerShell, для управления Exchange Online, Exchange Online в составе Office 365 или локальной версии Exchange, начиная с Exchange 2013. С помощью командной консоли Exchange можно создавать два типа инструментов: сценарии командной строки, работающие в среде Windows PowerShell, и средства, использующие командлеты командной консоли Exchange через управляемый интерфейс. С помощью управляемых приложений можно создать стандартный пользовательский интерфейс Windows или веб-интерфейс для администрирования сервера Exchange Server. 
  
## <a name="what-you-need-to-know-about-the-exchange-management-shell"></a>Что нужно знать о командной консоли Exchange

|Если вас интересует|Прочтите это|
|:-----|:-----|
|Доступность  <br/> |Команды Командная консоль Exchange устанавливаются на всех серверах, где запущены версии Exchange, начиная с Exchange 2007.<br/>Клиентские приложения можно развертывать на любом компьютере, работающем под управлением Windows PowerShell 2,0.<br/> Сведения о доступе к оболочке можно найти в статье [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).  <br/> |
|Языки и инструменты  <br/> |Вы можете создавать сценарии командной консоли Exchange в любом текстовом редакторе.<br/>Можно использовать один или несколько сторонних средств для создания сценариев Windows PowerShell, которые можно использовать в командной консоли Exchange.  <br/> [Объектная модель Командная консоль Exchange](exchange-management-shell-namespaces.md) основана на платформе .NET Framework.<br/>Для разработки приложений командной консоли Exchange можно использовать любой язык .NET.  <br/> |
|Доступные инструменты для тестирования и отладки  <br/> |Для тестирования и отладки сценариев консоли управления Exchange можно использовать одно из многих сторонних приложений.  <br/> С помощью Visual Studio и сторонних средств можно тестировать и отлаживать управляемые приложения командной консоли Exchange.  <br/> |
|Требования к платформе сервера  <br/> |Командную консоль Exchange можно использовать на любом сервере Exchange, на котором установлен Windows PowerShell 2,0.  <br/> |
|Требования к платформе клиента  <br/> |Клиентским приложениям командной консоли Exchange требуется Windows PowerShell 2,0.  <br/> |
|Разрешения  <br/> |Для запуска приложения командной консоли Exchange необходимо, чтобы у пользователя были права на управление доступом на основе ролей для затронутых данных в хранилище Exchange.<br/>Более подробную информацию об управлении доступом на основе ролей можно узнать в статье Общие сведения об [управлении доступом на основе](https://technet.microsoft.com/library/dd298183.aspx)ролей.  <br/> |
   
В статьях этого раздела описываются функции оболочки управления Exchange, важные для создания средств управления Exchange. Сведения о планировании, настройке или обслуживании Exchange можно найти на сайте [Exchange](https://docs.microsoft.com/exchange/) .
  
## <a name="in-this-section"></a>Содержание

- [Создание средств командной консоли Exchange](create-exchange-management-shell-tools.md)
    
- [Пространства имен командной консоли Exchange](exchange-management-shell-namespaces.md)
    
## <a name="see-also"></a>См. также
  
- [Документация по Windows PowerShell](https://docs.microsoft.com/powershell/scripting/getting-started/getting-started-with-windows-powershell?view=powershell-6)
- [Сценарии PowerShell](https://docs.microsoft.com/powershell/scripting/powershell-scripting?view=powershell-6)
    

