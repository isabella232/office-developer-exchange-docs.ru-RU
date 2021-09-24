---
title: Требования к перераспределению для управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 8b206274-eaa4-40d3-b504-af27335c8f43
description: Узнайте, как можно перераспределить сборки управляемых API EWS с помощью приложения.
ms.openlocfilehash: f43156838c735cfc17106deb7860329d3da6c07a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531332"
---
# <a name="redistribution-requirements-for-the-ews-managed-api"></a>Требования к перераспределению для управляемого API EWS

Узнайте, как можно перераспределить сборки управляемых API EWS с помощью приложения.
  
При разработке приложения управляемого API EWS необходимо также рассмотреть вопрос о том, как вы отпустите его для пользователей. 
  
## <a name="redistributing-your-ews-managed-api-application"></a>Перераспределение приложения управляемого API EWS

Если приложение не расположено на Exchange сервере, вам потребуется перераспределить сборки управляемого API EWS. Загрузка управляемого API EWS содержит две сборки, которые можно перераспределить: Microsoft.Exchange.WebServices.dll и Microsoft.Exchange.WebServices.Auth.dll. При разработке разработки приложения управляемого API EWS следует помнить следующие сведения:
  
- Управляемый API EWS разработан таким образом, что его можно скачать и распространить с помощью приложения, предназначенного для Exchange сервера. Кроме того, приложение может скачать управляемый API EWS.
    
- Управляемый API EWS можно использовать для связи с сервером Exchange с Exchange Online, Exchange Online в Office 365 или локальной версией Exchange начиная с Exchange Server 2007 г.
    
- В версиях управляемого API EWS, начиная с версии 2.1, можно установить API в кэше глобальной сборки (GAC). MSI автоматически добавляет DLL в GAC и будет доступен на компьютере, а не на основе каждого пользователя.
    
Условия лицензии включены в загрузку управляемого API EWS. Просмотрите условия получения достоверной информации о том, что можно сделать с управляемым API EWS.
  
## <a name="see-also"></a>См. также


- [Общие сведения о разработке клиента EWS для Exchange](ews-client-design-overview-for-exchange.md)
    
- [Управляемый API EWS (скачивание)](https://aka.ms/ews-managed-api-readme)
    

