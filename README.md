This repository contains the COL dataset introduced in Basallo-Triana M, Bravo-Bastidas J, Contreras I, Cordeau J, Vidal-Holguín C, 2023 Intermodal hub network design with generalized capacity constraints and non-synchronized train–truck operations. Transportation Research Part B: Methodological.

The available files include:

Excel file: Describes the COL dataset and contains the coordinates (latitude and longitude) of each node

Text files: Contain the different test instances for the hub location problem of the COL dataset. 

The following is a detailed description of the content of each text file.

<n>	Number of nodes

<q>	Number of capacity levels

<w[1][1]> <w[1][2]> ... <w[1][n]>    Haversine distance (normalized by 2000) from node 1 to all others
: : :
: : :
<w[n][1]> <w[n][2]> ... <w[n][n]>    Haversine distance (normalized by 2000) from node 1 to all others

<w[1][1]> <w[1][2]> ... <w[1][n]>    Flow from node 1 to all others
: : :
: : :
<w[n][1]> <w[n][2]> ... <w[n][n]>    Flow from node n to all others

<f[1][1]> <f[1][2]> ... <f[1][q]>	Fixed installation cost of a hub at node 1 for all capacity levels
: : :
: : :
<f[n][1]> <f[n][2]> ... <f[n][q]>	Fixed installation cost of a hub at node n for all capacity levels

<δ>	Collection cost

<α>	Transfer cost

<χ>	Distribution cost

<ρ>	Direct transport cost

<a[1][1]> <a[1][2]> ... <a[1][q]>	Unit processing rate for the export flow at node 1 for all capacity levels
: : :
: : :
<a[n][1]> <a[n][2]> ... <a[n][q]>	Unit processing rate for the export flow at node n for all capacity levels

<b[1][1]> <b[1][2]> ... <b[1][q]>	Unit processing rate for the import flow at node 1 for all capacity levels
: : :
: : :
<b[n][1]> <b[n][2]> ... <b[n][q]>	Unit processing rate for the import flow at node n for all capacity levels


NOTES:
(1) Haversine distances are computed considering a sphere of radius 6371
(2) Export flow refers to the flow that comes to a hub from non-hub nodes
(3) Import flow refers to the flow that comes to a hub from other hubs
