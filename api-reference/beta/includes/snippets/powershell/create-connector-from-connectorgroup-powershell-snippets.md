---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
	"@odata.id" = "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
}

New-MgOnPremisePublishingProfileConnectorGroupMemberByRef -OnPremisesPublishingProfileId $onPremisesPublishingProfileId -ConnectorGroupId $connectorGroupId -BodyParameter $params

```