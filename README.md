Inputs:   
1. Standard tax rates: I used state and local tax rates in "input/Sales taxes on goods/Raw/[year]_aftertaxes.xlsx" (Column A:C). These are produced by the Norwegian RA. It looks like the set of files named "[year]_aftertaxes.xlsx" are cleaned version of the files named "salestaxstatelocal.xlsx".      
   - There was a mistake in input file main/input/consumption_taxes/Sales taxes on goods/Raw/2010_aftertaxes.xlsx for Colorado. The raw file downloaded from tax foundation says 2.90          but the cleaned file somehow says 2.00. I manually corrected it in the input file.     
2. Food tax rates: I downloaded these from the Book of States into "input/Taxes on Food at Home/Raw". I converted them to Excel files "[year] Sales Tax.xlsx" and saved in "input/Taxes on Food at Home".     
3. Services tax rates: I used "services2007_clean.xlsx" in the input folder. I received this file from Jonathan.     
4. Color-coded input file: I received this file from Jonathan. I also made some changes:     
   - I manually added column F, G and J to the color-coded file received from Jonathan. Column F and G are to help with aggregation of tax rates to desired CEX expenditure aggregation       levels. Column J helps to identify what kind of tax rates we need to apply for each row.   
   - Column F: Subcompnent's expenditure share of the bigger component.   
   - Column G: The number of subcomponents to aggregate that the bigger component has.   
   - Column J:     
        (a) -1: no color or yellow. 0% tax rate      
        (b) 0: Food at home      
        (c) 1: Standard tax rates       
        (d) 2: Special tax rates given JF code       

Outputs:
1. Standard tax rates by state and year: "output/standard tax rate.xlsx"   
2. Food tax rates by state and year: "output/food tax rate.xlsx"   
3. Services tax rates by state and year and JF code: "output/services tax rate.xlsx"    
4. Tax rates aggregated to our CEX category by state, for each year: "output/[year]_tax_rates_by_CEX_states.xlsx"    
