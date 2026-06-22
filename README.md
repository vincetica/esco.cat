# esco.cat

Plataforma de participació cívica. Vota les mateixes lleis que el Parlament de Catalunya i compara els resultats.

## Estructura del projecte

```
esco-cat/
├── index.html              ← Landing page pública
├── app/
│   └── index.html          ← Demo interactiva de l'app
├── legal/
│   ├── privadesa.html      ← Política de privadesa
│   └── termes.html         ← Termes d'ús
├── assets/                 ← Recursos compartits
└── .github/workflows/
    └── deploy.yml          ← Desplegament automàtic via FTP
```

## Desplegament

Qualsevol push a la branca `main` desplega automàticament a esco.cat via FTP.

### Configuració dels secrets a GitHub

Ves a Settings → Secrets and variables → Actions i afegeix:

| Secret | Valor |
|--------|-------|
| `FTP_HOST` | El servidor FTP de CDMon (ex: ftp.esco.cat) |
| `FTP_USER` | El teu usuari FTP de CDMon |
| `FTP_PASSWORD` | La teva contrasenya FTP de CDMon |

## Desenvolupament local

Obre `index.html` directament al navegador, o fes servir un servidor local:

```bash
npx serve .
```

## Contacte

hola@esco.cat 

