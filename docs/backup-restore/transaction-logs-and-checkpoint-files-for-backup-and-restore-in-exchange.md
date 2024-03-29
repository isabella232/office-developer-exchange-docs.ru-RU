---
title: Журналы транзакций и файлы контрольно-пропускных пунктов для резервного копирования и восстановления в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 80e04b9f-87c7-4acf-89b1-aa66ffaf7e53
description: Сведения о журналах транзакций и файлах контрольно-пропускных пунктов, а также об их Exchange данных за 2013 год.
ms.openlocfilehash: ae47c7757a1001f28c467ea58ec87b4ddbc5a5c4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513264"
---
# <a name="transaction-logs-and-checkpoint-files-for-backup-and-restore-in-exchange"></a>Журналы транзакций и файлы контрольно-пропускных пунктов для резервного копирования и восстановления в Exchange

Сведения о журналах транзакций и файлах контрольно-пропускных пунктов, а также об их Exchange данных за 2013 год.
  
**Применяется к:** Exchange Server 2013 г. 
  
В этой статье описывается, Exchange Server 2013 г. для предотвращения потери данных используются журналы транзакций и файлы контрольно-пропускных пунктов. Важно знать об этой информации при разработке приложений резервного копирования и восстановления, которые используют службу копирования теней тома (VSS) в версиях Windows Server, начиная с Windows Server 2008.
  
## <a name="transaction-logs-in-exchange-2013"></a>Журналы транзакций в Exchange 2013 г.

Exchange 2013 поддерживает один набор файлов журнала транзакций для каждой базы данных. Транзакция определяется как любая операция, которая изменяет состояние или содержимое базы данных. Файлы журнала транзакций для отдельной базы данных записывают все транзакции, выполняемые в базе данных. Записи транзакций записывают в журналы транзакций, прежде чем они будут сделаны в самой базе данных, чтобы обеспечить восстановление всех совершенных транзакций в случае сбоя базы данных. Exchange 2013 г. журналы транзакций баз данных хранятся на диске до совершения транзакций в файле базы данных. 
  
Запись транзакций перед обновлением базы данных называется ведением журнала заранее. Чтобы обеспечить правильное состояние базы данных, Exchange 2013 г. записывает данные в файлы баз данных с помощью записей и контрольно-пропускных пунктов на основе страниц. Во время регулярных операций Exchange сначала регистрирует изменения базы данных в журналах транзакций, а затем вносит эти изменения в копию базы данных в памяти. Журналы транзакций записывают начало и конец каждой транзакции. Это обеспечивает доступ к достаточной информации для более поздней отмены или отката операций в базе данных.
  
При восстановлении ошибок, при которых файл базы данных на диске поврежден, но журналы транзакций не повреждены, приложение восстановления должно сначала восстановить известные хорошие копии файла базы данных.
  
В Exchange хранится повтор транзакций из ранее архивных журналов транзакций, а затем повторяются все оставшиеся транзакции из файлов журнала транзакций на диске. Обратите внимание, что иногда транзакции могут быть потеряны, если система не работает между записью транзакций в журналах транзакций и записью их в файлы базы данных. 
  
Периодически в Exchange проверяется изображение базы данных в памяти, а затем определяется, какие страницы изменились. Хранилище Exchange объединяет ожидающих изменений, а затем записывает эти страницы в файл базы данных на диске.
  
## <a name="checkpoint-files-in-exchange-2013"></a>Файлы контрольно-пропускных Exchange 2013 г.

Записи файлов контрольно-пропускных пунктов, в которых регистрируются транзакции, были записаны в файлы базы данных на диске. Эта контрольно-пропускная точка будет усовершенствована, когда все страницы базы данных, измененные записями в журналах транзакций, успешно записаны на диск. Так как записи файлов контрольно-пропускных пунктов, транзакции которых уже находятся на изображении базы данных на диске, Exchange хранилище должно только повторить транзакции, которые произошли после контрольно-пропускного пункта. В зависимости от периода времени между резервными копиями это может значительно уменьшить количество транзакций, которые необходимо повторить в базе данных в случае сбоя системы.
  
## <a name="see-also"></a>См. также

- [Концепции резервного копирования и восстановления Exchange 2013 г.](backup-and-restore-concepts-for-exchange-2013.md)
- [Типы операций резервного копирования Exchange 2013 г.](types-of-backup-operations-for-exchange-2013.md)
- [Восстановление Exchange 2013 г.](restoring-exchange-2013-databases.md)
    

