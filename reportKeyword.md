# Catalisio API
## Report 'keyword'
### Description
The 'keyword' report provides data by keywords, for particular period, goal and branding filter.
### Data
* `startDate` (required) : YYYY-MM-DD (i.e : 2015-12-23)
* `endDate` (required) : YYYY-MM-DD (i.e : 2015-12-23)
* `goalId` (required) : Id of the goal 
* `branding` (required) : `1` or `0` to have results for branding or no-branding
### File format
The file format is :
* CSV
* UTF8
* `;` delimiter
* UNIX line ending
* first line is a header
* quotes `""` in order to escape strings

Columns are, in this order :
1. Mot-clé
2. Visites
3. Ventes
4. Chiffre d'affaires
5. Panier moyen
6. Volume de recherche
7. Position moyenne
8. Taux de conversion
