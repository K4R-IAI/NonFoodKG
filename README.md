
# Non-FoodKG - A non-Food product knowledge graph for retail applications

Non-FoodKG is a non-food knowledge graph interlinking different ontologies designed for retail, household and robotic applications. It is based on a merged product taxonomy reflecting product classification in grocery stores and drugstores that is linked to a product location ontology created from a robot belief state while performing stocktaking in a retail store. The <b>product location ontology</b> therefore stores inventory data like stock and price of products as well as their positions relative to shelves (instead of coordinates). The <b>product taxonomy</b> classifies products that were recognized during stocktaking. It is linked to an <b>ingredients classification</b> based on string matching, which is connected to an <b>allergen classification</b>. The product taxonomy is also linked to further product information like name and place of production in <b>product information</b> or <b>product dimensions</b>, i.e. dimensions of product packaging as well as product weight/ filling information. 

# Ontologies

Please check out version 1 of the ontologies here:

base file: <a href="https://raw.githubusercontent.com/K4R-IAI/AllIn-NonFoodKG/master/WebGraph/ProductTaxonomy.owl">Product Taxonomy</a>

<a href="https://raw.githubusercontent.com/K4R-IAI/AllIn-NonFoodKG/master/WebGraph/Ingredients.owl">Ingredients Ontology</a>

<a href="https://raw.githubusercontent.com/K4R-IAI/AllIn-NonFoodKG/master/WebGraph/Allergen.owl">Allergen Ontology</a>(linked to ingredients ontology)

<a href="https://raw.githubusercontent.com/K4R-IAI/AllIn-NonFoodKG/master/WebGraph/ProductInfo.owl">Product Information Ontology</a>

<a href="https://raw.githubusercontent.com/K4R-IAI/AllIn-NonFoodKG/master/WebGraph/ProductDimensions.owl">Product Dimensions Ontology</a>

<a href="https://raw.githubusercontent.com/K4R-IAI/AllIn-NonFoodKG/master/WebGraph/ProductToShelf.owl">Product Location Ontology</a>

# Motivation

Retail stores are competing with online stores. They are aiming at digitization of shopping experiences. We believe that one main advantage of online stores is its connection to web information. Consumer needs can be unique but also change fast. It would be very time-consuming to manually model consumer preferences in a database. The Semantic Web already offers much information, mainly for food products (e.g. https://world.openfoodfacts.org/ ). Unfortunately, we could not find much information about non-food products like allergens contained in cosmetics. Therefore we decided to create this non-food knowledge graph to model cosumer preferences. For future applications we also created ontologies with further product information.
We have just started working on this knowledge graph and are continuously adding more ontologies.

# Use Cases

<b>Highlighting consumer preferences</b>


<b>Routing to product destination</b>


This knowledge graph has been created by the Institute for Artificial Intelligence at the University of Bremen. Please contact Michaela Kümpel for further info or collaboration: michaela(dot)kuempel(at)uni-bremen(dot)de
