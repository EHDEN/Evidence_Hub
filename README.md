# Evidence Hub
Requirements and specification for the evidence hub


## Objective

The EHDEN evidence hub is intended to be the primary repository where studies, including relevant documentation and interactive exploration of results will be made available to the users in a secure way. The studies in scope are the ones executed through the EHDEN network, irrespective of whom the respective lead investigator / participants are. 


## Principles

- The Evidence Hub will only be accessible to registered users
- Under studies we understand any coordinated effort to generate scientific insights or advance public health
- Excluded are the preparatory steps to evaluate the possibility for performing the intended study as well as the contractual / administrative preparation
- Any high level information on studies i.e. study title, description, status is accessible to all users of the evidence hub
- For the details i.e. protocol , methodology and results of a study a study can be classified as 'public' or 'confidential'
- For studies, classified as 'public', protocol, methods (incl scripts) and collective (aggregated) results will be accessible to all registered users of the tool
- For studies, classified as 'confidential', collective study results are only accessible to the users of the respective sponsoring organisation or the participating (data partners and analysis) organisations while individual study results are only accessible to the respective data partner and to the study lead / coordinator


## Requirements

- The Evidence Hub will be accessible through the EHDEN portal
- Access can be controlled at a study level
- A study will have the following attributes:
    * A title (public)
    * Unique ID (public)
    * A description (public)
    * A lead investigator (public)
    * Study Status: Planned / Active / Finalised (public)
    * Study Visibility: Public / Confidential (public)
    * Medical Conditions and/or Drug / drug classes and/or devices / procedures as subject for this study : list of OMOP concepts / classes (public)
    * Geographic coverage: list of selected country/ies (public)
    * Affiliated institutions: contributing partners to this study (confidential)
- It will be possible to associate a study with the following objects 
   * A study protocol: word or pdf file (public or confidential)
   * A statistical analysis plan : word or pdf file (public or confidential)
   * One or more scripts for executing the study with auxilliary files such as cohort definitions etc: zip file (public or confidential)
   * Results from individual sites: csv, json, xlsx or similar (always restricted to the lead investigator and respective data partner)
   * Summary results (obtained by processing further the results from the individual sites) : csv, json, xlsx, pdf, png (public or confidential)
   * An (interactive) application rendering the summary results (public or confidential): RShiny, Dash, Streamlit or equivalent
   * Publication(s) (public or confidential)


