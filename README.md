# Organigramme FAM

```mermaid
flowchart TB
    CA["Conseil d’Administration"]
    DG["Direction Génale"]
    DGA["Direction Générale Adjointe"]
    DPS["Direction Pôle Parcours Social"]
    CS["Cheffes de service"]

    CA --> DG
    DG --> DGA
    DGA --> DPS
    DPS --> CS

    SS["Services supports<br/>- Service Administratif et Financier<br/>- Service Informatique<br/>- Service H<br/>- Pôle QHSE"]
    DGA --> SS

    PMP["Professionnels médico-psychologiques"]
    STM["Services Transversaux Mutualisés<br/>- Secrétariat<br/>- Service Technique"]
    DPS --- PMP
    DPS --- STM

    PP["Professionnels paramédicaux"]
    PSE["Professionnels socio-éducatifs"]
    PE["Professionnels d’entretien"]

    CS --> PP
    CS --> PSE
    CS --> PE

    PMP_D["Médecin coordonateur<br/>Infirmière en Pratique Avancée<br/>Médecin psychiatre<br/>Psychologue"]
    PP_D["Infirmière Diplômée d’Etat<br/>Aides soignant·e·s"]
    PSE_D["Educatrices Spécialisées<br/>Coordinatrices<br/>Animatrices<br/>Accompagnant·e·s éducatif et social"]
    PE_D["Agent technique<br/>Gouvernante<br/>Agents de service et d’intérieurs"]

    PMP --> PMP_D
    PP --> PP_D
    PSE --> PSE_D
    PE --> PE_D
