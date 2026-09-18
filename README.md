# Finlay_Ryder_MPhil_Chapter3

Analysis and modelling for Chapter 3 spans three R Quarto scripts. `Parasite_Topological_Analysis.qmd` shows the topological extinction analysis and calculation of basic food web metrics, although several parts of this analysis were processed through Cardiff BIOSI High Performance Computing (HPC) server, 'Skomer'. `Bayesian_Modelling.qmd` shows the Bayesian model and analysis run for all network variants. `Bayesian_Modelling_Analysis.qmd` shows post-hoc analysis done on Bayesian model outputs to produce graphs and run Bayesian descriptive stats analysis. 

Parts of the modelling modelling analysis was performed on the Cardiff School of Biosciences' Biocomputing Hub HPC/Cloud infrastructure. Resources funded by the Cardiff School of Biosciences. 

Several files required for later developed scripts import analysis from prior scripts, rather than running from scratch, hence the **large** number of files included in this repository. I have listed below the files required for each script, hopefully to make re-running it easier!

These analyses were carried out for four food webs: Quick Pond (`Quick_Pond_Nodes.csv` and `Quick_Pond_Links.csv`) and Carpinteria Salt Marsh (`Carpinteria_Web.csv`). Both Ythan Estuary and Punta Banda Estuary are extracted from `Dune_2013_Webs.xlsx`. 

`Parasite_Topological_Analysis.qmd` requires files `gateway_food_web_list.rds`, `quick_pond_adj_matrices.rds, `null_qp_robustness_MC_results.csv`, `qp_robustness_results_auc_most_df.csv`, `qp_robustness_results_auc_random.rds`, `qp_robustness_results_auc_random.csv`, `qp_selected_networks.rds`, `all_carpinteria_matrices_cleaned.rds`, `Carp_MC_Sim_Results.csv`, `null_carp_robustness_MC_results.csv`, `carp_robustness_results_auc_most_df`, `carp_selected_networks.rds`, `ythan_parasites_removed.rds`, `ye_MC_Sim_Results.csv`, `ye_robustness_results_auc_random.rds`, `ye_selected_networks.rds`, `null_ye_robustness_MC_results.csv`, `banda_parasites_concamitant.rds`, `banda_parasites_removed.rds`, `pb_MC_Sim_Results.csv`, `banda_robustness_results_auc_random.rds`, `pb_selected_networks.rds`, `null_pb_robustness_MC_results.csv`, `banda_parasites_concamitant.rds`, `banda_parasites_concamitant.rds`, `pb_MC_Sim_Results.csv`, `banda_robustness_results_auc_random.rds`, `pb_selected_networks.rds`, `null_pb_robustness_MC_results.csv`, 


`Bayesian_Modelling.qmd` requires files `Quick_Pond_Nodes.csv`, `Quick_Pond_Links.csv`, `gateway_food_web_list.rds`, `carp_web_taxonomy.csv`, `Dunne_2013_Species_Lists.csv`,`Ythan_Estuary_Links.csv`, `ythan_nodes_complete.csv`, `banda_web.csv`,
`banda_nodes_complete.csv`


`Bayesian_Modelling_Analysis.qmd` requires files `carp_agg_wo_parasites_results.csv`, `carp_agg_results.csv`, `carp_ls_results.csv`, `carp_ls_wo_parasites_results.csv`, `qp_agg_results.csv`, `qp_ls_results.csv`, `ythan_with_parasites_concam_results.csv`, `ythan_without_parasites_results.csv`, `banda_with_parasites_concam_results.csv`, `banda_without_parasites_results.csv`, `carp_parasitic_species_ids.rds`,`carp_parasitic_node_ids.rds`
