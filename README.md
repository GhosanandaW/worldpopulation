# World Population
Data for a narrative visualization and dashboard explaining the current state of world population, growth, and demographic and analysis on it change trend.

The data has been manipulated with logic as follows:
1. WPP2022_GEN_F01_DEMOGRAPHIC_INDICATORS_COMPACT_REV1_manipulated is the data source providing the country names, crude birth rate, crude death rate, and growth percentage information. The manipulation on this data includes: 
   1. Deleted UN logo and header (not directly pertaining to the data).
   2. Deleted cascaded header to result in Tableau compatible data source.
2. WDICountry_manipulated is the data source providing the region classification for the country names.
   1. No manipulation was done for the data, but included in the repository for reference (same as original).
3. WPP2022_POP_F02_2_POPULATION_5-YEAR_AGE_GROUPS_MALE_tagged_manipulated, WPP2022_POP_F02_3_POPULATION_5-YEAR_AGE_GROUPS_FEMALE_tagged_manipulated, Male_population_pivoted_tagged_final_manipulated, Female_population_pivoted_tagged_final_manipulated is the data source providing the demographic breakdown by gender and age for each year for each country. The manipulation on this data includes: 
   1. Created additional attribute "gender" to result in relational-like data source that is compatible with Tableau.
   2. Deleted UN logo and header (not directly pertaining to the data).
   3. Deleted cascaded header to result in Tableau compatible data source.
   4. Pivoted the "age" attribute from each file to result in breakdown of the demographic for each given year.
4. The data mentioned were joined into joined_world_population_data# ghosanandaw.github.io
