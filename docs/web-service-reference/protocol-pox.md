---
title: Protocol (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.localizationpriority: medium
api_type:
- schema
ms.assetid: f77e4d66-6fdd-4999-9339-f7d7f9c86f44
description: Элемент Protocol содержит спецификации для подключения клиента к компьютеру, на Exchange Server установлена роль сервера клиентского доступа.
ms.openlocfilehash: 4f308951c74612936755e6d4c16620e38277aecb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516400"
---
# <a name="protocol-pox"></a>Protocol (POX)

Элемент **Protocol** содержит спецификации для подключения клиента к компьютеру, на Exchange Server установлена роль сервера клиентского доступа. 
  
[AutoDiscover (POX)](autodiscover-pox.md)
  
[Response (POX)](response-pox.md)
  
[Account (POX)](account-pox.md)
  
[Protocol (POX)](protocol-pox.md)
  
```xml
<Protocol>
   <Type/>
   <Internal/>
   <External/>
   <TTL/>
   <Server/>
   <ServerDN/>
   <ServerVersion/>
   <MdbDN/>
   <PublicFolderServer/>
   <Port/>
   <DirectoryPort/>
   <ReferralPort/>
   <ASUrl/>
   <EwsUrl/>
   <EmwsUrl/>
   <SharingUrl/>
   <EcpUrl/>
   <EcpUrl-um/>
   <EcpUrl-aggr/>
   <EcpUrl-mt/>
   <EcpUrl-ret/>
   <EcpUrl-sms/>
   <EcpUrl-publish/>
   <EcpUrl-photo/>
   <EcpUrl-tm/>
   <EcpUrl-tmCreating/>
   <EcpUrl-tmHiding/>
   <EcpUrl-tmEditing/>
   <EcpUrl-extinstall/>
   <OOFUrl/>
   <OABUrl/>
   <UMUrl/>
   <EwsPartnerUrl/>
   <LoginName/>
   <DomainRequired/>
   <DomainName/>
   <SPA/>
   <AuthPackage/>
   <CertPrincipalName/>
   <SSL/>
   <AuthRequired/>
   <UsePOPAuth/>
   <SMTPLast/>
   <NetworkRequirements/>
   <AddressBook/>
   <MailStore/>
</Protocol>
```

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Тип  <br/> |Указывает тип протокола, описанный в этом **элементе Протокола.** Единственным допустимым значением для этого атрибута является "mapiHttp". Этот атрибут присутствует только в том случае, если запрос автооткрытия, соответствующий этому ответу, содержит заглавную заголовку [X-MapiHttpCapability.](pox-autodiscover-request-for-exchange.md) Этот атрибут применим к клиентам, которые реализуют протокол MAPI/HTTP и целевые Exchange Online, Exchange Online как часть Office 365 или локальной версии Exchange, начиная со сборки 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
|Версия  <br/> |Указывает версию протокола, описанную этим элементом **Протокола.** Единственным допустимым значением для этого атрибута является "1". Этот атрибут присутствует только в том случае, если запрос автооткрытия, соответствующий этому ответу, включал заголовку **X-MapiHttpCapability.** Этот атрибут применим к клиентам, которые реализуют протокол MAPI/HTTP и целевые Exchange Online, Exchange Online как часть Office 365 или локальной версии Exchange, начиная со сборки 15.00.0847.032 (Exchange Server 2013 SP1).  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Type (POX)](type-pox.md) <br/> |Определяет тип настроенной учетной записи почты.  <br/> |
|[Internal (POX)](internal-pox.md) <br/> |Содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из сети организации.  <br/> |
|[External (POX)](external-pox.md) <br/> |Содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из-за пределов сети организации.  <br/> |
|[TTL (POX)](ttl-pox.md) <br/> |Указывает время для жизни в часы, в течение которых параметры остаются допустимы.  <br/> |
|[Server (POX)](server-pox.md) <br/> |Указывает имя почтового сервера.  <br/> |
|[ServerDN (POX)](serverdn-pox.md) <br/> |Указывает Exchange Server имя.  <br/> |
|[ServerVersion (POX)](serverversion-pox.md) <br/> |Представляет номер Exchange Server версии.  <br/> |
|[MdbDN (POX)](mdbdn-pox.md) <br/> |Представляет отличительное имя базы данных почтовых ящиков.  <br/> |
|[PublicFolderServer (POX)](publicfolderserver-pox.md) <br/> |Содержит полное доменное имя (FQDN) сервера общедоступных папок для пользователя.  <br/> |
|[Port (POX)](port-pox.md) <br/> |Указывает порт, используемый для подключения к магазину.  <br/> |
|[DirectoryPort (POX)](directoryport-pox.md) <br/> |Указывает порт, используемый для подключения к каталогу, когда используется протокол интерфейса поставщика услуг имен (NSPI).  <br/> |
|[ReferralPort (POX)](referralport-pox.md) <br/> |Указывает порт, используемый для получения направления в каталог.  <br/> |
|[ASUrl (POX)](asurl-pox.md) <br/> |Указывает URL-адрес наилучшего экземпляра веб-Exchange для пользователя с включенной почтой.  <br/> |
|[EwsUrl (POX)](ewsurl-pox.md) <br/> |Указывает URL-адрес наилучшего экземпляра конечной точки для Exchange веб-служб (EWS) для пользователя с включенной почтой.  <br/> |
|[EmwsUrl (POX)](emwsurl-pox.md) <br/> |Указывает URL-адрес наилучшего экземпляра конечной точки для Exchange веб-служб (EWS) для пользователя с включенной почтой.  <br/> |
|[SharingUrl (POX)](sharingurl-pox.md) <br/> |Содержит URL-адрес сервера общего доступа, используемого для совместного использования календарей и контактов.  <br/> |
|[EcpUrl (POX)](ecpurl-pox.md) <br/> |Указывает URL-адрес панели управления Exchange для пользователя с включенной почтой.  <br/> |
|[EcpUrl-um (POX)](ecpurl-um-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам голосовой почты для пользователя с включенной почтой.  <br/> |
|[EcpUrl-aggr (POX)](ecpurl-aggr-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам агрегации электронной почты для пользователя с включенной почтой.  <br/> |
|[EcpUrl-mt (POX)](ecpurl-mt-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам отслеживания сообщений электронной почты для пользователя с включенной почтой.  <br/> |
|[EcpUrl-ret (POX)](ecpurl-ret-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам тегов хранения для пользователя с поддержкой почты.  <br/> |
|[EcpUrl-sms (POX)](ecpurl-sms-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к настройкам службы коротких сообщений (SMS) для пользователя с включенной почтой.  <br/> |
|[EcpUrl-publish (POX)](ecpurl-publish-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к параметрам публикации календаря для пользователя с поддержкой почты.  <br/> |
|[EcpUrl-photo (POX)](ecpurl-photo-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для просмотра или изменения текущей фотографии пользователя с поддержкой почты.  <br/> |
|[EcpUrl-tm (POX)](ecpurl-tm-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для доступа к списку всех почтовых ящиков сайта, участником которых в настоящее время является пользователь с поддержкой почты.  <br/> |
|[EcpUrl-tmCreating (POX)](ecpurl-tmcreating-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для создания нового почтового ящика сайта.  <br/> |
|[EcpUrl-tmHiding (POX)](ecpurl-tmhiding-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для отписки пользователя из почтового ящика сайта.  <br/> |
|[EcpUrl-tmEditing (POX)](ecpurl-tmediting-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для редактирования существующего почтового ящика сайта.  <br/> |
|[EcpUrl-extinstall (POX)](ecpurl-extinstall-pox.md) <br/> |Указывает частичный URL-адрес, который можно сочетать со значением [элемента EcpUrl (POX)](ecpurl-pox.md) для создания URL-адреса, который можно использовать для просмотра или изменения почтовых приложений, установленных в почтовом ящике пользователя.  <br/> |
|[OOFUrl (POX)](oofurl-pox.md) <br/> |Указывает URL-адрес лучшего экземпляра службы доступности для пользователя с поддержкой почты.  <br/> |
|[OABUrl (POX)](oaburl-pox.md) <br/> |Указывает URL-адрес сервера конфигурации автономной адресной книги для Exchange топологии.  <br/> |
|[UMUrl (POX)](umurl-pox.md) <br/> |Указывает URL-адрес наилучшего экземпляра веб-службы единой системы обмена сообщениями для пользователя с поддержкой почты.  <br/> |
|[EwsPartnerUrl (POX)](ewspartnerurl-pox.md) <br/> |Указывает URL-адрес наилучшего экземпляра конечной точки для Exchange веб-служб (EWS) для пользователя с включенной почтой.  <br/> |
|[LoginName (POX)](loginname-pox.md) <br/> |Указывает имя логотипа пользователя.  <br/> |
|[DomainRequired (POX)](domainrequired-pox.md) <br/> |Указывает, требуется ли домен для проверки подлинности.  <br/> |
|[DomainName (POX)](domainname-pox.md) <br/> |Указывает домен пользователя.  <br/> |
|[SPA (POX)](spa-pox.md) <br/> |Указывает, требуется ли проверка подлинности безопасного пароля.  <br/> |
|[AuthPackage (POX)](authpackage-pox.md) <br/> |Указывает схему проверки подлинности, используемую при проверке подлинности на компьютере 2007 Exchange 2007 года с установленной ролью сервера почтовых ящиков.  <br/> |
|[CertPrincipalName (POX)](certprincipalname-pox.md) <br/> |Указывает основное имя сертификата уровня безопасных sockets (SSL), необходимое для подключения к организации Microsoft Exchange с помощью SSL.  <br/> |
|[SSL (POX)](ssl-pox.md) <br/> |Указывает, необходим ли безопасный логотип.  <br/> |
|[AuthRequired (POX)](authrequired-pox.md) <br/> |Указывает, требуется ли проверка подлинности.  <br/> |
|[UsePOPAuth (POX)](usepopauth-pox.md) <br/> |Указывает, используются ли сведения о проверке подлинности, предоставляемые для учетной записи типа POP3, также для протокола простой передачи почты (SMTP).  <br/> |
|[SMTPLast (POX)](smtplast-pox.md) <br/> |Указывает, требуется ли для smTP-сервера скачивание электронной почты перед отправкой электронной почты с помощью сервера SMTP.  <br/> |
|[NetworkRequirements (POX)](networkrequirements-pox.md) <br/> |Содержит критерии, используемые для определения того, находится ли клиентский компьютер в сети, которая соответствует требованиям поставщика интернет-услуг для подключения к серверу.  <br/> |
|[AddressBook (POX)](addressbook-pox.md) <br/> |Содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP. Этот элемент присутствует только в том случае, если атрибут **Type** в элементе **Protocol** присутствует и заданной на "mapiHttp". Элемент **AddressBook** применим к клиентам, реализующими протокол MAPI/HTTP и целевые Exchange Online и версии Exchange начиная с 15.00.0847.032.  <br/> |
|[MailStore (POX)](mailstore-pox.md) <br/> |Содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP. Этот элемент присутствует только в том случае, если атрибут **Type** в элементе **Protocol** присутствует и заданной на "mapiHttp". Элемент **MailStore** применим к клиентам, реализующими протокол MAPI/HTTP и целевые Exchange Online и версии Exchange начиная с 15.00.0847.032.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Account (POX)](account-pox.md) <br/> |Указывает параметры учетной записи для пользователя.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **Protocol** присутствует в ответе, которое имеет значение [Action (POX),](action-pox.md) равное **настройкам.**
  
## <a name="see-also"></a>См. также



[Элементы XML автооткрытия POX для Exchange](pox-autodiscover-xml-elements-for-exchange.md)

