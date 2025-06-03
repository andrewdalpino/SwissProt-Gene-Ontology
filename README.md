# SwissProt Gene Ontology Dataset

This is a snapshot of the SwissProt dataset with gene ontology (GO) term annotations scraped from the UniProt API. It is a raw and unfiltered dataset that can be processed to build datasets for protein function prediction.

## Example Usage

To load the default SwissProt Gene Ontology dataset using HuggingFace Datasets refer to the example below.

```python
from datasets import load_dataset

dataset = load_dataset("andrewdalpino/SwissProt-Gene-Ontology")
```

## References

>- The UniProt Consortium, UniProt: the Universal Protein Knowledgebase in 2025, Nucleic Acids Research, 2025, 53, D609–D617.