---
title: Общие сведения о разработке клиента EWS для Exchange
manager: sethgros
ms.date: 3/11/2016
ms.audience: Developer
ms.assetid: b26f67aa-7c66-4d7d-98b3-746f26ab37f4
description: Советы по разработке с использованием EWS для Exchange.
localization_priority: Priority
ms.openlocfilehash: 0ac4fe1be0800008af572ebc296e004aa29d8daf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455424"
---
# <a name="ews-client-design-overview-for-exchange"></a>Общие сведения о разработке клиента EWS для Exchange

Советы по разработке с использованием EWS для Exchange. 
  
В этой статье приведены общие сведения о создании приложения веб-служб Exchange (EWS). С помощью этих сведений можно определить, подходит ли API EWS для вашего приложения и какой тип реализации клиента вам нужен. Эта статья также содержит рекомендации по созданию приложений для Office 365, Exchange Online и версий Exchange, и версий Exchange, начиная с Exchange 2007, с использованием одной базы данных кода. Кроме того, она помогает решить, для какой среды лучше разрабатывать решения — для локальных серверов Exchange Server или Exchange Online.
  
## <a name="is-ews-the-right-api-for-your-application"></a>Подходит ли API EWS для вашего приложения?
<a name="IsEWSRight"> </a>

Прежде чем приступать к созданию приложения, необходимо определить, подходит ли вам API EWS. Если вы разрабатываете решение для Exchange Server или Exchange Online, EWS предпочтительной будет технология клиентского доступа. Разработка решений клиентского доступа для версий Exchange, начиная с Exchange 2007, в основном ориентировалась на EWS. EWS используется для работы новых функций клиентского доступа, реализованных в Outlook. К последним относится отображение состояния "нет на месте" и сведений о доступности, впервые доступное в Exchange 2007, а также функции подсказок и получения помещений, представленные в Exchange 2010. И для внутренних, и для внешних партнеров, разрабатывающих клиентские приложения Exchange, это говорит в пользу обязательности вложений в EWS.
  
API EWS — основной API клиентского доступа для клиентских приложений Exchange. Но в некоторых случаях для разработки клиентских приложений могут пригодиться другие API Exchange. Например, Exchange ActiveSync обладает следующими преимуществами перед EWS:
  
- Чтобы сделать протокол Exchange ActiveSync более компактным, проведена разметка структуры XML.  
- Exchange ActiveSync позволяет с помощью политик управлять клиентским доступом и использовать другие надежные решения для обмена мобильными сообщениями на предприятии.
    
> [!NOTE]
> Для разработки клиентов Exchange ActiveSync нужна лицензия. Дополнительные сведения о различиях между Exchange ActiveSync и EWS см. в статье [Choosing between Exchange ActiveSync and Exchange Web Services (EWS)](https://msdn.microsoft.com/library/dn144954%28v=exchg.140%29.aspx). 
  
MAPI RPC/HTTP — это еще один вариант для программирования клиентских приложений Exchange. Но тем не менее MAPI RPC/HTTP не обладает интуитивно понятным интерфейсом для связи между клиентами и сервером.
  
Дополнительные сведения о технологиях разработки для Exchange см. в статье [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).
  
## <a name="options-for-ews-client-development"></a>Способы разработки клиента EWS
<a name="EWSClientOptions"> </a>

Существует несколько способов разработки для Exchange с использованием EWS. Выбор оптимального варианта зависит от платформы разработки, инструментов, доступных реализаций и требований к приложениям для организации. Для создания клиентских приложений EWS доступны четыре основных варианта:
  
- управляемый API EWS;
- Java API EWS;
- автоматически созданные прокси EWS;
- настраиваемый клиентский API EWS.
    
### <a name="ews-managed-api"></a>Управляемый API EWS

[EWS Managed API](https://aka.ms/ews-managed-api-readme) является настраиваемым клиентом веб-службы. Он является стандартным API клиентского доступа для приложений .NET Framework. 
  
Вот несколько преимуществ управляемого API EWS:
  
- позволяет использовать интуитивно понятную объектную модель;   
- устраняет сложности описания служб в файлах схемы и WSDL;   
- включает в себя клиентскую бизнес-логику;   
- обрабатывает веб-запросы и веб-отклики, а также сериализацию и десериализацию объектов;   
- его поддерживает корпорация Майкрософт.
    
Обратите внимание, что управляемый API EWS — не полное решение. В управляемом API EWS не реализованы некоторые функции. Несмотря на то что управляемый API EWS не обладает всеми функциями EWS, он может оказаться лучшим вариантом для разработки клиентских приложений по следующим причинам:
  
- для разработки можно использовать .NET Framework;
- интерфейс позволяет реализовать автообнаружение в дополнение к большинству элементов объектной модели EWS;
- он реализует клиентскую бизнес-логику для работы с EWS в классе [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx). 
    
API веб-службы EWS может подойти вам больше, чем управляемый API EWS, по одной из следующих причин:
  
- ваше приложение не использует .NET Framework; 
- вы не хотите распространять сборку управляемого API EWS; 
- для приложения требуются функции, не доступные в управляемом API EWS.
    
Для получения дополнительной информации см. статью [Get started with EWS Managed API client applications](get-started-with-ews-managed-api-client-applications.md).
  
> [!NOTE]
> Управляемое API EWS теперь доступно в качестве проекта с открытым кодом на [GitHub](https://aka.ms/ews-managed-api-github). Вы можете использовать библиотеку открытого кода, чтобы: 
> - добавлять исправления ошибок и улучшения в API; 
> - получать исправления ошибок и улучшения до того, как они станут доступны в официальном выпуске;
> - получать доступ к самой полной и актуальной реализации API, которую можно использовать для справки или для создания новых библиотек на новых платформах.
> 
> Мы будем рады вашему [вкладу](https://github.com/OfficeDev/ews-managed-api/blob/master/CONTRIBUTING.md) в GitHub. 
  
### <a name="ews-java-api"></a>Java API веб-служб EWS

Java API EWS — это проект с открытым исходным кодом на сайте [GitHub](https://github.com/OfficeDev/ews-java-api), который сообщество может обновлять и расширять. Стилистически он похож на [EWS Managed API](https://msdn.microsoft.com/library/office/jj220535%28v=exchg.80%29.aspx) и использует сетевые запросы и ответы EWS SOAP. Хотя с помощью Java API EWS невозможно получить доступ ко всем [операциям EWS SOAP](https://msdn.microsoft.com/library/cf6fd871-9a65-4f34-8557-c8c71dd7ce09%28Office.15%29.aspx), но мы надеемся, что после [недавнего создания](https://blogs.office.com/2014/08/28/open-sourcing-exchange-web-services-ews-java-api/) проекта с открытым кодом сообщество поможет преодолеть это препятствие. Обратите внимание, что при наличии соответствующего контракта о поддержке служба поддержки Майкрософт поможет разобраться со всеми вопросами, связанными с протоколом SOAP EWS, но не с самим Java API EWS. Java API EWS доступен для скачивания на сайте [GitHub](https://github.com/OfficeDev/ews-java-api), где члены сообщества могут внести свой вклад в его развитие.

  
### <a name="ews-autogenerated-proxies"></a>Автоматически созданные прокси EWS

Клиентские API могут быть созданы автоматически с использованием определений схем XML и WSDL EWS. Генераторы клиентских объектных моделей доступны для многих языков. Как правило, автоматически созданные объектные модели управляют сериализацией и десериализацией объектов. Такие модели не включают бизнес-логику. Кроме того, автоматическое создание часто приводит к появлению артефактов, усложняющих работу с объектной моделью. Поддержка Exchange распространяется на XML-код, который клиент отправляет и получает, но не на объектную модель.
  
### <a name="custom-ews-client-api"></a>Настраиваемый клиентский API EWS

Для некоторых приложений, которые используют лишь малую часть возможностей EWS, можно создать настраиваемый клиентский API для связи с Exchange. Такой способ позволит сократить использование системных ресурсов. Это удобно для клиентов, работающих на устройствах с ограниченной памятью (например, использующих .NET Micro Framework).
  
## <a name="ews-client-features"></a>Возможности клиента EWS
<a name="EWSFeatures"> </a>

Какой бы вариант разработки вы ни выбрали, следует обдумать способ реализации возможностей EWS в клиенте. Доступность возможностей зависит от версии схемы EWS, для которой будете создавать приложение. Схемы EWS обратно и прямо совместимы. Если вы создаете приложение для более ранней версии схемы (например, Exchange Server 2007 с пакетом обновления 1), оно также будет работать с более поздними версиями схемы (например, с Exchange Online и службой Exchange Server 2013 с пакетом обновления 1).  
  
Так как функции и их обновления зависят от схемы, рекомендуем использовать наиболее раннюю базу общего кода, которая относится к тем возможностям EWS, которые нужно реализовать в клиентском приложении. Многие приложения могут работать с версией Exchange2007_SP1, потому что схема Exchange 2007 с пакетом обновления 1 содержит почти все основные возможности Exchange для работы с элементами и папками в хранилище Exchange. Рекомендуем сохранять ветви кода для каждой версии схемы EWS. Ниже приведены версии схем, доступные в настоящее время.  
  
```XML
  <xs:simpleType name="ExchangeVersionType">
    <xs:restriction base="xs:string">
      <xs:enumeration value="Exchange2007" />
      <xs:enumeration value="Exchange2007_SP1" />
      <xs:enumeration value="Exchange2010" />
      <xs:enumeration value="Exchange2010_SP1" />
      <xs:enumeration value="Exchange2010_SP2" />
      <xs:enumeration value="Exchange2013" />
      <xs:enumeration value="Exchange2013_SP1" />
    </xs:restriction>
  </xs:simpleType>
```

Версии схем хранятся в простом типе **ExchangeVersionType**. 
  
Сведения о возможностях, доступных в каждой из версий схем EWS, см. в статье [EWS schema versions in Exchange](ews-schema-versions-in-exchange.md).
  
## <a name="in-this-section"></a>В этой статье
<a name="bk_inthissection"> </a>

- [Доступность функции веб-службы API в Exchange и в Управляемом API EWS](web-service-api-feature-availability-in-exchange-and-the-ews-managed-api.md)   
- [Версии схемы EWS в Exchange](ews-schema-versions-in-exchange.md)  
- [Настройка параметров для EWS в Exchange](configuration-options-for-ews-in-exchange.md)  
- [Сравнение программирования локальных клиентов Exchange Online и Exchange](comparing-exchange-online-and-exchange-on-premises-client-programming.md)   
- [EWS регулирование в Exchange](ews-throttling-in-exchange.md)  
- [Требования к перераспределению для управляемого API EWS](redistribution-requirements-for-the-ews-managed-api.md)  
- [Инструментирование запросов клиентов для EWS и REST в Exchange](instrumenting-client-requests-for-ews-and-rest-in-exchange.md)
    
## <a name="see-also"></a>См. также
 
- [Начало работы с веб-службами Exchange](start-using-web-services-in-exchange.md)
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md) 
- [Типы приложений EWS](ews-application-types.md)
    

