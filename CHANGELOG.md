# Changelog Back Office
All notable changes to the Back Office Application will be documented in this file.

## [Unreleased]

## [2.X.0] - XXXX-XX-XX
### Added
 - Intégration de Gocardless Connect

## [2.8.1] - 2022-08-03
### Added
 - Changement de la navigation , pour les écrans de type mobile.

## [2.8.0] - 2022-07-20
### Added
 - Nouvelle section Installation dédié à guider les utilisateurs dans leur processus d'intégration de ProAbono.

## [2.7.1] - 2022-06-20
### Changed
 - Enregistrer une nouvelle carte ou mandat ne crée plus un nouveau client côté Stripe. On peut désormais retrouver le client en se basant sur la metadata suivante 'pa_customer_ref'

## [2.7.0] - 2022-05-20
### Changed
 - Revu de l'intégration de la PSP Stripe pour passer à la V3.
   NB au passage en prod, ça ne mettra pas à jour l'intégration Stripe SEPA pour les clients actuels (pour ne pas perturber leurs moulinettes) -> il faudra le migrer à l'unité"

   Stripe Connect ???


## [2.6.0] - 2022-04-20
### Added
- passerelle dummy => possibilité de simuler des rejets et des litiges depuis la fiche d'une transaction (BO v1)
- new endpoint - /v1/Pricing/Billing/Customer?nextBilling=true pour une projection de la prochaine facture.

### Changed
 - le champ "IsVisible" présent sur les "offres "est désormais un champs calculé
 - Si l'appel API à la gateway retourne une erreur technique alors ProAbono ne créera plus de transactions
 - toutes les opérations avec Transactions ont été revues (annulation, etc.)"

## [2.5.1] - 2021-11-25
### Fixed
 - Correction du batch SEPA
 - Correction du problème "Velobook"


## [2.X.0] - XXXX-XX-XX
### Added
 - Ajout de la gestion des chargebacks

## [2.5.0] - 2021-11-24
### Added
 - Ajout de l'option "Never Stop"

## [2.4.0] - 2021-11-17
### Added
 - remontée de la gestion des paiments par Batch SEPA

## [2.3.0] - 2021-10-05
### Added
 - Ajout du tableau de bord des métriques Saas. Cette fonctionnalité n'est accessible que pour les utilisateurs ayant l'abonnement.


## [2.3.0] - 2021-09-28
### Changed
 - Les rapports sont renommés "exports"
     - Les liens vers ces exports changent:(ex: /App/666/Reports/NewSubscribers devient /App/666/Reports/Export/NewSubscribers)
     - NB: Ce changement n'impacte que l'accès au pages du backoffice => les liens vers l'export JSON, CSV, etc..

## [2.2.1] - 2021-07-25
### Added
 - Lot de corrections

## [2.2.0] - 2021-07-11
### Added
 - personnalisation et traduction des textes du Catalogue
 - ordre des caractéristiques

## [2.1.0] - 2021-06-28
### Added
 - Changement d'offre à l'échéance

## [2.0.2] - 2021-06-14
### Added
 - remonté de la personnalisation des emails

## [2.0.1] - 2021-05-28
### Added
 - Lot de corrections

## [2.0.0] - 2021-05-09
### Added
 - Refont complète de l'interface du Backoffice. L'expérience utilisateur a été repensé pour mieux correspondre a la cible et facilité la compréhension. Sur le plan technique car elle est désormais développé grâce au framework JS React.