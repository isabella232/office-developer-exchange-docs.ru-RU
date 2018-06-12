---
title: Требования к распространения для управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Узнайте, как можно распространять на сборки управляемого интерфейса API веб-служб Exchange с приложением.
ms.openlocfilehash: d8fc57c4a2b3ed7d6218aeeed0fe88c2d3e0fbe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761236"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Требования к распространения для управляемого API EWS

Узнайте, как можно распространять на сборки управляемого интерфейса API веб-служб Exchange с приложением.
  
При разработке приложения управляемый API веб-служб Exchange, необходимо также рассмотрим, как оно будет выпуска для пользователей. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Распространение приложения управляемый API EWS

Если приложение находится на сервере Exchange, необходимо будет распространять сборки управляемого интерфейса API веб-служб Exchange. Управляемый API EWS файл содержит две сборки, которые можно распространять: Microsoft.Exchange.WebServices.dll и Microsoft.Exchange.WebServices.Auth.dll. При разработке будет освобождение управляемый API EWS приложения необходимо учитывайте следующие сведения:
  
- Управляемый API веб-служб Exchange был разработан таким образом, можно загрузить и распространять с приложением, предназначенное для Exchange server. Кроме того приложение можно загрузить управляемый API веб-служб Exchange.
    
- Управляемый API веб-служб Exchange можно использовать для связи с сервером Exchange под управлением Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange Server 2007.
    
- В версиях управляемый API EWS начиная с версии 2.1 вы можете установить API в глобальный кэш сборок (GAC). MSI-файла автоматическое добавление библиотеки DLL в глобальный кэш сборок и будут доступны для каждого компьютера, а не на уровне пользователя.
    
Условия лицензионного соглашения будут включены в пакет загрузки управляемый API веб-служб Exchange. Ознакомьтесь с условиями достоверные сведения о возможностях управляемый API веб-служб Exchange.
  
## <a name="see-also"></a>См. также


- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    
- [Управляемый API EWS (файл для загрузки)](http://aka.ms/ews-managed-api-readme)
    

