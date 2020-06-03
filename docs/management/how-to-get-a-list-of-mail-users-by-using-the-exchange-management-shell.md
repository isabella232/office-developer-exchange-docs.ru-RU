---
title: Получение списка пользователей почты с помощью командной консоли Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.assetid: 8b790dc8-5c4f-4acf-bbe7-63523395fbe7
description: Использование командлетов командной консоли Exchange для создания инструмента, который возвращает список пользователей почтового ящика Exchange
localization_priority: Priority
ms.openlocfilehash: 817d92ef1bb88017f471681b448c052ecaa54e7e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435711"
---
# <a name="get-a-list-of-mail-users-by-using-the-exchange-management-shell"></a>Получение списка пользователей почты с помощью командной консоли Exchange

Использование командлетов командной консоли Exchange для создания инструмента, который возвращает список пользователей почтового ящика Exchange
  
**Применимо к:** Exchange Online | Exchange Server 2013 | Office 365 
  
Получение списка пользователей из Exchange Online, Exchange Online в составе Office 365 или версий Exchange начиная с Exchange 2013 с помощью управляемого инструмента для вызова командлета командной консоли Exchange — это двухэтапный процесс. Сначала необходимо создать удаленное пространство выполнения на сервере Exchange, а затем запустить командлет для получения сведений о пользователях в удаленном пространстве выполнения. 

Для подключения к удаленному пространству выполнения необходимо пройти проверку подлинности на сервере Exchange согласно схеме, принятой в соответствии с требованиями безопасности вашей организации. 

В этой статье приведены примеры кодов, которые можно использовать для создания удаленного пространства выполнения, запуска командлета командной консоли Exchange и получения списка пользователей с сервера Exchange.

<a name="bk_prerequisites"> </a>

## <a name="prerequisites-for-getting-a-list-of-mailbox-users"></a>Необходимые условия для получения списка пользователей почтового ящика

Для выполнения этой задачи требуется ссылка на следующие пространства имен:
  
- **System. Collections. ObjectModel**
- **System. Management. Automation**
- **System. Management. Automation. Remoting**
- **System. Management. Automation. пространства**
    
> [!NOTE]
>  При создании приложения с помощью Visual Studio необходимо добавить к проекту ссылку на сборку System.Management.Automation.dll. Найти сборку можно, пройдя по одной из следующих ссылок:
> - Для ОС Windows XP и Windows Vista — каталог установки Windows PowerShell ($PSHOME).
> - Для ОС Windows 7 и Windows 8 — папка Windows\assembly\GAC_MSIL\System.Management.Automation. 
  
Не загружайте оснастку управления Exchange 2013 в пространство выполнения на компьютерах, где запущены приложения, автоматизирующие командлеты командной консоли Exchange. Вместо этого приложение должно создать удаленное пространство выполнения так, как будет описано ниже.

<a name="bk_gettinglistmailbox"> </a>

## <a name="connect-to-a-remote-runspace-on-an-exchange-server"></a>Создание удаленного пространства выполнения на сервере Exchange

Метод подключения к удаленному пространству выполнения, в котором будет использован командлет командной консоли Exchange, зависит от выбранной схемы проверки подлинности. В этом разделе приведены примеры кодов для подключения к удаленному пространству выполнения при использовании одного из методов проверки подлинности, перечисленных в таблице ниже.
  
|**Метод проверки подлинности**|**Относится к**|**URI**|
|:-----|:-----|:-----|
|[Подключение к удаленному пространству выполнения на сервере Exchange Online с помощью обычной проверки подлинности](#bk_basic) <br/> |Серверы Exchange Online  <br/> |`https://outlook.office365.com/PowerShell-LiveID`<br/><br/>`https://<server>/PowerShell-LiveID`  <br/> |
|[Подключение к удаленному пространству выполнения с помощью проверки подлинности на основе сертификата](#bk_cert) <br/> |Серверы Exchange Online и локальные серверы Exchange  <br/> |`https://outlook.office365.com/PowerShell`<br/><br/>`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |
|[Подключение к удаленному пространству выполнения на сервере Exchange с помощью проверки подлинности Kerberos](#bk_Kerberos) <br/> |Серверы Exchange Online и локальные серверы Exchange  <br/> |`https://<server>/PowerShell`<br/><br/>`http://<server>/PowerShell`  <br/> |

<a name="bk_basic"> </a>

### <a name="connect-to-a-remote-runspace-on-exchange-online-by-using-basic-authentication"></a>Подключение к удаленному пространству выполнения на сервере Exchange Online с помощью обычной проверки подлинности

Следующий код определяет метод **GetUsersUsingBasicAuth**, с помощью которого на удаленном сервере Exchange Online создается пространство выполнения для командной консоли Exchange с помощью обычной проверки подлинности. Затем этот метод вызывает **GetUserInformation**, как это описано в разделе [Получение списка пользователей почтового ящика из удаленного пространства](#bk_remote), для возврата списка пользователей на удаленном сервере.
  
Для этого метода требуются следующие параметры:
  
-  **ливеидконнектионури** &ndash; Строка, содержащая универсальный код ресурса (URI) сервера Exchange Online, который будет выполнять проверку подлинности для приложения. Если Exchange Online работает в Office 365, URI имеет значение `https://outlook.office365.com/PowerShell-LiveID` ; в противном случае — URI `https://<servername>/PowerShell-LiveID` . 
    
-  **счемаури** &ndash; Строка, содержащая URI документа схемы, который определяет схему командной консоли Exchange. URI схемы `https://schemas.microsoft.com/powershell/Microsoft.Exchange` . 
    
-  **учетные данные** &ndash; Объект [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) , содержащий учетные данные пользователя, запустившего приложение. 
    
-  **Count (количество** &ndash; ) Число возвращаемых пользователей почтовых ящиков Exchange. 
    
```cs
public Collection<PSObject> GetUsersUsingBasicAuth(
    string liveIDConnectionUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(liveIDConnectionUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingBasicAuth( _
    ByVal LiveIDConnectionUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(LiveIDConnectionUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Basic
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<a name="bk_cert"> </a>

### <a name="connect-to-a-remote-runspace-by-using-certificate-authentication"></a>Подключение к удаленному пространству выполнения с помощью проверки подлинности на основе сертификата

Следующий код определяет метод **GetUsersUsingCertificate**, с помощью которого на удаленном сервере Exchange Online создается пространство выполнения для командной консоли Exchange с помощью проверки подлинности на основе сертификата. Затем этот метод вызывает **GetUserInformation**, как это описано в разделе [Получение списка пользователей почтового ящика из удаленного пространства](#bk_remote), для возврата списка пользователей на удаленном сервере.
  
Для этого метода требуются следующие параметры:
  
-  **Thumbprint (отпечаток** &ndash; ) Строка, содержащая отпечаток сертификата, используемого для проверки подлинности приложения. 
    
-  **цертконнектионури** &ndash; Строка, содержащая универсальный код ресурса (URI) сервера, который будет выполнять проверку подлинности сертификата. Необходимо использовать один из универсальных кодов, приведенных в таблице ниже. 
    
    **Таблица 1. URI Цертконнектионури**

    |**Server**|**URI**|
    |:-----|:-----|
    |Сервер Exchange, не использующий протокол SSL  <br/> |`http://<servername>/PowerShell`  <br/> |
    |Сервер Exchange, использующий протокол SSL  <br/> |`https://<servername>/PowerShell`  <br/> |
    |Exchange Online в составе Office 365  <br/> |`https://outlook.office365.com/PowerShell`  <br/> |
   
- **счемаури** &ndash; Строка, содержащая URI документа схемы, который определяет схему командной консоли Exchange. URI схемы https://schemas.microsoft.com/powershell/Microsoft.Exchange . 
    
- **Count (количество** &ndash; ) Число возвращаемых пользователей почтовых ящиков Exchange. 
    
```cs
public Collection<PSObject> GetUsersUsingCertificate(
    string thumbprint, string certConnectionUri, string schemaUri, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(certConnectionUri),
        schemaUri,
        thumbprint)
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```


```vb
  Function GetUsersUsingCertificate( _
    ByVal Thumbprint As String, ByVal CertConnectionUri As String, _
    ByVal SchemaUri As String, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo
    ConnectionInfo = New WSManConnectionInfo(New Uri(CertConnectionUri), SchemaUri, Thumbprint)
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<a name="bk_Kerberos"> </a>

### <a name="connect-to-a-remote-runspace-on-an-exchange-server-by-using-kerberos-authentication"></a>Подключение к удаленному пространству выполнения на сервере Exchange с помощью проверки подлинности Kerberos

Следующий код определяет метод **GetUsersUsingKerberos**, с помощью которого на удаленном сервере создается пространство выполнения для командной консоли Exchange с помощью проверки подлинности Kerberos. Затем этот метод вызывает **GetUserInformation**, как это описано в разделе [Получение списка пользователей почтового ящика из удаленного пространства](#bk_remote), для возврата списка пользователей на удаленном сервере.
  
Для этого метода требуются следующие параметры:
  
- **керберосури** &ndash; Строка, содержащая URI сервера Kerberos, который будет выполнять проверку подлинности для приложения. Необходимо использовать один из универсальных кодов, приведенных в таблице ниже. 
    
    **Таблица 2. URI Керберосури**

    |**Server**|**URI**|
    |:-----|:-----|
    |Сервер Exchange, не использующий протокол SSL  <br/> |`http://<servername>/PowerShell`  <br/> |
    |Сервер Exchange, использующий протокол SSL  <br/> |`https://<servername>/PowerShell`  <br/> |
   
- **счемаури** &ndash; Строка, содержащая URI документа схемы, который определяет схему командной консоли Exchange. URI схемы https://schemas.microsoft.com/powershell/Microsoft.Exchange . 
    
- **учетные данные** &ndash; Объект [PSCredential](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) , содержащий учетные данные пользователя, запустившего приложение. 
    
- **Count (количество** &ndash; ) Число возвращаемых пользователей почтовых ящиков Exchange. 
    
```cs
public Collection<PSObject> GetUsersUsingKerberos(
    string kerberosUri, string schemaUri, PSCredential credentials, int count)
{
    WSManConnectionInfo connectionInfo = new WSManConnectionInfo(
        new Uri(kerberosUri),
        schemaUri, credentials);
    connectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos;
    using (Runspace runspace = RunspaceFactory.CreateRunspace(connectionInfo))
    {
        return GetUserInformation(count, runspace);
    }
}
```

```vb
  Function GetUsersUsingKerberos( _
    ByVal KerberosUri As String, ByVal ScehmaUri As String, _
    ByVal Credentials As PSCredential, ByVal Count As Integer) As Collection(Of PSObject)
    Dim ConnectionInfo As WSManConnectionInfo = _
        New WSManConnectionInfo(New Uri(KerberosUri), ScehmaUri, Credentials)
    ConnectionInfo.AuthenticationMechanism = AuthenticationMechanism.Kerberos
    Dim RemoteRunspace As Runspace
    RemoteRunspace = RunspaceFactory.CreateRunspace(ConnectionInfo)
    Return GetUserInformation(Count, RemoteRunspace)
  End Function

```

<a name="bk_remote"> </a>

## <a name="get-a-list-of-mailbox-users-from-a-remote-runspace"></a>Получение списка пользователей почтового ящика из удаленного пространства

В следующем примере кода определяется метод **жетусеринформатион** , который возвращает коллекцию экземпляров [PSObject](https://msdn.microsoft.com/library/system.management.automation.pscredential%28VS.85%29.aspx) , представляющих пользователей почтовых ящиков Exchange. Этот метод вызывается с помощью методов **GetUsersUsingBasicAuth**, **GetUsersUsingCertificate** и **GetUsersUsingKerberos** для возврата списка пользователей на удаленном сервере. 
  
Для этого метода требуются следующие параметры:
  
- **Count (количество** &ndash; ) Число возвращаемых пользователей почтовых ящиков Exchange. 
    
- **пространство выполнения** &ndash; Удаленное пространство выполнения, установленное для удаленного сервера Exchange. 
    
```cs
public Collection<PSObject> GetUserInformation(int count, Runspace runspace)
{
    using (PowerShell powershell = PowerShell.Create())
    {
        powershell.AddCommand("Get-Users");
        powershell.AddParameter("ResultSize", count);
        runspace.Open();
        powershell.Runspace = runspace;
        return powershell.Invoke();
    }
}
```

```vb
Function GetUserInformation(ByVal Count As Integer, ByVal RemoteRunspace As Runspace) As Collection(Of PSObject)
    Dim RemotePowerShell As PowerShell = PowerShell.Create
    RemotePowerShell.AddCommand("Get-Users")
    RemotePowerShell.AddParameter("ResultSize", Count)
    ' Open the remote runspace on the server.
    RemoteRunspace.Open()
    ' Associate the runspace with the Exchange Management Shell.
    RemotePowerShell.Runspace = RemoteRunspace
    ' Invoke the Exchange Management Shell to run the command.
    Return RemotePowerShell.Invoke
End Function

```

Метод **жетусеринформатион** будет возвращать не больше, чем _количество_ пользователей почтовых ящиков. Чтобы упростить код в этом примере, не выполняется фильтрация либо же другим способом ограничивается количество возвращаемых пользователей. 
  
## <a name="see-also"></a>См. также

- [Создание средств командной консоли Exchange](create-exchange-management-shell-tools.md)   
- [Использование ответа командлета командной консоли Exchange](how-to-use-the-exchange-management-shell-cmdlet-response.md)
    

