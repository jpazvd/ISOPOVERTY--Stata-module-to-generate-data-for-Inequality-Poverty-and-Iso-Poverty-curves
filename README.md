# ISOPOVERTY: Stata module to generate data for Inequality-Poverty and Iso-Poverty curves

## Description

    isopoverty generates data that can be used to plot the Inequality-Poverty, Growth-Poverty and
    the Iso-Poverty curves (ECLAC, 2002; Bourguignon, 2002; Kakwani and Pernia, 2000; Bigsten and
    Shimeles, 2003; Barros et al, 2005; Barros et al, 2003).

    stepgrw or stepinq have to be stated otherwise the programme does not work. If the option
    stepgrw is specified the ado automatically generates the Growth-Poverty data, likewise, if the
    option stepinq is spefied the program it will generate the Inequality-Poverty data. If both
    parameters are specified both procedures will be implemented.

    Please note that in order to provider a greater flexibility on the graph options this ado does
    not automatically produce any figures. The final output is stored as a matrix in the Stata
    memory (please see ereturn), in order to retrive it to the data set the use will have to use
    the svmat command. An illustration of a figure produced with data from this ado can be found
    in the examples below.

    Inequality -> r(ineqreduc)
    Growth -> r(growth)
    Iso-Poverty -> r(frontier)

    WARNING! The Iso-Poverty is quite computationally intensive.  We strongly advice the user to
    first estimate the Inequality-Poverty curve and then the Growth-Poverty curve, in order to
    find out the best cut off points for the data that she or he is using.

### Options

    varpl(varname) provide the variable name containing the values poverty line.

    pline(#) sets the value of the poverty line. The default poverty line is computed as half the
    median of varname.

    poverty is the default output and includes the head count ratio and the extremme poverty head
    count ratio, several other poverty measures can be easily included in this output.

    inequal includes the Gini and Theil inequallity measures in the output.

## Suggested Citation
[Joao Pedro Azevedo & Samuel Franco, 2006. "ISOPOVERTY: Stata module to generate data for Inequality-Poverty and Iso-Poverty curves," Statistical Software Components S456752, Boston College Department of Economics, revised 04 May 2014.](https://ideas.repec.org/c/boc/bocode/s456752.html)

## References

    Barros, R. Carvalho, M. Franco, S. Ganuza E., Mendonça, R. (2005) El combate a la pobreza en
        Centroamerica.  UNDP and IPEA. (Apendices 2 y 3 y Capitulo 5)

    Barros, R.P. Carvalho, M. Franco, S. (2003) La igualdad como estrategia de combate a la
        pobreza en Panam? (Cap?tulo 6). Panama: PNUD.   (link)

    ECLAC (2002) Meeting the Millennium Poverty Reduction Targets in Latin America and the
        Caribbean. Santiago, Chile: ECLAC-IPEA-UNDP.  (link)

    Bourguignon, F. (2002), "The Growth Elasticity of Poverty Reduction: explaining heterogeneity
        across countries and time periods", in T. Eichler and S. Turnovsky (eds.), Growth and
        Inequality, Cambridge: MIT Press.

    Bigsten, A. and A. Shimeles (2003). "Prospects for a Pro-Poor Growth Strategy in Africa",
        Paper presented at the WIDER Conference on Human Wellbeing and Income Inequality,
        Helsinki, May.

    Kakwani, N. and E.M. Pernia (2000), "What is Pro-Poor Growth", Asian Development Review
        18(1): 1-16.

### Handle: RePEc:boc:bocode:s456752 

### Note: 
This module should be installed from within Stata by typing "ssc install isopoverty". Windows users should not attempt to download these files with a web browser.

### Keywords
Poverty; Inequality; Iso-Poverty

## Author: 

  **JoÃ£o Pedro Azevedo**  
  [jazevedo@worldbank.org](mailto:jazevedo@worldbank.org)  
  World Bank  
  [personal page](http://www.worldbank.org/en/about/people/j/joao-pedro-azevedo)  

