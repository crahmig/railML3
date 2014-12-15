railML3
=======

Development of the new railML 3 version.

railML
------

(cp. [9]): railML is a data exchange format for interoperability in railway industry applications. railML (railway mark-up language) is a common exchange format, which employs the systematic of XML for the description of rail-specific data. railML enables the exchange of railway data between internal and external railway applications. railML is developed within the so-called “railML consortium” from railML.org. It is an open source exchange format; the modelling language of railML is English. A free registration on railML is mandatory for the usage and download of railML schemes.

railML 3 and the UIC RailTopoModel
----------------------------------

Why do we need railML 3 (see [1])? In the past years, resulting from discussions in the forum as well as from application examples, we discovered some infrastructure elements and parameters, which are difficult to define in the railML 2.x model. Some of these aspects have been transformed into Trac tickets that can be found in [2]. The underlaying topology is considered to be a central problem as it is not flexible enough for a modular modelling of coordinates and track elements.
Last year, the railML partner TrafIt (cf. [3]) analysed the requirements for a generic railway topology model considering the requirements of all the different stakeholders and their applications as well as existing model examples. This feasibility study was assigned and financed by the UIC and the result has been presented at the 24th railML.org conference in Paris on September 18, 2013 (cp.[4]). The final report of this study is available at [5].

Based on the results of the feasibility study, the French infrastructure manager RFF, together with the Belgium infrastructure manager Infrabel, initiated the development of a first version for a generic railway topology model. I reviewed the development process as the railML infrastructure coordinator. The result named as UIC RailTopoModel, which is documented in [6], can be considered more as a first than a final version of a new railway topology approach. Now it is up to all of you to discuss the model here in the forum. It is our aim to create a solution that all of you can understand, support and apply, and therefore we need your feedback on the development. Please share it with the community here in the forum.

What is the UIC RailTopoModel? This model is a topology approach based on a "connexity graph" as described in [7]. Simplified, this "connexity graph" is a node-edge-model where nodes and edges are both modelled as "NetElements" linked by "Connections". The node-edge-model itself is a common concept of graph theory (cf. [8]). A major concern of the model, which has been already pointed out in the feasibility study, is the generic character of the topology model providing the same structure for different levels of detail. Further, the different levels of detail should be convertible using aggregation methods.
The UIC RailTopoModel is considered to be one central component of the railML 3.0 infrastructure model. However, the railway network's topology is only one part of the basic layer, while the coordinate positions, which are required by many applications focusing on geometry or visualization, form the other part. Last, but not least, we should not forget that there are also applications, which may exchange infrastructure data without both coordinates and topology, based on railML. Therefore, the UIC RailTopoModel is only one component of the future railML 3.0 infrastructure approach, although a very central one.

[1] http://railml.org//index.php/railml3-entwicklung.html

[2] http://trac.railml.org/query?version=3.0&col=id&col=summary&col=status&col=owner&col=type&col=priority&col=milestone&order=priority

[3] http://railml.org//index.php/entwickler.html?show=48

[4] http://documents.railml.org/events/slides/2013-09-17_uic_nissi-erim_presentation.pdf

[5] http://railml.org/tl_files/railML.org/documents/science/270913_trafIT_FinalReportFeasibilityStudyRailTopoModel.pdf

[6] http://railml.org/tl_files/railML.org/documents/science/201213_UIC_RailTopoModel_DraftDec13.pdf

[7] http://library.witpress.com/pages/PaperInfo.asp?PaperID=19759

[8] http://en.wikipedia.org/wiki/Graph_(mathematics) 

[9] http://en.wikipedia.org/wiki/RailML
