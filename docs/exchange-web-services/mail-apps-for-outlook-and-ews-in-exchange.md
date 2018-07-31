---
title: Надстройки Outlook и веб-службах Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Найдите сведения о надстройках Outlook и работы с веб-служб Exchange в Exchange.
ms.openlocfilehash: fc004108c7f31ea6475d61f4e2cd2289b13d27f5
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353639"
---
# <a name="outlook-add-ins-and-ews-in-exchange"></a>Надстройки Outlook и веб-службах Exchange

Найдите сведения о надстройках Outlook и работы с веб-служб Exchange в Exchange.

Надстройки Outlook предоставляют единый интерфейс и модель программирования, которая использует веб-стандартов для создания пользовательского интерфейса для пользователей электронной почты. Можно создать почтовых приложений, отображающих сведения о контекстной или полезны в кадре HTML5, размещенных в Outlook; к примеру почтовое приложение позволяет показывать карты Bing с адресом выделен, если сообщение электронной почты содержит адрес. Или при создании сообщения в почтового приложения можно отобразить дополнительные сведения о получателе и Вставить стандартный приветствие в сообщение электронной почты нажатием кнопки.

> [!NOTE]
> В этой статье "Outlook" означает расширенный клиент Outlook, Outlook RT, Outlook Web App и OWA для устройств.

Интерфейс приложения почты является частью JavaScript API для Office. API можно использовать для доступа к сведениям в Exchange для включения вашего почтового приложения:

- [Распознавать сущности](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), как адреса, номера телефонов, предложения задач или предложения о собраниях в сообщение электронной почты.

- Открытие и отображение существующих [сообщений](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) и [встреч](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) в отдельном представлении, чтобы пользователи могут перекрестная ссылка сведения в одно или несколько сообщений.

- [Запросы на выполнение веб-служб Exchange](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) на сервере Exchange, на котором размещен почтовый ящик пользователя. Почтовое приложение например, список можно получить папок, чтобы пользователя можно выбрать один для хранения сообщения или отображение всех элементов в беседе или пометить как нежелательные сообщения электронной почты.

- [Получить маркер](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) для уникальной идентификации учетной записи электронной почты для включения единого входа службе сторонних производителей.

- [Получить маркер](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) , позволяющий сторонних служб мог выполнять запросы EWS от имени пользователя, например, чтобы извлечь вложения из элемента или для получения элемента с сервера Exchange server для дальнейшей обработки.

Почтовые приложения можно использовать для настройки взаимодействия Outlook Web App для пользователей; Если необходимо настроить «внешний вид и функции» из Outlook Web App, отображается в этих статьях на сайте TechNet:

- [Создание темы для Outlook Web App](http://technet.microsoft.com/en-us/library/bb201700%28v=exchg.150%29.aspx)

- [Настройка Outlook Web App входа, выбора языка и страницы ошибок](http://technet.microsoft.com/en-us/library/ee633483%28v=exchg.150%29.aspx)

Вашей организации можно установить почтовых приложений на внутреннем сервере для ограничения доступа к авторизованные пользователи, или вы разработчиков приложений и других почтовых приложений можно размещать почтовых приложений в [Магазине Office](http://office.microsoft.com/store/) для продажи для всех. Любой пользователь, запущен Outlook можно загрузить, установить и использовать почтовые приложения из магазина.

Если вы хотите узнать больше о создании почтовых приложений, извлечь [документации надстроек Outlook](/outlook/add-ins/index.md) или пример [выполнения запроса веб-служб Exchange](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) .

## <a name="ews-and-outlook-add-ins"></a>Надстройки Outlook и веб-служб Exchange

Можно использовать подмножества операций веб-служб Exchange на сервере Exchange, на котором размещается учетная запись, запускающая почтового приложения.

Функция [mailbox.makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) позволяет выполнять запросы EWS из почтового приложения на сервере, на котором размещен почтовый ящик пользователя. Создайте конверте SOAP и XML-запрос и вызовы функций **makeEwsRequestAsync** веб-служб Exchange с помощью маркера проверки подлинности, который идентифицирует почтовый ящик и почтовые приложения, делающего запрос. Для улучшения защиты почтового ящика пользователя, Exchange server будет отклонять все запросы, полученные из почтового приложения или из почтового ящика, который не находится на сервере.

Как и другие приложения почтовое приложение должно разрешения для работы. Администратор должен:

- [Веб-служб Exchange предоставление доступа](controlling-client-application-access-to-ews-in-exchange.md) к пользователю почтового приложения.

- [Набор параметра «OAuthAuthentication» имеет значение true](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) в каталоге Client Access Server EWS.

Необходимо также убедитесь в том, что ваше приложение запрашивает разрешение чтение и запись почтового ящика в приложениях для Office [модель разрешений](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).

После выполнения этих шагов подмножество папки и операции EWS элемента доступны для почтового приложения для использования.

**В таблице 1. Можно использовать операции папок и элементов веб-служб Exchange, почтовые приложения**

|**Папка операций**|**Операции с элементами**|
|:-----|:-----|
|[Операция CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [Операция FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [Операция GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [Операция UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[Операция CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [Операция CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [Операция FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [Операция FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [Операция GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [Операция GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [Операция MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [Операция MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [Операция SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [Операция UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |

### <a name="service-callback-tokens"></a>Служба маркеров обратного вызова

Служба маркеров обратного вызова включите почтовые приложения передать маркер доступа к службе сторонних производителей, чтобы службы можно выполнять запросы EWS на сервере Exchange, на котором размещен почтовый ящик. Например почтового приложения можно передать маркер обратного вызова службы сторонних служб вместе со списком идентификаторы вложений для изображений, подключенного к сообщения электронной почты. Служба будет использовать идентификаторы вложений и маркер обратного вызова для выполнения запроса EWS для пользователя Exchange server для получения вложенных рисунков. Также почтовые приложения могут использовать маркер обратного вызова службы со списком идентификаторов элементов для получения элементов электронной почты и встречи с сервера Exchange.

Маркер обратного вызова службы — это непрозрачный маркера, который подключает службы сторонних производителей для запроса веб-служб Exchange в заголовок проверки подлинности носителя. Маркер определяет почтового приложения и почтовых ящиков для улучшения защиты запроса веб-служб Exchange. Чтобы узнать, как использовать службы маркеров обратного вызова, обратитесь к разделу [надстроек Outlook: получение вложений с сервера Exchange,](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) образца.

## <a name="see-also"></a>См. также


- [Управление доступом к клиентского приложения для веб-служб Exchange в Exchange](controlling-client-application-access-to-ews-in-exchange.md)

- [Метод Mailbox.makeEwsRequestAsync (API JavaScript для Office)](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)

- [Надстройки Outlook](https://docs.microsoft.com/en-us/outlook/add-ins/)

- [Метод Mailbox.getUserIdentityTokenAsync (API JavaScript для Office)](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)

- [Проверка подлинности надстройки Outlook с помощью маркеров удостоверений Exchange](http://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)

- [Общие сведения о разрешениях для надстроек Outlook](https://docs.microsoft.com/en-us/outlook/add-ins/understanding-outlook-add-in-permissions)

- [SET-WebServicesVirtualDirectory](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)

- [Надстройки Outlook: для выполнения запроса EWS](http://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)

- [Надстройки Outlook: Использование маркера удостоверения клиента](http://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)

- [Надстройки Outlook: получение вложений с сервера Exchange](http://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)
