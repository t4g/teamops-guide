PlantUML
========

[![GitHub Sponsors](https://img.shields.io/github/sponsors/plantuml?logo=github)](https://github.com/sponsors/plantuml/)
[![GitHub Org's stars](https://img.shields.io/github/st
































































































































































































































































































































































Orange Stack
========

[![GitHub Sponsors](https://img.shields.io/github/sponsors/plantuml?logo=github)](https://github.com/sponsors/plantuml/)
[![GitHub Org's stars](https://img.shields.io/github/stars/plantuml)](https://github.com/t4g/teamops-guide/stargazers/)
[![GitHub watchers](https://img.shields.io/github/watchers/plantuml/plantuml)](https://github.com/t4g/teamops-guide/)
[![GitHub contributors](https://img.shields.io/github/contributors-anon/plantuml/plantuml?color=blue)](https://github.com/t4g/teamops-guide/graphs/contributors)
[![GitHub forks](https://img.shields.io/github/forks/plantuml/plantuml)](https://github.com/t4g/teamops-guide/network/)
[![GitHub all releases](https://img.shields.io/sourceforge/dt/plantuml?color=blue)](https://github.com/t4g/teamops-guide/releases)

[![rate](https://img.shields.io/endpoi]
[![Release (latest by date)](https://img.shields.io/github/v/release/t4g/teamops-guide)](https://github.com/t4g/teamops-guide/releases/latest)
[![Release Date](https://img.shields.io/github/release-date/t4g/teamops-guide?color=blue)](https://github.com/t4g/teamops-guide/releases/latest)
[![GitHub commits since latest release (by date)](https://img.shields.io/github/commits-since/t4g/teamops-guide/latest)](https://github.com/t4g/teamops-guide/commits/)

[![Pre-release (latest by date)](https://img.shields.io/github/v/release/t4g/teamops-guide?color=chocolate&include_prereleases)](https://github.com/t4g/teamops-guide/releases/tag/snapshot)
[![Pre-release Date](https://img.shields.io/github/release-date-pre/t4g/teamops-guide?color=chocolate)](https://github.com/t4g/teamops-guide/releases/tag/snapshot)
[![GitHub last commit](https://img.shields.io/github/last-commit/t4g/teamops-guide?color=chocolate)](https://github.com/t4g/teamops-guide/commits/)


# The Orange Stack

@startuml
queue "<$github>\nPull request" as ghpr
@enduml

# Switching mattermost for Slack

Below are a few differences when maintaining the orange stack

@startuml
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


























