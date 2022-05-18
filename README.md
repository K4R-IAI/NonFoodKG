
# NonFoodKG - A non-food product knowledge graph

Non-FoodKG is a non-food knowledge graph interlinking different ontologies designed for retail, household and robotic applications. It is based on a merged product taxonomy reflecting the product classification in grocery stores and drugstores that is linked to a product location ontology created from a robot belief state while performing stocktaking in a retail store as depicted in the following picture:<br> 
<img src="UseCaseImg/semDTCompose2.jpg" width="600" alt="semantic Digital Twin"/><br>
<small>Kümpel, M., Mueller, C.A., Beetz, M. (2021). <a href="https://link.springer.com/chapter/10.1007/978-3-030-88662-2_7"><i>Semantic Digital Twins for Retail Logistics</i></a>. In: Freitag, M., Kotzab, H., Megow, N. (eds) <b>Dynamics in Logistics</b>. Springer, Cham.</small><br>


The <b>product location ontology</b> therefore stores inventory data like stock and price of products as well as their positions relative to shelves (instead of coordinates). We use the <a href="http://knowrob.org/">KnowRob knowledge processing system</a> for creation of the location ontology. In KnowRob, a robot can access specific position information of the perceived objects. The <b>product taxonomy</b> classifies products that were recognized during stocktaking. It is linked to an <b>ingredients classification</b> based on string matching, which is connected to an <b>allergen classification</b>. The product taxonomy is also linked to further product information like name and place of production in <b>product information</b>,<b> product label</b> or <b>product dimensions</b>, i.e. dimensions of product packaging as well as product weight/ filling information. 
All this can be used for shopping applications on mobile phones or smart glasses, for example.

Version 1.2, 1.3 additionally link NonFoodKG to <a href="https://foodkg.github.io/">FoodKG</a> and kitchen objects and products from the KnowRob product taxonomy. With this additional knowledge, robot shopping assistants can integrate NonFoodKG information and applications in the food domain can be implemented. Additionally, a nutrition ontology and a brand information ontology was created and linked to NonFoodKG.

Version 2.0 integrates the <a href="https://foodon.org/">FoodOn food product taxonomy</a> in NonFoodKG, comes with a nutrition ontology from <a href="fdc.nal.usda.gov/">fdc</a> information and provides a user profile and quantity ontology for use in various applications. 

  
# Motivation

Retail stores are competing with online stores. They are aiming at digitization of the shopping experience. We believe that one main advantage of online stores is its connection to Web information. Consumer needs can be unique but also change fast. It would be very time-consuming to manually model consumer preferences in a database. The Semantic Web already offers much information, mainly for food products (e.g. https://world.openfoodfacts.org/ ). Unfortunately, it lacks information about non-food products like allergens contained in cosmetics. Therefore we created this non-food knowledge graph. 
To further enhance the knowledge graph information and in order to being able to apply the included knowledge in example applications, we also integrate location information from a perception-based system, leading to a unique embodiment of knowledge in various consumer and robot applications.

# Querying the knowledge graph

The knowledge graph is publicly available here and on <a href="https://triply.cc/">triply</a> (links see below), many thanks to the <a href="https://krr.cs.vu.nl/">knowledge representation and reasoning group</a> at the Vrije Universiteit Amsterdam.

<h3>Predefined queries</h3> 
<a href="http://grlc.io/api/K4R-IAI/NonFoodKG/SPARQLfiles/"><img src="UseCaseImg/grlc_logo_01.png" width="150" alt="grlc image"/></a>

We created some predefined queries for everyone to test all versions of NonFoodKG via the <a href="http://grlc.io/api/K4R-IAI/NonFoodKG/SPARQLfiles/">NonFoodKG grlc api</a>. grlc is a git repository linked data API constructor that automatically builds Web APIs using shared SPARQL queries <a href="https://github.com/CLARIAH/grlc">(grlc on github)</a>
<h3>Version 1.0</h3> <a href="https://api.krr.triply.cc/datasets/mkumpel/NonFoodKG/services/NonFoodKG/sparql">NonFoodKG via triply SPARQL api</a>
<h3>Version 1.1</h3> <a href="https://api.krr.triply.cc/datasets/mkumpel/TrustNonFoodKG/services/TrustNonFoodKG/sparql">TrustNonFoodKG via triply SPARQL api</a>
<h3>Version 1.2</h3> <a href="https://api.krr.triply.cc/datasets/mkumpel/TrustNonFoodKG/services/FoodToNonFood/sparql">FoodToNonFoodKG via triply SPARQL api</a>



# Disclaimer

This NonFoodKG is made available under the <a href="http://opendatacommons.org/licenses/by/1.0/">Open Data Commons Attribution License</a>.


This knowledge graph has been created by the <a href="https://ai.uni-bremen.de/">Institute for Artificial Intelligence</a> at the University of Bremen. Please contact <a href="https://ai.uni-bremen.de/team/michaela_k%C3%BCmpel">Michaela Kümpel</a> for further info or collaboration: michaela(dot)kuempel(at)uni-bremen(dot)de

<img src="UseCaseImg/ai_logo.png" width="200"/><img align=right src="UseCaseImg/university_new.png" width="200"/>
