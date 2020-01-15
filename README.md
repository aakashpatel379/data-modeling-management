## Data Modeling - Management

### Overview

Data Management project based on Kaggle datasets on multidisciplinary domains like Economy, School and Vehicle Sales. Performed Exploratory Data Analysis, Cleaning, Modelling and Design to arrive on final schema. Final design is normalized in 3NF.

### Datasets Used

• **Name:** New motor vehicle sales, by type of vehicle
**URL:** https://open.canada.ca/data/en/dataset/f6e7e871-79b7-49e1-90a2-e3c913f1951d
**Reason for selection:** This dataset provides information about sales of new vehicles
annually and thus it can serve to better understand sales demographic for new vehicles
across Canada.

• **Name:** Manufacturers' sales, inventories, orders and inventory to sales ratios, by industry
(dollars unless otherwise noted)
**URL:** https://open.canada.ca/data/en/dataset/2e6f30d9-857d-4364-8611-5625b59562be
**Reason for selection:** This dataset provides industry based financial information about
manufacturer’s sales, new orders, unfilled orders, raw materials, goods or work in process,
finished goods, total inventories, inventory to sales ratios and finished goods to sales ratios.
All this information is useful for study financial performance of manufacturing domain
linked to the transport industry. Thus, it can link Economics and Industry domain to the
Transport domain.

• **Name:** Sales of fuel used for road motor vehicles, annual
**URL:** https://open.canada.ca/data/en/dataset/6797dd39-8a2d-4ec3-b285-6123ef61699b
**Reason for selection:** This dataset provides information about fuel sales for road motor
vehicles and can be utilised to know fuel consumption across the provinces.

• **Name:** School board revenues, by direct source of funds and geography
**URL:** https://open.canada.ca/data/en/dataset/7dabde2e-d383-490e-b8e4-acfa9e88edec
**Reason for selection:** This dataset provides statistical information about revenues by school
boards by their source of funds and geography. It can be useful to know revenues to school
boards from different sources.

• **Name:** School board expenditures, by function and economic classification
**URL:** https://open.canada.ca/data/en/dataset/c5e55cde-19fb-4dda-b36f-bcee966fb430
**Reason for selection:** This dataset provides puts forward statistical information about
expenses of school boards. It can be utilised to know trends of school board expenses by
function and economic classification

• **Name:** Combined public and private expenditure on educational institutions, by level of
education
**URL:** https://open.canada.ca/data/en/dataset/ed5b6abd-5f22-467b-b3a1-e1ff5a689225
**Reason for selection:** This dataset provides public and private expenditure statistics of
educational institutions according to level of education. It is useful to understand total
expenditure on education.

• **Name:** Wholesale trade, sales
**URL:** https://open.canada.ca/data/en/dataset/57fff1ed-1240-4004-9b37-8c43c0fc249a
**Reason for selection:** This dataset can be utilised to study and understand wholesale trade
sales for different provinces as per the NAICS (North American Industry Classification
system).

• **Name:** Trade in goods by exporter characteristics, by enterprise employment size and
export size
**URL:** https://open.canada.ca/data/en/dataset/700c4c4e-66f1-46be-9d47-cf8b5797f7c9
**Reason for selection:** This dataset can be used to evaluate goods trade information of
Canada by exporter characteristics, enterprise employment size and export size.

### Initial and Final Design

**Intial Design**
<img src="Initial_Design.jpg" width=800/>

The above entity relationship diagram shows how different entities where found to be related to each other.
It describes Entities in rectangle shape and their attributes inside oval. Attributes are shown only for few
major entities after initial database design. It helps us to visualise and get a glimpse of how database is
going to get developed. Attributes underlined show primary keys for the entities. Cardinalities are based on
data available from the datasets selected. For instance, Measurement and Scale are related to some entities
using one to many relationships, which is according to the data available and which may sometimes
contradict general intuitive sense one may have after before careful examination.
The flaws / design issues in the diagram as below:
• The data for some entity is time variant data. There may arise changes in the design later,
as new data gets added in the newer format.
• There is a Fan trap issue for Scale and Measurement entities. Both these entities are related
to many other entities with one to many relationships. Thus, they pose a fan trap issue to
the design.

**Final Design**
<img src="Final_Design_ERD.png" width=800/>

### License
Aakash Patel - B00807065
