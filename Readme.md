Dokumentation
# Open Data-Workflows

[Robert Koch-Institut](https://rki.de) | RKI  
Nordufer 20  
13353 Berlin

[Fabian Eckelmann](https://github.com/eckelmannf)
[Knut Perseke](https://github.com/eckelmannf)
[Hannes Wuensche](https://orcid.org/0000-0002-8837-0326)  
MF4 | Fach- und Forschungsdatenmanagement

## Create Release on Tag Push Action

**Parameter**

| Parameter | Bedeutung                                                  | Standardwert | zwingend notwendig |
|-----------|------------------------------------------------------------|--------------|--------------------|
| REF_NAME  | Name des Tags anhand dessen der Release gebaut werden soll | -            | ja                 |

**Environment**

| Parameter    | Bedeutung                                                                                   | Standardwert | zwingend notwendig |
|--------------|---------------------------------------------------------------------------------------------|--------------|--------------------|
| GITHUB_TOKEN | Github Token des aktuellen Workflows mit entsprechenden Rechten für das aktuelle Repository | -            | ja                 |

## Send Metadata To Govdata

**Parameter**

| Parameter             | Bedeutung                                                                | Standardwert                            | zwingend notwendig |
|-----------------------|--------------------------------------------------------------------------|-----------------------------------------|--------------------|
| source_file           | Quelldatei die in das Sammelrepo für Govdata kopiert werden soll         | Metadaten/govdata.ttl                   | nein               |
| destination_file_name | Name der kopierten Datei im Zielrepo                                     | ${{github\.event.repository.name }}.ttl | nein               |
| destination_repo      | Repo, in das die entfernte Datei kopiert werden soll                     | knutator2/Metadaten_Test                | nein               | 
| destination_folder    | Ordner im entfernten Repo in den die kopierte Datei abgelegt werden soll | Datensaetze                             | nein               |
| user_email            | E-Mail Adresse für den Git Commit                                        | opendata@rki.de                         | nein               |
| Parameter             | Text                                                                     | Text                                    | Text               |
| Parameter             | Text                                                                     | Text                                    | Text               |

**Environment**

| Parameter    | Bedeutung                                                                                   | Standardwert | zwingend notwendig |
|--------------|---------------------------------------------------------------------------------------------|--------------|--------------------|
| GITHUB_TOKEN | Github Token des aktuellen Workflows mit entsprechenden Rechten für das aktuelle Repository | -            | ja                 |