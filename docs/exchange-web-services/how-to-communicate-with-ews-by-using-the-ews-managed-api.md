---
title: Взаимодействие с EWS с помощью управляемого API EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: d1b78293-da02-413a-875c-681e99146af3
description: Сведения о том, как использовать управляемый API EWS для связи с EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: be807f2d936bf79d181476ec8eb12f20fca7950f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528246"
---
# <a name="communicate-with-ews-by-using-the-ews-managed-api"></a>Взаимодействие с EWS с помощью управляемого API EWS

Сведения о том, как использовать управляемый API EWS для связи с EWS в Exchange.
  
Класс [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS содержит методы и свойства, которые используются для задания учетных данных пользователя, определения КОНЕЧНОЙ точки EWS, отправки и получения сообщений SOAP, а также для настройки привязки для связи с EWS. Прежде чем использовать управляемый API EWS для выполнения любой задачи, необходимо создать экземпляр класса **ExchangeService** и связать его с EWS. 
  
После настройки объекта [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) с помощью учетных данных пользователя и КОНЕЧНОЙ точки EWS любой объект почтового ящика, ссылающийся на объект [ExchangeService](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.aspx) , может использовать следующие типы методов для общения с EWS: 
  
- Методы объекта ExchangeService — все методы объекта **ExchangeService** , которые не наследуются от базового типа **объекта** , выполняют вызовы EWS. 
    
- Методы элементов и типов папок почтового ящика Exchange.
    
**Таблица 1. Методы и типы папок почтового ящика, взаимодействующие с EWS**

|Method|Действие|Вызываемые операции|
|:-----|:-----|:-----|
|[Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.load%28v=exchg.80%29.aspx) <br/> |Получает свойства элемента, вложения или объекта конфигурации пользователя.  <br/> |[Операция GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/><br/> [Операция GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/><br/> [Операция GetUserConfiguration](https://msdn.microsoft.com/library/71d50e3c-92bd-435f-8118-b28bb85f8138%28Office.15%29.aspx) <br/> |
|[Базу](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |Заполняет новый элемент на клиенте сведениями из существующего элемента на сервере.  <br/> |[Операция GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.save%28v=exchg.80%29.aspx) <br/> |Сохраняет копию клиентского элемента на сервере.  <br/> |[Операция UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/> [Операция UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/><br/>[Операция CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/><br/>[Операция CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|[Обновление](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> |Обновляет сервер с учетом изменений, внесенных в клиенте.<br/><br/>Для элементов и папок метод **Update** использует [операцию UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) и [операцию операцию UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx).  <br/> |[Операция UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/><br/>[Операция UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|[Удаление](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> |Удаляет элемент на сервере.<br/><br/>Для элементов и папок метод **Delete** использует [операцию и DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx).  <br/> |[Операция DeleteItem](https://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/><br/> [Операция DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |
|[Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> |Создает копию элемента или папок на сервере.  <br/> |[Операция CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/><br/> [Операция CopyFolder](https://msdn.microsoft.com/library/c7ea0d68-9793-4144-b378-d99536776db9%28Office.15%29.aspx) <br/> |
|[Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> |Перемещает элементы или папки на сервере.  <br/> |[Операция MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/><br/> [Операция MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
## <a name="to-use-the-ews-managed-api-to-communicate-with-ews"></a>Использование управляемого API EWS для общения с EWS

1. Создайте экземпляр класса **ExchangeService** . 
    
   ```csharp
    ExchangeService service = new ExchangeService();
   ```

   > [!NOTE]
   > При создании экземпляра **ExchangeService** с пустым конструктором будет создан экземпляр, привязанный к последней известной версии Exchange. Кроме того, вы можете ориентироваться на определенную версию Exchange, указав в качестве параметра версию Version. `ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2007_SP1);`
  
2. Задайте учетные данные пользователя, который отправляет запросы на сервер Exchange. Если вы хотите подключиться к EWS с компьютера, выполнившего вход в домен, используя учетные данные пользователя, прошедшего проверку подлинности, присвойте свойству **уседефаулткредентиалс** объекта **ExchangeService** **значение true**.
    
   ```cs
    // Connect by using the default credentials of the authenticated user.
    service.UseDefaultCredentials = true;
   ```

   Если вы не хотите подключаться с помощью учетных данных пользователя по умолчанию, задайте для свойства **Credentials** объекта **ExchangeService** явное указание учетных данных другого пользователя. Если вы используете Exchange Online или Exchange Online в составе Office 365, вы будете использовать обычную проверку подлинности с использованием только имени пользователя и пароля. Для проверки подлинности NTLM необходимо указать имя домена. 
    
   ```cs
    // Connect by using the credentials of user1 at contoso.com.
    service.Credentials = new WebCredentials("user1@contoso.com", "password");
   ```

   Вы также можете указать учетные данные пользователя, используя доменное имя пользователя и пароль.
    
   ```cs
    // Connect by using the credentials of contoso/user1.
    service.Credentials = new WebCredentials("user1", "password", "contoso");
   ```

   > [!NOTE]
   > Если для свойства **уседефаулткредентиалс** задано значение **true**, то значение свойства **Credentials** игнорируется. 
  
3. Задайте URL-адрес конечной точки EWS. Этот URL-адрес определяет расположение файла Exchange. asmx на сервере клиентского доступа.
    
   ```cs
    // Use Autodiscover to set the URL endpoint.
    service.AutodiscoverUrl("user1@contoso.com");
   ```

   > [!NOTE]
   >  Несмотря на то, что вы можете явно задать для свойства **URL** **ExchangeService** значение жестко заданное значение, рекомендуется использовать службу автообнаружения по следующим причинам: > служба автообнаружения определяет наилучшую конечную точку для определенного пользователя (конечная точка, ближайшую к серверу почтовых ящиков пользователей). > URL-адрес EWS может измениться при развертывании новых серверов клиентского доступа. В этом сценарии использование [автообнаружения](autodiscover-for-exchange.md) означает, что не требуется вносить изменения в код. > необходимо явно задать URL-адрес или вызвать **AutodiscoverUrl**, но не делать и то, и другое. 
  
## <a name="see-also"></a>См. также

- [Начало работы с клиентскими приложениями, использующими управляемый API EWS](get-started-with-ews-managed-api-client-applications.md) 
- [Поиск точек соединения с помощью службы автообнаружения](how-to-use-autodiscover-to-find-connection-points.md)   
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    

