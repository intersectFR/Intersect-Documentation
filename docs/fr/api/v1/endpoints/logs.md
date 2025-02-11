# Logs

## Activité Joueur

Renvoie les informations d'activité d'un joueur

### Requête

**URL** : `/api/v1/logs/player/[lookupKey]/activity`

**Méthode** : `Character's id.`

**Clé de Recherche:** : `GET`

**Autorisation Requise** : `Oui`

**Type Contenus** : `NA`

**Corps**
Vide

---

### Réponse

**Condition** : NA

**Code** : `200 SUCCESS`

**Exemple**

```json
{
  "Total": 9,
  "Page": 0,
  "PageSize": 5,
  "Count": 5,
  "Values": [
    {
      "Id": "709e3acb-1c1e-406f-bd0d-a05d538e96b3",
      "TimeStamp": "2021-04-21T10:20:19.2101157",
      "UserId": "f4c6bead-48dc-4625-95a4-de2693efcf53",
      "PlayerId": "0d27012e-697e-4558-bf0a-794a17ab0e40",
      "Action": "SelectPlayer",
      "Peer": "Client",
      "Ip": "127.0.0.1",
      "Meta": "admin,Admin"
    },
    ...
  ],
  "Sort": null,
  "Extra": null
}
```

## Activity Utilisateur

Renvoie les informations d'activité utilisateur

### Requête

**URL** : `/api/v1/logs/user/[lookupKey]/activity`

**Méthode** : `User's id.`

**Clé de Recherche:** : `GET`

**Autorisation Requise** : `Oui`

**Type Contenus** : `NA`

**Corps**
Vide

---

### Réponse

**Condition** : NA

**Code** : `200 SUCCESS`

**Exemple**

```json
{
  "Total": 28,
  "Page": 0,
  "PageSize": 5,
  "Count": 5,
  "Values": [
    {
      "Id": "edb6512f-345b-4196-bc84-17587bd0eb2e",
      "TimeStamp": "2021-04-21T10:20:19.06552",
      "UserId": "f4c6bead-48dc-4625-95a4-de2693efcf53",
      "PlayerId": null,
      "Action": "Login",
      "Peer": "Client",
      "Ip": "127.0.0.1",
      "Meta": null
    },
    ...
  ],
  "Sort": null,
  "Extra": null
}
```

## Activité Utilisateur par IP

Renvoie les informations d'activité utilisateur par ip

### Requête

**URL** : `/api/v1/logs/user/[lookupKey]/ip`

**Méthode** : `User's id.`

**Clé de Recherche:** : `GET`

**Autorisation Requise** : `Oui`

**Type Contenus** : `NA`

**Corps**
Vide

---

### Réponse

**Condition** : NA

**Code** : `200 SUCCESS`

**Exemple**

```json
{
  "Total": 1,
  "Page": 0,
  "PageSize": 5,
  "Count": 1,
  "Values": [
    {
      "Ip": "127.0.0.1",
      "LastUsed": "2021-06-13T15:48:50.3759295",
      "OtherUsers": {
        "11487dde-7c15-4222-bb5a-eed6791251ed": "test"
      }
    },
    ...
  ],
  "Sort": null,
  "Extra": null
}
```
