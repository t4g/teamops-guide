
<div hidden>
  ```
@startuml firstDiagram
!include <logos/mattermost>
!include <logos/github>
!include <logos/slack>
!include <logos/azure>
!include <logos/zapier>
!theme materia-outline
title Using both Code Foundation and Github 



queue "<$azure>\nfoundations\n*Pull request*" as tfpr
queue "<$github>\nPull request" as ghpr
rectangle "<$zapier>\nzapier" as z
rectangle "<$mattermost>\nmattermost" as mm
rectangle "<$github>\npages" as ghp

tfpr -> z
z <- ghpr
z --> mm
mm --> ghp


@enduml
  ```
</div>
![](firstDiagram.svg)
