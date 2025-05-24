# Les 12 principes du game engineering

## 1. Deterministic Tick (Tickbound) - L’autorité sur le temps

Ce n’est pas à la machine d’imposer son rythme, mais au moteur de déterminer le tempo du jeu avec précision et rigueur. Il est l’unique chef d’orchestre, le **métronome logique** qui compose sa propre réalité **mesure après mesure**. Toute variation flottante n’apporterait qu’incertitude, imprécision et désordre au sein des cycles. C’est l’horloger qui décide du temps qui s’écoule.

## 2. Bounded Simulation Box (Simbox) - L’univers est borné

L’espace de jeu, comme la mémoire qu’il occupe, doit être **fini**, **borné**, **mesurable**. Les entités vivent dans un cadre limité, qu’il soit une grille, carte ou un tableau. Rien ne doit s’étendre sans **consentement explicite**,  et toutes les données sont administrées sous un contrôle strict. Un petit territoire bien gouverné vaut mille champs sauvages.

## 3. Progressive Workload (Dipload) - Répartir au compte-goutte

Le temps d’exécution est une ressource limitée qu’il faut manipuler avec parcimonie. Il faut **répartir** et **différer** le traitement d’une charge de travail, afin de **lisser la courbe de l’effort** et réduire les pics de charge. L’instant d’exécution ne coïncide pas toujours avec l’instant de décision. L’élan de l’euphorie s’épuise sans la constance du travail.


## 4. Forward Only Logic (Uniflow) - La verticalité du raisonnement

La logique de jeu doit s’écouler telle une cascade irréversible, du début jusqu’à la fin de son cycle. Elle est comme  un livre linéaire où chaque chapitre dépend strictement du précédent. Ce qui est en haut, ne doit jamais être corrompu par ce qui est en bas. Ce **flux unidirectionnel** garantit la lisibilité, la testabilité et la maîtrise de la causalité. La promesse de jeu devient ainsi **prévisible** et **structuré**. Le courant ne remonte jamais à sa source.

## 5. Explicite State Machine (StateLogic) - L’état encadre, le code exécute

Le comportement d’une entité ne doit jamais se reposer sur des conditions éparses, ni caché dans des ramifications implicites. Il est gouverné par un **état explicite**, **unique** et **observable**. Chaque état délimite ses **actions possibles**, ses **transitions autorisées** et ses **réactions attendues**. Le code ne décide de rien, l’état encadre tout.

## 6. Single-Authority Update (Onewrite) - Le vérité n’émerge jamais de deux scribes

La vérité ne peut venir que d’un seul endroit, écrite par une seule main. Chaque donnée ne doit être écrite qu’une **seule fois par cycle**. Il est gouverné par un système unique, à l’autorité exclusive, dont **chaque opération est traçable**. Il ne peut y avoir de propriété partagée, ni de double écriture. Nul ne peut servir deux maîtres.

## 7. Input-Simulation-Render Split (Triarc) - Une pièce en trois actes

L’**entrée**, la **logique** et le **rendu** sont trois canaux séparés qui ne doivent jamais se confondre. Le premier est le souffle qui effleure le monde, mais n’en détermine pas l’issue. Le second est le cœur qui bat à son rythme, maître de l’espace-temps, qui raisonne et évolue selon les états. Le dernier est un miroir du passé, il reflète ce qui fut, jamais ce qui sera.

## 8. Grouped Execution Strategy (Batchlane) - L’appel des mille

Tout ce qui se ressemble s’assemble. Les **entités semblables** doivent être **traitées ensemble**, invoquées d’un seul mot, appelées d’un seul geste. Celui qui s’adresse à un groupe est plus efficace que celui qui s’adresse à chacun. Aucune entité n’est jamais vraiment orpheline.

## 9. Transparent Cost Discipline (Transparent Cost) - Tout se révèle à la discipline 

L’ouvrier qui cache ses efforts, trahit son architecte. Toute tâche lourde doit pouvoir **alerter d’un signal**. Tout ce qui consomme doit **pouvoir se mesurer**. Tout ce qui ralentit doit **pouvoir s’expliquer**. L’invisible est une menace silencieuse, un traître embusqué dans le cycle, une dette aux intérêts tragiques.

## 10. Explicite Scope Discipline (Explicit Scope) - Aucune ombre dans le palais

Aucun marionnettiste caché ne doit injecter des ordres sans passer par un canal clair. Toute variable qui **influence doit apparaître**. Ce qui change l’état du palais doit franchir **la porte du contexte**. Ce qui agit doit être vu. Le moteur n’obéit pas aux fantômes des variables globales ou de systèmes cachés. Il ne répond qu’aux voix déclarées, aux signatures explicites.

## 11. Prebake Discipline (Bakefix) - Aucun plat ne se prépare à table

Le cuisinier qui prépare ses ingrédients évite l’agitation durant la cuisson. Ce qui peut être **calculé d’avance** ne doit jamais l’être en temps réel. Chaque effort anticipé est un effort épargné à l’ouvrier. Chaque donnée inscrite dans le marbre en amont ne redoute plus les incertitudes futures.

## 12. Logical Filtering (Trimset) - Les morts ne parlent pas

Le moteur ne doit consacrer son énergie qu’à ce qui vit, agit ou influence. Les entités hors champ ou mortes doivent être **mises de côté ou ignorées**. Ce qui n’est plus utile doit quitter la scène. Mais les morts ne s’effacent pas : ils attendent dans l’ombre, en silence, loin des regards, jusqu’à ce qu’on les** **invoque à nouveau**.
