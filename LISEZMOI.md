# Site Luxicom — Guide de mise en ligne

## Ce qu'il y a dans le dossier

```
luxicom-site/
├── index.html          ← le site (tout est dedans)
├── favicon.svg         ← la petite icône dans l'onglet du navigateur
├── robots.txt          ← permet à Google d'indexer le site
└── images/
    └── clients/        ← mets ici les logos de tes clients
```

---

## Étape 1 — Remplir tes infos (10 minutes)

Ouvre `index.html` avec un éditeur de texte (VS Code, gratuit, est le plus simple : code.visualstudio.com).

1. **Tes clients** : tout en haut du fichier, dans le bloc `NOS CLIENTS`.
   Remplis `nom`, `secteur`, `services`, et si tu as le logo : `"logo": "images/clients/nom.png"`.
2. **Ton courriel** : cherche `VOTRE@COURRIEL.COM` (Ctrl+F / Cmd+F) et remplace-le partout (3 fois).
3. **Ton téléphone et ta ville** : cherche `[votre téléphone]` et `[votre ville]`.
4. **Ton Instagram** : cherche `VOTRE_COMPTE` et remplace-le (2 fois).

Double-clique sur `index.html` pour voir le résultat dans ton navigateur.

---

## Étape 2 — Mettre le site en ligne (gratuit)

### Option A : Netlify Drop (le plus simple, 2 minutes)
1. Va sur **app.netlify.com/drop**
2. Crée un compte gratuit
3. Glisse-dépose **le dossier `luxicom-site` au complet** dans la page
4. Ton site est en ligne avec une adresse du genre `luxicom-123.netlify.app`
5. Pour changer l'adresse : *Site configuration › Change site name* → `luxicom.netlify.app`

Pour mettre à jour plus tard : *Deploys* → glisse-dépose le dossier à nouveau.

### Option B : Vercel (tu as déjà un compte)
1. Installe Node.js (nodejs.org) si ce n'est pas déjà fait
2. Ouvre un terminal dans le dossier `luxicom-site` et tape : `npx vercel`
3. Réponds aux questions (les choix par défaut sont bons), puis `npx vercel --prod`
4. Ton site est en ligne avec une adresse `.vercel.app`

(Ou demande-moi : je peux le mettre en ligne directement sur ton compte Vercel.)

---

## Étape 3 — Ton propre nom de domaine (≈ 15 à 25 $ / an)

Pour avoir **luxicom.ca** ou **luxicom.com** au lieu de `.netlify.app` :

1. Vérifie que le nom est libre et achète-le chez un registraire :
   - `.ca` : Namecheap, GoDaddy ou Porkbun (le `.ca` demande d'être au Canada — c'est ton cas)
   - `.com` : Namecheap, Porkbun, Cloudflare
2. Dans Netlify : *Domain management › Add a domain* → entre ton domaine
   (dans Vercel : *Settings › Domains*)
3. Netlify/Vercel t'indique quoi changer chez ton registraire (les « DNS »).
   Copie-colle ce qu'ils te donnent. Ça prend de quelques minutes à 24 h.
4. Le cadenas HTTPS s'active tout seul, gratuitement.

---

## Étape 4 — Un courriel pro (recommandé)

Un courriel comme **bonjour@luxicom.ca** fait beaucoup plus pro qu'un Gmail.
- **Google Workspace** (≈ 8 $/mois) ou **Zoho Mail** (version gratuite possible)
- Ils te guident pour l'associer à ton domaine.

Ensuite, mets cette adresse partout où il y a `VOTRE@COURRIEL.COM`.

---

## Étape 5 — Être trouvé sur Google

1. **Google Business Profile** (gratuit) : business.google.com — fiche avec ton adresse, tes heures, tes avis. Très important pour une entreprise locale.
2. **Google Search Console** (gratuit) : search.google.com/search-console — ajoute ton site pour que Google l'indexe plus vite.
3. Mets le lien de ton site dans ta bio Instagram, Facebook et LinkedIn.

---

## Le formulaire de contact

Quand un visiteur clique sur « Envoyer ma demande », son application courriel s'ouvre avec le message déjà écrit, adressé à toi. Ça marche sans rien installer.

**Pour recevoir les demandes directement (sans que le visiteur ouvre son courriel)** :
- Sur Netlify : ajoute `data-netlify="true"` et `name="contact"` à la balise `<form>` et Netlify t'enverra les demandes par courriel (gratuit jusqu'à 100/mois). Demande-moi et je te fais la modif.
- Ou utilise **Formspree** (formspree.io, gratuit pour commencer).

---

## Récap rapide

| Quoi | Où | Prix |
|---|---|---|
| Hébergement | Netlify ou Vercel | Gratuit |
| Nom de domaine | Namecheap / Porkbun | ≈ 15–25 $/an |
| Courriel pro | Zoho / Google Workspace | 0–8 $/mois |
| Fiche Google | business.google.com | Gratuit |
