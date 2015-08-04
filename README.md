## Template of Dev in Company Event Page.

### Usage

- Fork this repository and clone to your workspace

- Run this, `cd devincompany-site-event && npm install`

- Create a local branch using this template: `city/YYYY-MM-DD`.
    - For example... `belo-horizonte/2015-07-18`

- And run this, `node --harmony metalsmith.js`

- After all your project are now in a folder named `output`

### Important

- Find a file named `metadata.json` to bind all data of your event.

- To deploy your site in [devincompany.in](http://devincompany.in) send a Pull Request using the local branch created with your changes.

### Sections in `metadata.json`

#### devincompany

REQUIRED

```json
"devincompany": {
    "slug": "your-city-urlname",
    "facebook_thumb": "assets/images/thumbnail-facebook.png",
    "banner": "assets/images/cover.jpg",
    "logo": "assets/images/logo.png",
    "event_date": "Oct 31, 2015 09:00:00",
    "global_infos": "Google • 32 de dezembro de 2015 • Belo Horizonte • Minas Gerais",
    "call_to_action": {
        "link": "http://bit.ly/tickets_devincompany",
        "text": "INSCRIÇÕES ABERTAS"
    },
    "about": {
        "title": "O Dev in Company",
        "text": "O Dev in Company surge para consolidar e suprir uma deficiência de comunicação entre empresas e profissionais do mercado, abrir portas para quem deseja levar conteúdo de qualidade para a comunidade e possibilitar uma maior interação e experiência entre os participantes, aumentando assim o network entre os presentes."
    },
    "contacts": {
        "facebook": "https://www.facebook.com/devincompany",
        "twitter": "https://twitter.com/devincompany",
        "email": "contato@devincompany.in"
    },
    "location": {
        "address": "Google • Avenida Bias Fortes, 382 • Lourdes • Belo Horizonte • MG",
        "reference": "Próximo a Praça da Liberdade",
        "lat": "-19.9295323",
        "lon": "-43.9407365"
    },
    "ga": "UA-XXXXXX-X",
    "schedule": true
}
```
#### lineup

OPTIONAL: to remove this section, just empty the array in `metadata.json`

```json
"lineup": [
    {
        "name": "Off-time",
        "scheduled_to": "99h99"
    }, {
        "featured": true,
        "photo": "assets/images/speakers/speaker.png",
        "name": "Speaker",
        "contact": "http://github.com/speakeronedevincompany",
        "company": {
            "name": "Company Name",
            "site": "https://company.com"
        },
        "bio": "Vitae, assumenda nemo tempore quasi, quidem officiis voluptate facilis molestiae quas laudantium? Nesciunt cumque, in!",
        "talk": {
            "theme": "A super star deluxe talk!!!",
            "desc": "Sit dolor architecto repellat tenetur, doloremque aspernatur delectus voluptate aliquam itaque eius aperiam a aut accusantium, pariatur culpa rem qui sed!"
        },
        "scheduled_to": "99h99"
    }, {

    ...

    }, {
        "featured": true,
        "last_speaker": true,
        "photo": "assets/images/speakers/speaker.png",
        "name": "Speaker",
        "contact": "http://github.com/speakeronedevincompany",
        "company": {
            "name": "Company Name",
            "site": "https://company.com"
        },
        "bio": "Vitae, assumenda nemo tempore quasi, quidem officiis voluptate facilis molestiae quas laudantium? Nesciunt cumque, in!",
        "talk": {
            "theme": "A super star deluxe talk!!!",
            "desc": "Sit dolor architecto repellat tenetur, doloremque aspernatur delectus voluptate aliquam itaque eius aperiam a aut accusantium, pariatur culpa rem qui sed!"
        },
        "scheduled_to": "99h99"
    },
    {
        "name": "Off-time",
        "scheduled_to": "99h99"
    }
]
```

#### partners

REQUIRED

```json
"partners": [
    {
        "name": "Minas Dev",
        "site": "http://minasdev.org",
        "logo": "assets/images/partners/minasdev.png"
    },
    {
        "name": "Partner",
        "site": "http://partner.com",
        "logo": "assets/images/partners/partner.png"
    },
    ...
]
```

#### sponsors

OPTIONAL: to remove this section, just empty the array in `metadata.json`

```json
"sponsors": [
    {
        "name": "Sponsor",
        "site": "http://sponsor.com",
        "logo": "assets/images/sponsors/sponsor.png"
    },
    {
        "name": "Sponsor",
        "site": "http://sponsor.com",
        "logo": "assets/images/sponsors/sponsor.png"
    },
    ...
]
```

#### organizers

REQUIRED

```json
"organizers": [
    {
        "name": "Staff Member",
        "photo": "assets/images/staff/member.png",
        "contact": "http://member.com"
    },
    {
        "name": "Staff Member",
        "photo": "assets/images/staff/member.png",
        "contact": "http://facebook.com/member"
    },
    ...
]
```

#### TODO

- Improve this doc
- Improve code of template
- Improve layout of template
