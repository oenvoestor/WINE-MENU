# WINE-MENU
Guide des cartes des vins des restaurants de France, avec filtres, recherche, fiches restaurants, aperçu des cartes et assistant sommelier IA.

## Aperçu

Tchin tchin  est une application React/TypeScript qui permet de :

- parcourir une sélection de restaurants
- filtrer par type de vin, région et ville
- rechercher un restaurant, un vin ou une région
- consulter les cartes des vins par restaurant
- ouvrir les PDF des cartes complètes
- discuter avec un sommelier IA selon la carte du restaurant

## Fonctionnalités

- **Page d’accueil** avec barre de recherche
- **Filtres** par type de vin, région et ville
- **Cartes restaurant** avec image, ville, cuisine et nombre de vins
- **Modal de carte des vins** avec aperçu des références
- **Assistant Sommelier IA** connecté à une fonction Supabase
- **Navigation par routes** vers les pages restaurant et vin
- **Import de données statiques** depuis `src/data`

## Stack technique

- **React**
- **TypeScript**
- **Vite**
- **Tailwind CSS**
- **React Router**
- **Lucide React**
- **Supabase Edge Functions**

## Structure du projet

```bash
src/
  components/
    FilterBar.tsx
    HeroSection.tsx
    NavLink.tsx
    RestaurantCard.tsx
    SommelierChat.tsx
    WineListModal.tsx

  data/
    restaurants.ts
    wines-rosette.ts
    wines-comptoir.ts
    wines-mermoz.ts
    wines-clarence.ts
    wines-ressources.ts
    wines-110taillevent.ts
    ...

  hooks/
    use-toast.ts

  lib/
    utils.ts

git clone https://github.com/oenvoestor/WINE-MENU.md
cd tchin-tchin
npm install
npm run dev
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_PUBLISHABLE_KEY=your_supabase_key
