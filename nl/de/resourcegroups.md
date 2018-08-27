---



copyright:

  years: 2017, 2018
lastupdated: "2018-08-02"


---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:tip: .tip}
{:new_window: target="_blank"}

# Ressourcengruppen verwalten
{: #rgs}

Ressourcengruppen bieten Ihnen die Möglichkeit, Ihre Kontoressourcen in anpassbaren Gruppierungen zu organisieren, sodass Sie den Benutzern schnell Zugriff auf mehrere Ressourcen gleichzeitig zuordnen können. Jede Kontoressource, die mit der Zugriffssteuerung von {{site.data.keyword.Bluemix}} Identity and Access Management (IAM) verwaltet wird, gehört zu einer Ressourcengruppe innerhalb Ihres Kontos. Cloud Foundry-Services bleiben den Organisationen und Bereichen zugewiesen und können nicht zu einer Ressourcengruppe hinzugefügt werden.

Um mit dem Verwalten Ihrer Ressourcengruppen zu beginnen, rufen Sie an der {{site.data.keyword.Bluemix}}-Konsole die Optionen **Verwalten** &gt; **Konto** &gt; **Ressourcengruppen** auf. Dort können Sie Ihre Ressourcengruppen anzeigen, umbenennen und neue Ressourcengruppen erstellen. Weitere Informationen zur Arbeit mit Ressourcengruppen finden Sie unter [Bewährte Verfahren für die Organisation von Ressourcen in Ressourcengruppen](/docs/resources/bestpractice_rgs.html#bp_resourcegroups).


## Ressourcengruppe erstellen

Wenn Sie über ein nutzungsabhängiges Konto oder ein Abonnementkonto verfügen, dann können Sie mehrere Ressourcengruppen erstellen, um auf einfache Weise Kontingente zu verwalten und die Informationen zu Abrechnung und Nutzung für ein Ressourcenset anzuzeigen. Durch die Gruppierung von Ressourcen wird außerdem die gleichzeitige Zuweisung von Zugriffsberechtigungen für mehrere Instanzen an die Benutzer erleichtert. Beachten Sie, dass Sie eine Ressourcengruppe umbenennen, jedoch keine Ressourcengruppe nach der Erstellung löschen können.

Wenn Sie über ein Lite-Konto oder ein 30-Tage-Testkonto verfügen, können Sie zwar keine zusätzlichen Ressourcengruppen erstellen, jedoch die Standardressourcengruppe umbenennen.

Die einzelnen Ressourcengruppen sind kostenfrei, die Verbindungen zwischen einer Ressourcengruppe und einer Cloud Foundry-Organisation oder einem Cloud Foundry-Bereich werden jedoch bei Ihrem Kontokontingent angerechnet. Weitere Informationen finden Sie in [Was ist ein Alias?](/docs/resources/connecting_apps.html#what_is_alias).
{: tip}

1. Rufen Sie **Verwalten** &gt; **Konto** &gt; **Ressourcengruppen** auf.
2. Klicken Sie auf **Ressourcengruppe erstellen**.
3. Geben Sie einen Namen für Ihre Ressourcengruppe ein.
4. Klicken Sie auf **Hinzufügen**.

## Ressourcen zu einer Ressourcengruppe hinzufügen

Services, die mit IAM verwaltet werden, gehören nicht zu einer Organisation oder einem Bereich von Cloud Foundry, sondern zu einer Ressourcengruppe. Wenn Sie eine Serviceinstanz für einen dieser Services aus dem Katalog erstellen, werden Sie aufgefordert, die Instanz einer Ressourcengruppe zuzuweisen. Ihre Ressourcengruppenauswahl bei der Erstellung der Instanz ist endgültig und kann nicht geändert werden.

## Ressourcen in Ressourcengruppen anzeigen

Um die Ressourcen, die in einer Ressourcengruppe enthalten sind, auf einfache Weise anzeigen zu können, müssen Sie die Informationen über das Dashboard nach Ressourcengruppen filtern.

## Ressourcengruppe umbenennen

Ihre erste Ressourcengruppe wird vom System für Sie erstellt und erhält den Namen `Standard`. Sie können auswählen, ob der Name dieser Gruppe oder anderer Gruppen, die Sie erstellen, aktualisiert werden soll.

1. Rufen Sie **Verwalten** &gt; **Konto** &gt; **Ressourcengruppen** auf.
2. Klicken Sie auf **Umbenennen**.
3. Geben Sie einen eindeutigen Namen ein und klicken Sie auf **Speichern**.

## Ressourcengruppen und Ressourcen mit der {{site.data.keyword.Bluemix_notm}}-CLI verwalten

Von der {{site.data.keyword.Bluemix_notm}}-Befehlszeilenschnittstelle werden mehrere Befehle für das Ressourcenmanagement unterstützt. Weitere Informationen finden Sie unter [Befehle zum Verwalten von Ressourcengruppen und Ressourcen](/docs/cli/reference/ibmcloud/cli_resource_group.html#ibmcloud_commands_resource).

## Zugriff auf eigene Ressourcengruppen verwalten

Cloud IAM ermöglicht Ihnen die flexible Bereitstellung eines genau differenzierten Benutzerzugriffs auf die Ressourcen in Ihrem Konto. Sie können Cloud IAM dazu verwenden, Benutzern Richtlinien zuzuweisen, die den Benutzerzugriff auf alle Ressourcen einer Ressourcengruppe, auf einen einzelnen Servicetyp in einer Ressourcengruppe oder auf eine einzelne Serviceinstanz im Konto bereitstellen. Wird Benutzern Zugriff auf Ressourcen in einer Ressourcengruppe zur Verfügung gestellt, so bedeutet dies nicht, dass diesen Benutzer auch die Zugriffsberechtigungen zur Verwaltung der Ressourcengruppe selbst erteilt werden. Sie können den Zugriff auf die Funktionen zum Anzeigen, Bearbeiten und Verwalten der eigentlichen Ressourcengruppe separat definieren.

Weitere Informationen finden Sie unter [IAM-Zugriff verwalten](/docs/iam/mngiam.html#iammanidaccser).
