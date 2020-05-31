---
title: Надстройки для Outlook и EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 821c8eb9-bb58-42e8-9a3a-61ca635cba59
description: Сведения о надстройках Outlook и их работе с EWS в Exchange.
ms.openlocfilehash: 7eae834fe0bb93e2e94f094e811ab6cf002fc71b
ms.sourcegitcommit: 42eecc78e7aed7e95f73370d6c39ab8f4e96bf68
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 10/12/2018
ms.locfileid: "25541640"
---
# <a name="outlook-add-ins-and-ews-in-exchange"></a>Надстройки для Outlook и EWS в Exchange

Сведения о надстройках Outlook и их работе с EWS в Exchange.

Надстройки Outlook предоставляют единый интерфейс и модель программирования, использующие веб-стандарты для создания пользовательского интерфейса для пользователей электронной почты. Вы можете создавать почтовые приложения, отображающие контекстные или полезные сведения в фрейме HTML5, размещенном в Outlook; Например, почтовое приложение может показывать карту Bing с адресом, выделенным, когда сообщение электронной почты содержит адрес. Или когда пользователь создает сообщение, почтовое приложение может показывать дополнительные сведения о получателе и вставлять стандартное приветствие в сообщение по нажатию кнопки.

> [!NOTE]
> В этой статье "Outlook" означает расширенный клиент Outlook, Outlook RT, Outlook Web App и OWA для устройств.

Интерфейс почтовых приложений является частью API JavaScript для Office. Вы можете использовать API для доступа к данным в Exchange, чтобы позволить почтовому приложению выполнять следующие действия:

- [Распознавание сущностей](http://msdn.microsoft.com/library/a6b0904b-afe9-4882-9136-3d8cfd57fcf8%28Office.15%29.aspx), таких как адреса, Номера телефонов, предложения по задачам и предложения о собраниях в сообщении электронной почты.

- Открытие и отображение существующих [сообщений](http://msdn.microsoft.com/library/d0bca550-70c3-457c-85f8-e19b39e3b892%28Office.15%29.aspx) и [встреч](http://msdn.microsoft.com/library/6cfbc29d-8581-474e-9a8b-510471e4bf8b%28Office.15%29.aspx) в отдельном представлении, чтобы пользователи могли перекрестно ссылаться на информацию в одном или нескольких сообщениях.

- [Сделайте запросы EWS](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) на сервер Exchange, на котором размещается почтовый ящик пользователя. Почтовое приложение может, например, получить список папок, чтобы пользователь мог выбрать одну из них для хранения сообщения или Показать все элементы в беседе или пометить сообщение электронной почты как нежелательное.

- [Получите маркер](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) для уникальной идентификации учетной записи электронной почты, чтобы включить единый вход в сторонней службе.

- [Получение маркера](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx) , который позволяет сторонней службе выполнять запросы EWS от имени пользователя, например, для извлечения вложений из элемента или получения элемента с сервера Exchange для дальнейшей обработки.

Вы можете использовать почтовые приложения, чтобы настроить взаимодействие с Outlook Web App для пользователей; Однако, если вы хотите настроить внешний вид и поведение Outlook Web App, ознакомьтесь со статьями на сайте TechNet:

- [Создание темы для приложения Outlook Web App](http://technet.microsoft.com/en-us/library/bb201700%28v=exchg.150%29.aspx)

- [Настройка страниц входа, выбора языка и ошибок в Outlook Web App](http://technet.microsoft.com/en-us/library/ee633483%28v=exchg.150%29.aspx)

Ваша организация может устанавливать почтовые приложения на внутреннем сервере, чтобы ограничить доступ к авторизованным пользователям, а другие разработчики почтовых приложений могут помещать почтовые приложения в [магазин Office](http://office.microsoft.com/store/) для продажи в общедоступной общедоступной сети. Все, кто работает с Outlook, могут скачивать, устанавливать и использовать почтовые приложения из Marketplace.

Если вы хотите узнать больше о создании почтовых приложений, ознакомьтесь с [документацией по надстройкам Outlook](/outlook/add-ins) или [сделайте пример запроса EWS](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Outlook-Make-770b2528) .

## <a name="ews-and-outlook-add-ins"></a>Надстройки EWS и Outlook

Вы можете использовать подмножество операций EWS на сервере Exchange, на котором размещается учетная запись, на которой выполняется почтовое приложение.

Функция [Mailbox. makeEwsRequestAsync](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx) позволяет ОТПРАВЛЯТЬ запросы EWS из почтового приложения обратно на сервер, на котором размещается почтовый ящик пользователя. Вы создаете конверт SOAP и запрос XML, а функция **makeEwsRequestAsync** вызывает EWS с помощью маркера проверки подлинности, определяющего почтовый ящик и почтовое приложение, которое делает запрос. Чтобы обеспечить безопасность почтового ящика пользователя, сервер Exchange Server отклоняет все запросы, которые не поступают из почтового приложения или из почтового ящика, не размещенного на сервере.

Как и для любого другого приложения, почтовому приложению требуется разрешение на работу. Администратору необходимо выполнить указанные ниже действия.

- [Предоставьте доступ](controlling-client-application-access-to-ews-in-exchange.md) к службам EWS пользователю почтовых приложений.

- [Присвойте параметру "OAuthAuthentication" значение true](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx) в каталоге Client Access Server EWS.

Кроме того, необходимо убедиться, что ваше приложение запрашивает разрешение на чтение и запись почтового ящика в [модели разрешений](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)приложений для Office.

После выполнения этих действий для почтового приложения будут доступны подмножество операций с папками и элементами EWS.

**Таблица 1. Операции с папками и элементами EWS, которые могут использовать почтовые приложения**

|**Операции с папками**|**Операции с элементами**|
|:-----|:-----|
|[Операция CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [Операция FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [Операция GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [Операция UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |[Операция CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [Операция CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [Операция FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> [Операция FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> [Операция GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> [Операция GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [Операция MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) <br/> [Операция MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [Операция SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> [Операция UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |

### <a name="service-callback-tokens"></a>Маркеры обратного вызова службы

Маркеры обратного вызова службы позволяют почтовым приложениям передавать маркер доступа сторонней службе, чтобы служба могла отправлять запросы EWS на сервер Exchange, на котором размещается почтовый ящик. Например, почтовое приложение может передать маркер обратного вызова службы сторонней службе, а также список идентификаторов вложений для изображений, вложенных в сообщение электронной почты. Затем служба может использовать идентификаторы вложений и маркер обратного вызова, чтобы отправить запрос EWS на сервер Exchange пользователя для получения вложенных изображений. Почтовые приложения также могут использовать токен обратного вызова службы со списком идентификаторов элементов для получения электронной почты и элементов встреч с сервера Exchange.

Маркер обратного вызова службы — это непрозрачный маркер, который служба стороннего разработчика присоединяется к запросу EWS в заголовке проверки подлинности носителя. Маркер определяет почтовое приложение и почтовый ящик для защиты запроса EWS. Чтобы узнать, как использовать маркеры обратного вызова службы, ознакомьтесь с разделом [надстройки Outlook: получение вложений из примера сервера Exchange Server](http://code.msdn.microsoft.com/exchange/Mail-apps-for-Office-Get-38babdc9) .

## <a name="see-also"></a>См. также


- [Управление доступом клиентских приложений к EWS в Exchange](controlling-client-application-access-to-ews-in-exchange.md)

- [Метод Mailbox.makeEwsRequestAsync (API JavaScript для Office)](http://msdn.microsoft.com/library/2ec380e0-4a67-4146-92a6-6a39f65dc6f2%28Office.15%29.aspx)

- [Надстройки Outlook](https://docs.microsoft.com/outlook/add-ins)

- [Метод Mailbox.getUserIdentityTokenAsync (API JavaScript для Office)](http://msdn.microsoft.com/library/c658518b-6867-41a0-99cf-810303e4c539%28Office.15%29.aspx)

- [Проверка подлинности надстройки Outlook с помощью маркеров удостоверения Exchange](http://msdn.microsoft.com/library/c0520a1e-d9ba-495a-a99f-6816d7d2a23e%28Office.15%29.aspx)

- [Общие сведения о разрешениях для надстроек Outlook](https://docs.microsoft.com/en-us/outlook/add-ins/understanding-outlook-add-in-permissions)

- [Set — Webservicesvirtualdirectory используется](http://technet.microsoft.com/en-us/library/aa997233%28v=exchg.150%29.aspx)

- [Надстройки Outlook: Создание запроса EWS](http://code.msdn.microsoft.com/office/Mail-apps-for-Outlook-Make-770b2528)

- [Надстройки Outlook: использование маркера удостоверения клиента](http://code.msdn.microsoft.com/Mail-apps-for-Outlook-Use-b20a66b6)

- [Надстройки Outlook: получение вложений с сервера Exchange Server](http://code.msdn.microsoft.com/office/Mail-apps-for-Office-Get-38babdc9)
