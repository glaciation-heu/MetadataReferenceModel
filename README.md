The Metadata Reference Model for the EU GLACIATION Project
==========================================================

Release: "2024-07-20"
---------------------

Modified on: "2024-10-30"

This version:

[https://glaciation-project.eu/MetadataReferenceModel/1.1.0/](https://glaciation-project.eu/MetadataReferenceModel/1.1.0/)

Latest version:

[https://glaciation-project.eu/MetadataReferenceModel](https://glaciation-project.eu/MetadataReferenceModel)

Previous version:

[https://glaciation-project.eu/MetadataReferenceModel/1.0.0/](https://glaciation-project.eu/MetadataReferenceModel/1.0.0/)

Revision:

1.1.0

Authors:

"Michalis Mountantonakis", "Panagiotis Papadakos", "Rigo Wenning"

Contributors:

"Konstantin Tatarnikov", "Guangyuan Piao", "Alessio Chellini", "Paolo Tartara", "Péter Forgács", " Jonas Böhler"

Download serialization:

 [![JSON-LD](https://img.shields.io/badge/Format-JSON_LD-blue.svg)](ontology.jsonld)[![RDF/XML](https://img.shields.io/badge/Format-RDF/XML-blue.svg)](ontology.owl) [![N-Triples](https://img.shields.io/badge/Format-N_Triples-blue.svg)](ontology.nt) [![TTL](https://img.shields.io/badge/Format-TTL-blue.svg)](ontology.ttl)

License:

[![https://www.apache.org/licenses/LICENSE-2.0](https://img.shields.io/badge/License-https://www.apache.org/licenses/LICENSE_2.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

Visualization:

[![Visualize with WebVowl](https://img.shields.io/badge/Visualize_with-WebVowl-blue.svg)](webvowl/index.html#)

Cite as:

"Michalis Mountantonakis", "Panagiotis Papadakos", "Rigo Wenning". The Metadata Reference Model for the EU GLACIATION Project. Revision: 1.1.0. Retrieved from: https://glaciation-project.eu/MetadataReferenceModel/1.1.0/

[Provenance of this page](provenance/provenance-en.html)

* * *

peerReviewed

Abstract
--------

The Glaciation Reference Metadata Model (GLC-MRM) provides a conceptual model that allows making data ingestion and data processing interoperable for all the use cases of the Glaciation project. The model can be considered as a general conceptualization of a tasks scheduling problem that considers various measuring indicators over the deployed resources.

GLACIATION Metadata Reference Model: Overview back to [ToC](#toc)
-----------------------------------------------------------------

This ontology has the following classes and properties.

#### Classes

*   [AggregatedMeasurement](#AggregatedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#AggregatedMeasurement")
*   [Aspect](#Aspect "https://glaciation-project.eu/MetadataReferenceModel#Aspect")
*   [AssignedTask](#AssignedTask "https://glaciation-project.eu/MetadataReferenceModel#AssignedTask")
*   [Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class")
*   [Constraint](#Constraint "https://glaciation-project.eu/MetadataReferenceModel#Constraint")
*   [Electrical Grid](#ElectricalGrid "https://glaciation-project.eu/MetadataReferenceModel#ElectricalGrid")
*   [Energy Power Generation Resource](#EnergyPowerGenerationResource "https://glaciation-project.eu/MetadataReferenceModel#EnergyPowerGenerationResource")
*   [Energy Resource](#EnergyResource "https://glaciation-project.eu/MetadataReferenceModel#EnergyResource")
*   [HardConstraint](#HardConstraint "https://glaciation-project.eu/MetadataReferenceModel#HardConstraint")
*   [Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement")
*   [MeasurementProperty](#MeasurementProperty "https://glaciation-project.eu/MetadataReferenceModel#MeasurementProperty")
*   [MeasurementUnit](#MeasurementUnit "https://glaciation-project.eu/MetadataReferenceModel#MeasurementUnit")
*   [MeasuringResource](#MeasuringResource "https://glaciation-project.eu/MetadataReferenceModel#MeasuringResource")
*   [Monitor](#Monitor "https://glaciation-project.eu/MetadataReferenceModel#Monitor")
*   [NonWorkProducingResource](#NonWorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#NonWorkProducingResource")
*   [Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource")
*   [Scheduler](#Scheduler "https://glaciation-project.eu/MetadataReferenceModel#Scheduler")
*   [Site](#Site "https://glaciation-project.eu/MetadataReferenceModel#Site")
*   [SoftConstraint](#SoftConstraint "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraint")
*   [SoftConstraintComposition](#SoftConstraintComposition "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraintComposition")
*   [Status](#Status "https://glaciation-project.eu/MetadataReferenceModel#Status")
*   [SubmittedTask](#SubmittedTask "https://glaciation-project.eu/MetadataReferenceModel#SubmittedTask")
*   [Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task")
*   [WorkProducingResource](#WorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource")


#### Object Properties

*   [assigns](#assigns "https://glaciation-project.eu/MetadataReferenceModel#assigns")
*   [composedBy](#composedBy "https://glaciation-project.eu/MetadataReferenceModel#composedBy")
*   [consumes](#consumes "https://glaciation-project.eu/MetadataReferenceModel#consumes")
*   [consumesEnergyFrom](#consumesEnergyFrom "https://glaciation-project.eu/MetadataReferenceModel#consumesEnergyFrom")
*   [hasAspect](#hasAspect "https://glaciation-project.eu/MetadataReferenceModel#hasAspect")
*   [hasComposition](#hasComposition "https://glaciation-project.eu/MetadataReferenceModel#hasComposition")
*   [hasConstraint](#hasConstraint "https://glaciation-project.eu/MetadataReferenceModel#hasConstraint")
*   [hasResourceMeasurement](#hasResourceMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasResourceMeasurement")
*   [hasStatus](#hasStatus "https://glaciation-project.eu/MetadataReferenceModel#hasStatus")
*   [hasSubResource](#hasSubResource "https://glaciation-project.eu/MetadataReferenceModel#hasSubResource")
*   [hasTaskMeasurement](#hasTaskMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskMeasurement")
*   [hasTaskPredictedMeasurement](#hasTaskPredictedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskPredictedMeasurement")
*   [hasTaskRealizedMeasurement](#hasTaskRealizedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskRealizedMeasurement")
*   [isLocatedIn](#isLocatedIn "https://glaciation-project.eu/MetadataReferenceModel#isLocatedIn")
*   [makesMeasurement](#makesMeasurement "https://glaciation-project.eu/MetadataReferenceModel#makesMeasurement")
*   [manages](#manages "https://glaciation-project.eu/MetadataReferenceModel#manages")
*   [measuredIn](#measuredIn "https://glaciation-project.eu/MetadataReferenceModel#measuredIn")
*   [monitors](#monitors "https://glaciation-project.eu/MetadataReferenceModel#monitors")
*   [produces](#produces "https://glaciation-project.eu/MetadataReferenceModel#produces")
*   [relatesToConstraint](#relatesToConstraint "https://glaciation-project.eu/MetadataReferenceModel#relatesToConstraint")
*   [relatesToMeasurementProperty](#relatesToMeasurementProperty "https://glaciation-project.eu/MetadataReferenceModel#relatesToMeasurementProperty")
*   [reschedules](#reschedules "https://glaciation-project.eu/MetadataReferenceModel#reschedules")
*   [scheduledBy](#scheduledBy "https://glaciation-project.eu/MetadataReferenceModel#scheduledBy")
*   [triggersReschedule](#triggersReschedule "https://glaciation-project.eu/MetadataReferenceModel#triggersReschedule")

#### Data Properties

*   [endingInterval](#endingInterval "https://glaciation-project.eu/MetadataReferenceModel#endingInterval")
*   [endTime](#endTime "https://glaciation-project.eu/MetadataReferenceModel#endTime")
*   [hasAggregatedFuntion](#hasAggregatedFuntion "https://glaciation-project.eu/MetadataReferenceModel#hasAggregatedFuntion")
*   [hasConfiguration](#hasConfiguration "https://glaciation-project.eu/MetadataReferenceModel#hasConfiguration")
*   [hasDescription](#hasDescription "https://glaciation-project.eu/MetadataReferenceModel#hasDescription")
*   [hasID](#hasID "https://glaciation-project.eu/MetadataReferenceModel#hasID")
*   [hasTimestamp](#hasTimestamp "https://glaciation-project.eu/MetadataReferenceModel#hasTimestamp")
*   [hasValue](#hasValue "https://glaciation-project.eu/MetadataReferenceModel#hasValue")
*   [startingInterval](#startingInterval "https://glaciation-project.eu/MetadataReferenceModel#startingInterval")
*   [startTime](#startTime "https://glaciation-project.eu/MetadataReferenceModel#startTime")
*   [statusCode](#statusCode "https://glaciation-project.eu/MetadataReferenceModel#statusCode")
*   [timeStepResolution](#timeStepResolution "https://glaciation-project.eu/MetadataReferenceModel#timeStepResolution")

#### Annotation Properties

*   [abstract](#http://purl.org/dc/terms/abstract "http://purl.org/dc/terms/abstract")
*   [contributor](#http://purl.org/dc/elements/1.1/contributor "http://purl.org/dc/elements/1.1/contributor")
*   [created](#http://purl.org/dc/terms/created "http://purl.org/dc/terms/created")
*   [creator](#http://purl.org/dc/elements/1.1/creator "http://purl.org/dc/elements/1.1/creator")
*   [description](#http://purl.org/dc/terms/description "http://purl.org/dc/terms/description")
*   [issued](#http://purl.org/dc/elements/1.1/issued "http://purl.org/dc/elements/1.1/issued")
*   [license](#http://purl.org/dc/terms/license "http://purl.org/dc/terms/license")
*   [preferred Namespace Uri](#http://purl.org/vocab/vann/preferredNamespaceUri "http://purl.org/vocab/vann/preferredNamespaceUri")
*   [preffered Namespace Prefix](#http://purl.org/vocab/vann/prefferedNamespacePrefix "http://purl.org/vocab/vann/prefferedNamespacePrefix")
*   [status](#http://purl.org/ontology/bibo/status "http://purl.org/ontology/bibo/status")
*   [title](#http://purl.org/dc/terms/title "http://purl.org/dc/terms/title")

GLACIATION Metadata Reference Model: Description back to [ToC](#toc)
--------------------------------------------------------------------

The GLACIATION platform develops a novel Distributed Knowledge Graph (DKG) that stretches across the edge-core-cloud architecture to reduce energy consumption, improving data processing and optimizing data movement operations. Towards this aim, the platform needs to consume the data and metadata that are fed into the DKG. The metadata can affect and inform the decision-making processes in the GLACIATION architecture and introduces the GLACIATION Metadata Reference Model that will be used for modelling the metadata in the DKG. The GLACIATION Reference Metadata Model makes data ingestion and processing interoperable inside the GLACIATION platform. Linked Data allows for a high level of flexibility and to tackle the variety and merging issues that emerge in heterogenous environments, especially due to the wide range of sensors and other data sources that the platform may integrate. The GLACIATION Reference Metadata Model is tailored to fit the specific purposes of the GLACIATION platform, while the GLACIATION use cases define the scope of the model for better interoperability. There are common metadata challenges for all use cases. This stems from the use of the Kubernetes orchestration system as a basis for the GLACIATION platform. In addition, common to the platform is the ingestion of data from other sources into the DKG that can then be used to affect processing decisions. There are direct data flows from sensors within the system, but also data and metadata from sources external to the system. This allows the system to react e.g. to environmental situations like weather or temperature, but also to requirements concerning security or privacy. Exemplary uses and specializations of the reference model to the GLACIATION use cases are also provided. The GLACIATION Metadata Reference Model can be used for scheduling and performing tasks. The model can be considered as a general conceptualization of a tasks scheduling problem that considers various measuring indicators over the deployed resources. It captures the assignment of time-constrained tasks to time constrained and energy consuming resources, that can satisfy various hard and soft constraints, even compositions of such constraints. The tasks can be monitored through various measuring resources using a variety of single or aggregated, predicted or real measurements The model is generic, by being both domain and application independent, describing the scheduling tasks, without providing specific solutions on how they can be solved. It can be easily adjusted to each of the current three GLACIATION use cases, covering also the Kubernetes orchestration and its Telemetry System deployed by the project. The proposed model makes it feasible to answer the competency queries defined by each of the Glaciation's use case.

Cross-reference for GLACIATION Metadata Reference Model classes, object properties and data properties back to [ToC](#toc)
--------------------------------------------------------------------------------------------------------------------------

This section provides details for each class and property defined by GLACIATION Metadata Reference Model.

### Classes

*   [AggregatedMeasurement](#AggregatedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#AggregatedMeasurement")
*   [Aspect](#Aspect "https://glaciation-project.eu/MetadataReferenceModel#Aspect")
*   [AssignedTask](#AssignedTask "https://glaciation-project.eu/MetadataReferenceModel#AssignedTask")
*   [Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class")
*   [Constraint](#Constraint "https://glaciation-project.eu/MetadataReferenceModel#Constraint")
*   [Electrical Grid](#ElectricalGrid "https://glaciation-project.eu/MetadataReferenceModel#ElectricalGrid")
*   [Energy Power Generation Resource](#EnergyPowerGenerationResource "https://glaciation-project.eu/MetadataReferenceModel#EnergyPowerGenerationResource")
*   [Energy Resource](#EnergyResource "https://glaciation-project.eu/MetadataReferenceModel#EnergyResource")
*   [HardConstraint](#HardConstraint "https://glaciation-project.eu/MetadataReferenceModel#HardConstraint")
*   [Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement")
*   [MeasurementProperty](#MeasurementProperty "https://glaciation-project.eu/MetadataReferenceModel#MeasurementProperty")
*   [MeasurementUnit](#MeasurementUnit "https://glaciation-project.eu/MetadataReferenceModel#MeasurementUnit")
*   [MeasuringResource](#MeasuringResource "https://glaciation-project.eu/MetadataReferenceModel#MeasuringResource")
*   [Monitor](#Monitor "https://glaciation-project.eu/MetadataReferenceModel#Monitor")
*   [NonWorkProducingResource](#NonWorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#NonWorkProducingResource")
*   [Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource")
*   [Scheduler](#Scheduler "https://glaciation-project.eu/MetadataReferenceModel#Scheduler")
*   [Site](#Site "https://glaciation-project.eu/MetadataReferenceModel#Site")
*   [SoftConstraint](#SoftConstraint "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraint")
*   [SoftConstraintComposition](#SoftConstraintComposition "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraintComposition")
*   [Status](#Status "https://glaciation-project.eu/MetadataReferenceModel#Status")
*   [SubmittedTask](#SubmittedTask "https://glaciation-project.eu/MetadataReferenceModel#SubmittedTask")
*   [Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task")
*   [WorkProducingResource](#WorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource")

### AggregatedMeasurementc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#AggregatedMeasurement

Represents any AggregatedMeasurement, by using an AggregatedFunction, a time interval and time step resolution.

has super-classes

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

is in domain of

[endingInterval](#endingInterval "https://glaciation-project.eu/MetadataReferenceModel#endingInterval") dp, [hasAggregatedFuntion](#hasAggregatedFuntion "https://glaciation-project.eu/MetadataReferenceModel#hasAggregatedFuntion") dp, [startingInterval](#startingInterval "https://glaciation-project.eu/MetadataReferenceModel#startingInterval") dp, [timeStepResolution](#timeStepResolution "https://glaciation-project.eu/MetadataReferenceModel#timeStepResolution") dp

### Aspectc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Aspect

It describes the Aspect of a Contstraint, e.g., time, power consumption.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

is in range of

[hasAspect](#hasAspect "https://glaciation-project.eu/MetadataReferenceModel#hasAspect") op

### AssignedTaskc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#AssignedTask

An AssignedTask that will be performed by using some Resources and will be based on some Constraints.

has super-classes

[Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

is in domain of

[consumes](#consumes "https://glaciation-project.eu/MetadataReferenceModel#consumes") op, [produces](#produces "https://glaciation-project.eu/MetadataReferenceModel#produces") op

is in range of

[assigns](#assigns "https://glaciation-project.eu/MetadataReferenceModel#assigns") op, [monitors](#monitors "https://glaciation-project.eu/MetadataReferenceModel#monitors") op, [reschedules](#reschedules "https://glaciation-project.eu/MetadataReferenceModel#reschedules") op

### Classc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Class

A generic Class for the GLACIATION project

has sub-classes

[Aspect](#Aspect "https://glaciation-project.eu/MetadataReferenceModel#Aspect") c, [Constraint](#Constraint "https://glaciation-project.eu/MetadataReferenceModel#Constraint") c, [Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c, [MeasurementProperty](#MeasurementProperty "https://glaciation-project.eu/MetadataReferenceModel#MeasurementProperty") c, [MeasurementUnit](#MeasurementUnit "https://glaciation-project.eu/MetadataReferenceModel#MeasurementUnit") c, [MeasuringResource](#MeasuringResource "https://glaciation-project.eu/MetadataReferenceModel#MeasuringResource") c, [Monitor](#Monitor "https://glaciation-project.eu/MetadataReferenceModel#Monitor") c, [Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c, [Scheduler](#Scheduler "https://glaciation-project.eu/MetadataReferenceModel#Scheduler") c, [Site](#Site "https://glaciation-project.eu/MetadataReferenceModel#Site") c, [SoftConstraintComposition](#SoftConstraintComposition "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraintComposition") c, [Status](#Status "https://glaciation-project.eu/MetadataReferenceModel#Status") c, [Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

is in domain of

[hasConfiguration](#hasConfiguration "https://glaciation-project.eu/MetadataReferenceModel#hasConfiguration") dp, [hasDescription](#hasDescription "https://glaciation-project.eu/MetadataReferenceModel#hasDescription") dp, [hasID](#hasID "https://glaciation-project.eu/MetadataReferenceModel#hasID") dp, [hasStatus](#hasStatus "https://glaciation-project.eu/MetadataReferenceModel#hasStatus") op

### Constraintc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Constraint

For representing the Constraint(s) of a Task.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

has sub-classes

[HardConstraint](#HardConstraint "https://glaciation-project.eu/MetadataReferenceModel#HardConstraint") c, [SoftConstraint](#SoftConstraint "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraint") c

is in domain of

[hasAspect](#hasAspect "https://glaciation-project.eu/MetadataReferenceModel#hasAspect") op

is in range of

[hasConstraint](#hasConstraint "https://glaciation-project.eu/MetadataReferenceModel#hasConstraint") op, [relatesToConstraint](#relatesToConstraint "https://glaciation-project.eu/MetadataReferenceModel#relatesToConstraint") op

### Electrical Gridc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#ElectricalGrid

It represents an electrical grid

has super-classes

[Energy Resource](#EnergyResource "https://glaciation-project.eu/MetadataReferenceModel#EnergyResource") c

is in range of

[consumesEnergyFrom](#consumesEnergyFrom "https://glaciation-project.eu/MetadataReferenceModel#consumesEnergyFrom") op

### Energy Power Generation Resourcec back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#EnergyPowerGenerationResource

It represents an energy resource that generates power

has super-classes

[Energy Resource](#EnergyResource "https://glaciation-project.eu/MetadataReferenceModel#EnergyResource") c

### Energy Resourcec back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#EnergyResource

It represents an energy resource

has super-classes

[WorkProducingResource](#WorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource") c

has sub-classes

[Electrical Grid](#ElectricalGrid "https://glaciation-project.eu/MetadataReferenceModel#ElectricalGrid") c, [Energy Power Generation Resource](#EnergyPowerGenerationResource "https://glaciation-project.eu/MetadataReferenceModel#EnergyPowerGenerationResource") c

### HardConstraintc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#HardConstraint

For representing the HardConstraints of a Task.

has super-classes

[Constraint](#Constraint "https://glaciation-project.eu/MetadataReferenceModel#Constraint") c

### Measurementc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Measurement

Represents any Measurement, e.g., for energy.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

has sub-classes

[AggregatedMeasurement](#AggregatedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#AggregatedMeasurement") c

is in domain of

[hasTimestamp](#hasTimestamp "https://glaciation-project.eu/MetadataReferenceModel#hasTimestamp") dp, [hasValue](#hasValue "https://glaciation-project.eu/MetadataReferenceModel#hasValue") dp, [measuredIn](#measuredIn "https://glaciation-project.eu/MetadataReferenceModel#measuredIn") op, [relatesToConstraint](#relatesToConstraint "https://glaciation-project.eu/MetadataReferenceModel#relatesToConstraint") op, [relatesToMeasurementProperty](#relatesToMeasurementProperty "https://glaciation-project.eu/MetadataReferenceModel#relatesToMeasurementProperty") op

is in range of

[hasResourceMeasurement](#hasResourceMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasResourceMeasurement") op, [hasTaskMeasurement](#hasTaskMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskMeasurement") op, [hasTaskPredictedMeasurement](#hasTaskPredictedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskPredictedMeasurement") op, [hasTaskRealizedMeasurement](#hasTaskRealizedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskRealizedMeasurement") op, [makesMeasurement](#makesMeasurement "https://glaciation-project.eu/MetadataReferenceModel#makesMeasurement") op

### MeasurementPropertyc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#MeasurementProperty

Represents a MeasurementProperty, e.g., allocated CPU, energy, etc.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

is in range of

[relatesToMeasurementProperty](#relatesToMeasurementProperty "https://glaciation-project.eu/MetadataReferenceModel#relatesToMeasurementProperty") op

### MeasurementUnitc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#MeasurementUnit

Represents a MeasurementUnit, e.g., Kwh.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

is in range of

[measuredIn](#measuredIn "https://glaciation-project.eu/MetadataReferenceModel#measuredIn") op

### MeasuringResourcec back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#MeasuringResource

It represents any WorkProducingResource that can perform Measurements.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c, [WorkProducingResource](#WorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource") c

is in domain of

[makesMeasurement](#makesMeasurement "https://glaciation-project.eu/MetadataReferenceModel#makesMeasurement") op

### Monitorc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Monitor

Represents an entity that monitors an AssignedTask.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

is in domain of

[monitors](#monitors "https://glaciation-project.eu/MetadataReferenceModel#monitors") op, [triggersReschedule](#triggersReschedule "https://glaciation-project.eu/MetadataReferenceModel#triggersReschedule") op

### NonWorkProducingResourcec back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#NonWorkProducingResource

It represents any NonWorkProducingResource (e.g., dataset).

has super-classes

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

### Resourcec back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Resource

It represents any Resource.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

has sub-classes

[NonWorkProducingResource](#NonWorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#NonWorkProducingResource") c, [WorkProducingResource](#WorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource") c

is in domain of

[hasResourceMeasurement](#hasResourceMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasResourceMeasurement") op, [hasSubResource](#hasSubResource "https://glaciation-project.eu/MetadataReferenceModel#hasSubResource") op

is in range of

[consumes](#consumes "https://glaciation-project.eu/MetadataReferenceModel#consumes") op, [hasSubResource](#hasSubResource "https://glaciation-project.eu/MetadataReferenceModel#hasSubResource") op, [manages](#manages "https://glaciation-project.eu/MetadataReferenceModel#manages") op, [produces](#produces "https://glaciation-project.eu/MetadataReferenceModel#produces") op

is disjoint with

[Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

### Schedulerc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Scheduler

Responsible for Scheduling a SubmittedTask and for managing the Resources.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

is in domain of

[assigns](#assigns "https://glaciation-project.eu/MetadataReferenceModel#assigns") op, [manages](#manages "https://glaciation-project.eu/MetadataReferenceModel#manages") op, [reschedules](#reschedules "https://glaciation-project.eu/MetadataReferenceModel#reschedules") op

is in range of

[scheduledBy](#scheduledBy "https://glaciation-project.eu/MetadataReferenceModel#scheduledBy") op, [triggersReschedule](#triggersReschedule "https://glaciation-project.eu/MetadataReferenceModel#triggersReschedule") op

### Sitec back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Site

It represents any Site, e.g., a location, an island, etc.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

is in range of

[isLocatedIn](#isLocatedIn "https://glaciation-project.eu/MetadataReferenceModel#isLocatedIn") op

### SoftConstraintc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#SoftConstraint

For representing the SoftConstraints of a Task.

has super-classes

[Constraint](#Constraint "https://glaciation-project.eu/MetadataReferenceModel#Constraint") c

is in range of

[composedBy](#composedBy "https://glaciation-project.eu/MetadataReferenceModel#composedBy") op

### SoftConstraintCompositionc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#SoftConstraintComposition

It describes the composition of SoftConstraints, e.g., the order of soft constraings according to a given preference priority, Pareto, Pareto optimal, etc.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

is in domain of

[composedBy](#composedBy "https://glaciation-project.eu/MetadataReferenceModel#composedBy") op

is in range of

[hasComposition](#hasComposition "https://glaciation-project.eu/MetadataReferenceModel#hasComposition") op

### Statusc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Status

Represents information about a specific Status over a given time interval.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

is in domain of

[endTime](#endTime "https://glaciation-project.eu/MetadataReferenceModel#endTime") dp, [startTime](#startTime "https://glaciation-project.eu/MetadataReferenceModel#startTime") dp, [statusCode](#statusCode "https://glaciation-project.eu/MetadataReferenceModel#statusCode") dp

is in range of

[hasStatus](#hasStatus "https://glaciation-project.eu/MetadataReferenceModel#hasStatus") op

### SubmittedTaskc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#SubmittedTask

A Submitted Task that will be processed by a Scheduler.

has super-classes

[Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

is in domain of

[scheduledBy](#scheduledBy "https://glaciation-project.eu/MetadataReferenceModel#scheduledBy") op

### Taskc back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#Task

It describes any Task that has Constraints and a Status.

has super-classes

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

has sub-classes

[AssignedTask](#AssignedTask "https://glaciation-project.eu/MetadataReferenceModel#AssignedTask") c, [SubmittedTask](#SubmittedTask "https://glaciation-project.eu/MetadataReferenceModel#SubmittedTask") c

is in domain of

[hasComposition](#hasComposition "https://glaciation-project.eu/MetadataReferenceModel#hasComposition") op, [hasConstraint](#hasConstraint "https://glaciation-project.eu/MetadataReferenceModel#hasConstraint") op, [hasTaskMeasurement](#hasTaskMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskMeasurement") op, [hasTaskPredictedMeasurement](#hasTaskPredictedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskPredictedMeasurement") op, [hasTaskRealizedMeasurement](#hasTaskRealizedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskRealizedMeasurement") op

is disjoint with

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

### WorkProducingResourcec back to [ToC](#toc) or [Class ToC](#classes)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource

It represents any WorkProducingResource, e.g., a node, a CPU, etc.

has super-classes

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

has sub-classes

[Energy Resource](#EnergyResource "https://glaciation-project.eu/MetadataReferenceModel#EnergyResource") c, [MeasuringResource](#MeasuringResource "https://glaciation-project.eu/MetadataReferenceModel#MeasuringResource") c

is in domain of

[consumesEnergyFrom](#consumesEnergyFrom "https://glaciation-project.eu/MetadataReferenceModel#consumesEnergyFrom") op, [isLocatedIn](#isLocatedIn "https://glaciation-project.eu/MetadataReferenceModel#isLocatedIn") op

### Object Properties

*   [assigns](#assigns "https://glaciation-project.eu/MetadataReferenceModel#assigns")
*   [composedBy](#composedBy "https://glaciation-project.eu/MetadataReferenceModel#composedBy")
*   [consumes](#consumes "https://glaciation-project.eu/MetadataReferenceModel#consumes")
*   [consumesEnergyFrom](#consumesEnergyFrom "https://glaciation-project.eu/MetadataReferenceModel#consumesEnergyFrom")
*   [hasAspect](#hasAspect "https://glaciation-project.eu/MetadataReferenceModel#hasAspect")
*   [hasComposition](#hasComposition "https://glaciation-project.eu/MetadataReferenceModel#hasComposition")
*   [hasConstraint](#hasConstraint "https://glaciation-project.eu/MetadataReferenceModel#hasConstraint")
*   [hasResourceMeasurement](#hasResourceMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasResourceMeasurement")
*   [hasStatus](#hasStatus "https://glaciation-project.eu/MetadataReferenceModel#hasStatus")
*   [hasSubResource](#hasSubResource "https://glaciation-project.eu/MetadataReferenceModel#hasSubResource")
*   [hasTaskMeasurement](#hasTaskMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskMeasurement")
*   [hasTaskPredictedMeasurement](#hasTaskPredictedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskPredictedMeasurement")
*   [hasTaskRealizedMeasurement](#hasTaskRealizedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskRealizedMeasurement")
*   [isLocatedIn](#isLocatedIn "https://glaciation-project.eu/MetadataReferenceModel#isLocatedIn")
*   [makesMeasurement](#makesMeasurement "https://glaciation-project.eu/MetadataReferenceModel#makesMeasurement")
*   [manages](#manages "https://glaciation-project.eu/MetadataReferenceModel#manages")
*   [measuredIn](#measuredIn "https://glaciation-project.eu/MetadataReferenceModel#measuredIn")
*   [monitors](#monitors "https://glaciation-project.eu/MetadataReferenceModel#monitors")
*   [produces](#produces "https://glaciation-project.eu/MetadataReferenceModel#produces")
*   [relatesToConstraint](#relatesToConstraint "https://glaciation-project.eu/MetadataReferenceModel#relatesToConstraint")
*   [relatesToMeasurementProperty](#relatesToMeasurementProperty "https://glaciation-project.eu/MetadataReferenceModel#relatesToMeasurementProperty")
*   [reschedules](#reschedules "https://glaciation-project.eu/MetadataReferenceModel#reschedules")
*   [scheduledBy](#scheduledBy "https://glaciation-project.eu/MetadataReferenceModel#scheduledBy")
*   [triggersReschedule](#triggersReschedule "https://glaciation-project.eu/MetadataReferenceModel#triggersReschedule")

### assignsop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#assigns

A relationship between a Scheduler and an AssignedTask.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Scheduler](#Scheduler "https://glaciation-project.eu/MetadataReferenceModel#Scheduler") c

has range

[AssignedTask](#AssignedTask "https://glaciation-project.eu/MetadataReferenceModel#AssignedTask") c

### composedByop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#composedBy

For keeping information about the SoftConstraints that are included in a Composition.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[SoftConstraintComposition](#SoftConstraintComposition "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraintComposition") c

has range

[SoftConstraint](#SoftConstraint "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraint") c

### consumesop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#consumes

A property for recording the Resource(s) of each AssignedTask.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[AssignedTask](#AssignedTask "https://glaciation-project.eu/MetadataReferenceModel#AssignedTask") c

has range

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

### consumesEnergyFromop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#consumesEnergyFrom

The grid where a work producing resource consumes energy from

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[WorkProducingResource](#WorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource") c

has range

[Electrical Grid](#ElectricalGrid "https://glaciation-project.eu/MetadataReferenceModel#ElectricalGrid") c

### hasAspectop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasAspect

For keeping information about the Aspect of each Constraint, e.g., time, power consumption.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Constraint](#Constraint "https://glaciation-project.eu/MetadataReferenceModel#Constraint") c

has range

[Aspect](#Aspect "https://glaciation-project.eu/MetadataReferenceModel#Aspect") c

### hasCompositionop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasComposition

For keeping information about the Composition of the SoftConstraints of a Task.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

has range

[SoftConstraintComposition](#SoftConstraintComposition "https://glaciation-project.eu/MetadataReferenceModel#SoftConstraintComposition") c

### hasConstraintop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasConstraint

A relationship for recording all the Constraints of a Task.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

has range

[Constraint](#Constraint "https://glaciation-project.eu/MetadataReferenceModel#Constraint") c

### hasResourceMeasurementop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasResourceMeasurement

A relationship between a Resource and a Measurement.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

has range

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

### hasStatusop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasStatus

A relationship between any Class and its Status.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

has range

[Status](#Status "https://glaciation-project.eu/MetadataReferenceModel#Status") c

### hasSubResourceop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasSubResource

Relationships for recording the SubResource(s) of each Resource (e.g, the hardware of a node).

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

has range

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

### hasTaskMeasurementop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasTaskMeasurement

A relationship between a Task and a Measurement.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has sub-properties

[hasTaskPredictedMeasurement](#hasTaskPredictedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskPredictedMeasurement") op, [hasTaskRealizedMeasurement](#hasTaskRealizedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskRealizedMeasurement") op

has domain

[Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

has range

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

### hasTaskPredictedMeasurementop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasTaskPredictedMeasurement

A relationship for recording the PredictedMeasurements of a Task.

has super-properties

[hasTaskMeasurement](#hasTaskMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskMeasurement") op

has domain

[Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

has range

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

### hasTaskRealizedMeasurementop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasTaskRealizedMeasurement

A relationship for recording the RealizedMeasurements (actual measurements) of a Task.

has super-properties

[hasTaskMeasurement](#hasTaskMeasurement "https://glaciation-project.eu/MetadataReferenceModel#hasTaskMeasurement") op

has domain

[Task](#Task "https://glaciation-project.eu/MetadataReferenceModel#Task") c

has range

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

### isLocatedInop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#isLocatedIn

The location of a Work Producing Resource

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[WorkProducingResource](#WorkProducingResource "https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource") c

has range

[Site](#Site "https://glaciation-project.eu/MetadataReferenceModel#Site") c

### makesMeasurementop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#makesMeasurement

A relationship between a MeasuringResource and a Measurement.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[MeasuringResource](#MeasuringResource "https://glaciation-project.eu/MetadataReferenceModel#MeasuringResource") c

has range

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

### managesop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#manages

A relationship between a Scheduler and a Resource.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Scheduler](#Scheduler "https://glaciation-project.eu/MetadataReferenceModel#Scheduler") c

has range

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

### measuredInop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#measuredIn

For recording the MeasurimentUnit of each Measurement.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

has range

[MeasurementUnit](#MeasurementUnit "https://glaciation-project.eu/MetadataReferenceModel#MeasurementUnit") c

### monitorsop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#monitors

For recording which Monitor tracks an AssignedTask.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Monitor](#Monitor "https://glaciation-project.eu/MetadataReferenceModel#Monitor") c

has range

[AssignedTask](#AssignedTask "https://glaciation-project.eu/MetadataReferenceModel#AssignedTask") c

### producesop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#produces

For keeping information about the production Resource, e.g., the output, of an AssignedTask.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[AssignedTask](#AssignedTask "https://glaciation-project.eu/MetadataReferenceModel#AssignedTask") c

has range

[Resource](#Resource "https://glaciation-project.eu/MetadataReferenceModel#Resource") c

### relatesToConstraintop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#relatesToConstraint

For keeping information about the Constraint that each Measurement relates to.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

has range

[Constraint](#Constraint "https://glaciation-project.eu/MetadataReferenceModel#Constraint") c

### relatesToMeasurementPropertyop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#relatesToMeasurementProperty

For recording the MeasurementProperty of each Measurement.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

has range

[MeasurementProperty](#MeasurementProperty "https://glaciation-project.eu/MetadataReferenceModel#MeasurementProperty") c

### reschedulesop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#reschedules

A relationship between a Scheduler and an AssignedTask that concerns rescheduling.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Scheduler](#Scheduler "https://glaciation-project.eu/MetadataReferenceModel#Scheduler") c

has range

[AssignedTask](#AssignedTask "https://glaciation-project.eu/MetadataReferenceModel#AssignedTask") c

### scheduledByop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#scheduledBy

A relationship between a SubmittedTask and a Scheduler.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[SubmittedTask](#SubmittedTask "https://glaciation-project.eu/MetadataReferenceModel#SubmittedTask") c

has range

[Scheduler](#Scheduler "https://glaciation-project.eu/MetadataReferenceModel#Scheduler") c

### triggersRescheduleop back to [ToC](#toc) or [Object Property ToC](#objectproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#triggersReschedule

A triggered event relationship about Rescheduling from a Monitor.

has super-properties

[top Object Property](http://www.w3.org/2002/07/owl#topObjectProperty "http://www.w3.org/2002/07/owl#topObjectProperty") op

has domain

[Monitor](#Monitor "https://glaciation-project.eu/MetadataReferenceModel#Monitor") c

has range

[Scheduler](#Scheduler "https://glaciation-project.eu/MetadataReferenceModel#Scheduler") c

### Data Properties

*   [endingInterval](#endingInterval "https://glaciation-project.eu/MetadataReferenceModel#endingInterval")
*   [endTime](#endTime "https://glaciation-project.eu/MetadataReferenceModel#endTime")
*   [hasAggregatedFuntion](#hasAggregatedFuntion "https://glaciation-project.eu/MetadataReferenceModel#hasAggregatedFuntion")
*   [hasConfiguration](#hasConfiguration "https://glaciation-project.eu/MetadataReferenceModel#hasConfiguration")
*   [hasDescription](#hasDescription "https://glaciation-project.eu/MetadataReferenceModel#hasDescription")
*   [hasID](#hasID "https://glaciation-project.eu/MetadataReferenceModel#hasID")
*   [hasTimestamp](#hasTimestamp "https://glaciation-project.eu/MetadataReferenceModel#hasTimestamp")
*   [hasValue](#hasValue "https://glaciation-project.eu/MetadataReferenceModel#hasValue")
*   [startingInterval](#startingInterval "https://glaciation-project.eu/MetadataReferenceModel#startingInterval")
*   [startTime](#startTime "https://glaciation-project.eu/MetadataReferenceModel#startTime")
*   [statusCode](#statusCode "https://glaciation-project.eu/MetadataReferenceModel#statusCode")
*   [timeStepResolution](#timeStepResolution "https://glaciation-project.eu/MetadataReferenceModel#timeStepResolution")

### endingIntervaldp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#endingInterval

The ending interval time of an AggregatedMeasurement.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[AggregatedMeasurement](#AggregatedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#AggregatedMeasurement") c

has range

[date Time Stamp](http://www.w3.org/2001/XMLSchema#dateTimeStamp "http://www.w3.org/2001/XMLSchema#dateTimeStamp")

### endTimedp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#endTime

The end time of a Status of any Class.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[Status](#Status "https://glaciation-project.eu/MetadataReferenceModel#Status") c

has range

[date Time Stamp](http://www.w3.org/2001/XMLSchema#dateTimeStamp "http://www.w3.org/2001/XMLSchema#dateTimeStamp")

### hasAggregatedFuntiondp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasAggregatedFuntion

The AggregatedFunction of an AggregatedMeasurement.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[AggregatedMeasurement](#AggregatedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#AggregatedMeasurement") c

has range

[string](http://www.w3.org/2001/XMLSchema#string "http://www.w3.org/2001/XMLSchema#string")

### hasConfigurationdp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasConfiguration

The Configuration of any instance of a Class, e.g., Task, Resource, etc.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

has range

[string](http://www.w3.org/2001/XMLSchema#string "http://www.w3.org/2001/XMLSchema#string")

### hasDescriptiondp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasDescription

The Description of any entity.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

has range

[string](http://www.w3.org/2001/XMLSchema#string "http://www.w3.org/2001/XMLSchema#string")

### hasIDdp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasID

The ID of any entity.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[Class](#Class "https://glaciation-project.eu/MetadataReferenceModel#Class") c

has range

[string](http://www.w3.org/2001/XMLSchema#string "http://www.w3.org/2001/XMLSchema#string")

### hasTimestampdp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasTimestamp

The date and time of a Measurement.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

has range

[date Time Stamp](http://www.w3.org/2001/XMLSchema#dateTimeStamp "http://www.w3.org/2001/XMLSchema#dateTimeStamp")

### hasValuedp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#hasValue

The Value of a Measurement.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[Measurement](#Measurement "https://glaciation-project.eu/MetadataReferenceModel#Measurement") c

has range

[string](http://www.w3.org/2001/XMLSchema#string "http://www.w3.org/2001/XMLSchema#string")

### startingIntervaldp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#startingInterval

The starting interval time of an AggregatedMeasurement.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[AggregatedMeasurement](#AggregatedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#AggregatedMeasurement") c

has range

[date Time Stamp](http://www.w3.org/2001/XMLSchema#dateTimeStamp "http://www.w3.org/2001/XMLSchema#dateTimeStamp")

### startTimedp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#startTime

The date and time of a Status.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[Status](#Status "https://glaciation-project.eu/MetadataReferenceModel#Status") c

has range

[date Time Stamp](http://www.w3.org/2001/XMLSchema#dateTimeStamp "http://www.w3.org/2001/XMLSchema#dateTimeStamp")

### statusCodedp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#statusCode

The status code of a Status.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[Status](#Status "https://glaciation-project.eu/MetadataReferenceModel#Status") c

has range

[integer](http://www.w3.org/2001/XMLSchema#integer "http://www.w3.org/2001/XMLSchema#integer")

### timeStepResolutiondp back to [ToC](#toc) or [Data Property ToC](#dataproperties)

**IRI:** https://glaciation-project.eu/MetadataReferenceModel#timeStepResolution

The time step resolution of an AggregatedMeasurement.

has super-properties

[top Data Property](http://www.w3.org/2002/07/owl#topDataProperty "http://www.w3.org/2002/07/owl#topDataProperty") dp

has domain

[AggregatedMeasurement](#AggregatedMeasurement "https://glaciation-project.eu/MetadataReferenceModel#AggregatedMeasurement") c

has range

[string](http://www.w3.org/2001/XMLSchema#string "http://www.w3.org/2001/XMLSchema#string")

### Annotation Properties

*   [abstract](#http://purl.org/dc/terms/abstract "http://purl.org/dc/terms/abstract")
*   [contributor](#http://purl.org/dc/elements/1.1/contributor "http://purl.org/dc/elements/1.1/contributor")
*   [created](#http://purl.org/dc/terms/created "http://purl.org/dc/terms/created")
*   [creator](#http://purl.org/dc/elements/1.1/creator "http://purl.org/dc/elements/1.1/creator")
*   [description](#http://purl.org/dc/terms/description "http://purl.org/dc/terms/description")
*   [issued](#http://purl.org/dc/elements/1.1/issued "http://purl.org/dc/elements/1.1/issued")
*   [license](#http://purl.org/dc/terms/license "http://purl.org/dc/terms/license")
*   [preferred Namespace Uri](#http://purl.org/vocab/vann/preferredNamespaceUri "http://purl.org/vocab/vann/preferredNamespaceUri")
*   [preffered Namespace Prefix](#http://purl.org/vocab/vann/prefferedNamespacePrefix "http://purl.org/vocab/vann/prefferedNamespacePrefix")
*   [status](#http://purl.org/ontology/bibo/status "http://purl.org/ontology/bibo/status")
*   [title](#http://purl.org/dc/terms/title "http://purl.org/dc/terms/title")

### abstractap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/dc/terms/abstract

### contributorap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/dc/elements/1.1/contributor

### createdap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/dc/terms/created

### creatorap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/dc/elements/1.1/creator

### descriptionap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/dc/terms/description

### issuedap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/dc/elements/1.1/issued

### licenseap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/dc/terms/license

### preferred Namespace Uriap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/vocab/vann/preferredNamespaceUri

### preffered Namespace Prefixap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/vocab/vann/prefferedNamespacePrefix

### statusap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/ontology/bibo/status

### titleap back to [ToC](#toc) or [Annotation Property ToC](#annotationproperties)

**IRI:** http://purl.org/dc/terms/title

Legend back to [ToC](#toc)
--------------------------

c: Classes  
op: Object Properties  
dp: Data Properties  

Changes from last version
-------------------------

### Classes

Added classes

*   [https://glaciation-project.eu/MetadataReferenceModel#ElectricalGrid](#ElectricalGrid)
    *   Added: SubClass of https://glaciation-project.eu/MetadataReferenceModel#EnergyResource
*   [https://glaciation-project.eu/MetadataReferenceModel#EnergyPowerGenerationResource](#EnergyPowerGenerationResource)
    *   Added: SubClass of https://glaciation-project.eu/MetadataReferenceModel#EnergyResource
*   [https://glaciation-project.eu/MetadataReferenceModel#EnergyResource](#EnergyResource)
    *   Added: SubClass of https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource
*   [https://glaciation-project.eu/MetadataReferenceModel#Site](#Site)
    *   Added: SubClass of https://glaciation-project.eu/MetadataReferenceModel#Class

### Object Properties

Added object properties

*   [https://glaciation-project.eu/MetadataReferenceModel#consumesEnergyFrom](#consumesEnergyFrom)
    *   Added: Range https://glaciation-project.eu/MetadataReferenceModel#ElectricalGrid
    *   Added: domain https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource
    *   Added: SubProperty of http://www.w3.org/2002/07/owl#topObjectProperty
*   [https://glaciation-project.eu/MetadataReferenceModel#isLocatedIn](#isLocatedIn)
    *   Added: Range https://glaciation-project.eu/MetadataReferenceModel#Site
    *   Added: domain https://glaciation-project.eu/MetadataReferenceModel#WorkProducingResource
    *   Added: SubProperty of http://www.w3.org/2002/07/owl#topObjectProperty

Acknowledgments back to [ToC](#toc)
-----------------------------------

The authors would like to thank [Silvio Peroni](http://www.essepuntato.it/) for developing [LODE](http://www.essepuntato.it/lode), a Live OWL Documentation Environment, which is used for representing the Cross Referencing Section of this document and [Daniel Garijo](https://w3id.org/people/dgarijo) for developing [Widoco](https://github.com/dgarijo/Widoco), the program used to create the template used in this documentation.
