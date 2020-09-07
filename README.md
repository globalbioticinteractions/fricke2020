[![Build Status](https://travis-ci.com/globalbioticinteractions/fricke2020.svg)](https://travis-ci.com/globalbioticinteractions/fricke2020) [![GloBI](http://api.globalbioticinteractions.org/interaction.svg?accordingTo=globi:globalbioticinteractions/fricke2020)](http://globalbioticinteractions.org/?accordingTo=globi:globalbioticinteractions/fricke2020)

Configuration to help Global Biotic Interactions (GloBI, https://globalbioticinteractions.org) index: 

Fricke, E.C., Svenning, J. Accelerating homogenization of the global plant–frugivore meta-network. Nature 585, 74–78 (2020). https://doi.org/10.1038/s41586-020-2640-y

Fricke, Evan; Svenning, Jens-Christian (2020), Data from: Accelerating homogenization of the global plant–frugivore meta-network, Dryad, Dataset, https://doi.org/10.5061/dryad.44j0zpcbx

The included datafile ```net.long0.tsv``` was created by:

0. open a web browser and visit https://doi.org/10.5061/dryad.44j0zpcbx
1. download and save the dataset zip by clicking on "download dataset" 
2. unzip the saved file "doi_10.5061_dryad.44j0zpcbx__v1.zip" (hash://sha256/c2b2d06be42d231025c7aa5b6fc8b44109797854bc42a0284529be27f0ef8fb2)
3. unzip the single file contained in "doi_10.5061_dryad.44j0zpcbx__v1.zip" (hash://sha256/9104befc86f96058e88b74f0a204d8a6055197c95b97079a87dc29beea400033)
4. open R workspace ```"metanetwork data and code/metanetwork data and code.Rproj"``` in R studio Version 1.2.5033
5. read R code in file ```"metanetwork data and code/analysis/network homogenization analysis.R"``` (hash://sha256/40d4a71437ae96dbdd1527d69a36522125c0ed9fb628c58cf2da17b8b1649965) 
6. using R extract the "long" version of the interaction data using the binary RData file ```"metanetwork data and code/analysis/homogenization.RData"``` (hash://sha256/40d4a71437ae96dbdd1527d69a36522125c0ed9fb628c58cf2da17b8b1649965)
```R
load(file = "./analysis/homogenization.RData")
write.table(net.long0, "net.long0.tsv", quote = FALSE, sep = "\t", fileEncoding ="UTF-8", row.names=F)
```
7. which results in the included file ```net.long0.tsv``` with hash://sha256/c98029705a50c4576df5e25fd6ac55dca8c8a49d2d322efd99ea142fd5824943
