# Fluxy — architecture

[← Retour à la présentation](README.md)

Application web de gestion du budget du foyer. Ce dépôt présente le produit ; le code source est privé.

| Couche | Technologies et rôle |
| --- | --- |
| Interface | React, TypeScript et Tailwind CSS : saisie quotidienne, récurrents et pilotage du mois. |
| Application | TanStack Start et TanStack Router : pages et fonctions serveur. |
| Données côté interface | TanStack Query : lecture et actualisation des données. |
| Persistance | PostgreSQL et Prisma : foyers, membres, opérations et récurrents. |
| Authentification | Better Auth : comptes et sessions. |
| Validation | Zod : validation des données. |

## De la dépense au mois

Les opérations quotidiennes alimentent le rythme de dépenses. Les revenus et charges récurrents, ainsi que les dépenses exceptionnelles, complètent l’estimation de fin de mois.

Le pilotage compare le rythme actuel à un objectif de dépenses courantes. Les récurrents peuvent comporter des rappels, des actions programmées et des changements de tarif.

Les données sont partagées au sein du foyer. Un propriétaire peut inviter un autre membre à le rejoindre.

Les visuels publics sont des compositions simplifiées avec des données fictives. Aucun budget personnel ni identifiant de connexion n’est publié dans ce dépôt.
