# LeBonVoisin

> _Description courte du projet à compléter._

Monorepo contenant :

- **`front/`** — application web en [Next.js](https://nextjs.org) (React, TypeScript)
- **`back/`** — API en [FastAPI](https://fastapi.tiangolo.com) (Python), gérée avec [uv](https://docs.astral.sh/uv/)

```
LeBonVoisin/
├── back/        # API Python (FastAPI)
├── front/       # Application Next.js
├── .gitignore
└── README.md
```

## Prérequis

- [Node.js](https://nodejs.org) 20.9 ou plus (LTS recommandée)
- [uv](https://docs.astral.sh/uv/getting-started/installation/) (il installe lui-même la bonne version de Python)

```bash
# Installer uv — macOS / Linux
curl -LsSf https://astral.sh/uv/install.sh | sh

# Installer uv — Windows (PowerShell)
powershell -c "irm https://astral.sh/uv/install.ps1 | iex"
```

## Installation

```bash
git clone <url-du-repo>
cd LeBonVoisin

# Front
cd front
npm install

# Back
cd ../back
uv sync
```

## Lancer le projet en local

Il faut deux terminaux, un pour chaque partie.

**Terminal 1 — API**

```bash
cd back
uv run fastapi dev main.py
```

**Terminal 2 — Front**

```bash
cd front
npm run dev
```

| Service | URL |
|---|---|
| Front | http://localhost:3000 |
| API | http://localhost:8000 |
| Documentation de l'API (Swagger) | http://localhost:8000/docs |

## Variables d'environnement

Les fichiers `.env` ne sont pas versionnés. Créez-les à partir des exemples :

- `front/.env.local` — ex. `NEXT_PUBLIC_API_URL=http://localhost:8000`
- `back/.env` — ex. URL de la base de données, clés secrètes

## Commandes utiles

| Commande | Où | Rôle |
|---|---|---|
| `npm run dev` | `front/` | Serveur de développement |
| `npm run build` | `front/` | Build de production |
| `npm run lint` | `front/` | Lint du code |
| `uv add <paquet>` | `back/` | Ajouter une dépendance Python |
| `uv sync` | `back/` | Installer les dépendances |
| `uv run fastapi dev main.py` | `back/` | Lancer l'API en mode dev |