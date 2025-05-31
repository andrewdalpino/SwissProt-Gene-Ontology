# SwissProt Gene Ontology Dataset

This is a snapshot of the SwissProt dataset with gene ontology (GO) term annotations scraped from the Uniprot API. It is a raw and unfiltered dataset that can be processed to build datasets for protein function prediction.

## Subsets

The SwissProt Gene Ontology dataset is available on HuggingFace Hub and can be loaded using the HuggingFace [Datasets](https://huggingface.co/docs/datasets) library. 

The dataset is divided into three subsets according to the GO terms that the sequences are annotated with.

- `all` - All annotations
- `mf` - Only molecular function terms
- `cc` - Only celluar component terms
- `bp` - Only biological process terms

To load the default SwissProt Gene Ontology dataset with all function annotations you can use the example below.

```python
from datasets import load_dataset

dataset = load_dataset("andrewdalpino/SwissProt-Gene-Ontology")
```

To load a subset of the SwissProt Gene Ontology dataset use the example below.

```python
dataset = load_dataset("andrewdalpino/SwissProt-Gene-Ontology", "mf")
```

## References

>- The UniProt Consortium, UniProt: the Universal Protein Knowledgebase in 2025, Nucleic Acids Research, 2025, 53, D609–D617.