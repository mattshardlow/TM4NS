# Corpus Sample

Each sentence is annotated in brat format. For each sentence, there are 2 files '.ann' and '.txt'. 
 - The '.txt' file contains the text in ASCII format. 
 - The '.ann' file contains the annotations according to the brat format. 
 
Full specification of the brat format is given here: http://brat.nlplab.org/standoff.html
 
Corpus specific annotation details are below:

Each .ann file contains one line per annotation. Each line is a tab separated entry with three fields. The first field contains an identifier for the term. The second field contains information specifying the term. The third field contains the text that the annotation covers.

The second field has 3 subfields, separated by spaces. The first subfield is a category identifier, labelling the annotation as a specific type from our schema. The next 2 subfields are the begin and end indices, expressed as character offsets in the '.txt' file.

An example is given below:

  T1    Ionic_Current 82 94    leak current

 - T1            is the term identifier (field 1)
 - Ionic_Current is the category identifier (field 2, subfield 1)
 - 82            is the begin index of the annotation (field 2, subfield 2)
 - 94            is the end index of the annotation (field 2, subfield 3)
 - leak current  is the text of the annotation (field 3)

A list of all potential category identifiers if given below:
- Brain_Region
- Neuron
- Species
- Ionic_Channel
- Ionic_Conductance
- Ionic_Current
- Units
- Experimental_Value
