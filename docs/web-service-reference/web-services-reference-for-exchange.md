---
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.assetid: 6c969133-6036-448b-af39-a3caf9917e98
description: Справочные сведения по веб-службам в Exchange.
localization_priority: Priority
ms.openlocfilehash: 8bdb3d6c4244bf8e0f092f5a9ffa3de5e8f1c3c2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467349"
---
# <a name="web-services-reference-for-exchange"></a>Справочник по веб-службам для Exchange

Справочные сведения по веб-службам в Exchange.
  
В этом разделе приведены справочные сведения по интерфейсам API, нацеленным на Exchange Online, Exchange Online в составе Office 365, а также на версии Exchange, начиная с Exchange Server 2007 или включенным в эти службы. Этот раздел включает:
  
- [Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)  содержит справочную документацию по API для API веб-служб Exchange (EWS). Это основной интерфейс API для создания клиентов и служб, подключаемых к Exchange для получения доступа к сведениям о почтовом ящике. Здесь вы найдете информацию об операциях, доступных в EWS, а также справочную документацию по XML, которая содержит данные об XML-документе экземпляра, отправляемом в или получаемом из Exchange. 
    
- [Справочник по управляемому API EWS](ews-managed-api-reference-for-exchange.md)  содержит справочную документацию по API для управляемого API EWS. Управляемый API EWS представляет собой простой и полнофункциональный интерфейс для разработки и расширения приложений, используемых EWS. 
    
- [Ссылки веб-службу автообнаружения для Exchange](autodiscover-web-service-reference-for-exchange.md)  содержит справочник по API XML для служб автообнаружения, предоставляемых Exchange. Интерфейсы API автообнаружения передают данные подготовки в клиентские приложения, что позволяет им автоматически обнаруживать конечные точки службы Exchange. 
    
- [Единой системы обмена сообщениями веб-службы ссылки для Exchange](unified-messaging-web-service-reference-for-exchange.md)  содержит справочник API XML для веб-службы единой системы обмена сообщениями. Веб-служба единой системы обмена сообщениями обеспечивает клиентским приложениям доступ к функциям единой системы обмена сообщениями в Exchange. Обратите внимание, что EWS также предоставляет функциональные возможности единой системы обмена сообщениями. 
    
- [Веб-служб Exchange создан объектных моделей для Exchange](ews-generated-object-models-reference-for-exchange.md)  содержит справочник по API для автоматически созданных прокси-классов в пространстве имен ExchangeWebServices. 
    
    > [!NOTE]
    > Для клиентов, основанных на версиях платформы .NET Framework, начиная с версии платформы .NET Framework 3.5, мы рекомендуем использовать для доступа к EWS управляемый API EWS. Дополнительные сведения см. в статье [Начало работы с клиентскими приложениями, использующими управляемый API EWS](../exchange-web-services/get-started-with-ews-managed-api-client-applications.md). 
  
Чтобы узнать, какой набор интерфейсов API использовать, ознакомьтесь со статьей [Общие сведения о разработке клиента EWS для Exchange](../exchange-web-services/ews-client-design-overview-for-exchange.md).
  
Справочник по XML для Exchange основывается на экземплярах XML, которыми обмениваются клиент и сервер. Язык XML описывается в файлах WSDL и XSD для служб автообнаружения EWS и SOAP. В веб-службе единой системы обмена сообщениями и службе автообнаружения POX отсутствуют WSDL-файлы и файлы схемы, описывающие их структуру. Справочник по XML для служб, не имеющих файлов схемы, основывается на экземплярах XML, которые удается наблюдать и захватывать в процессе обмена ними между клиентом и сервером.
  
## <a name="see-also"></a>См. также

- [Сведения об управляемом API EWS, EWS и веб-службах в Exchange](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [Начать работу с использованием веб-служб Exchange](../exchange-web-services/start-using-web-services-in-exchange.md)
- [Автообнаружение для Exchange](../exchange-web-services/autodiscover-for-exchange.md)
    

