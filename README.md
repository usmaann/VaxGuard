# VaxGuard
## **Data for "VaxGuard: A Multi-Generator, Multi-Type, and Multi-Role Dataset for Detecting LLM-Generated Vaccine Misinformation"**

## Detailed Distribution of VaxGuard Dataset — Roles, Vaccine Types, and Generators

| Class           | Role                          | Vaccine Type | GPT-3.5 | GPT-4o | LLaMA3 | PHI3 | Mistral | Total Samples |
|----------------|-------------------------------|--------------|---------|--------|--------|------|---------|----------------|
| Misinformation | Misinformation Spreader       | COVID        | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                |                               | HPV          | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                |                               | Influenza    | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                | Religious Conspiracy Theorist | COVID        | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                |                               | HPV          | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                |                               | Influenza    | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                | Fear Monger                   | COVID        | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                |                               | HPV          | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                |                               | Influenza    | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                | Anti-Vacciner                 | COVID        | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                |                               | HPV          | 500     | 500    | 500    | 500  | 500     | 2,500          |
|                |                               | Influenza    | 500     | 500    | 500    | 500  | 500     | 2,500          |
| Otherwise      | N/A                           | COVID        | 2,000   | 2,000  | 2,000  | 2000 | 2000    | 10,000         |
|                |                               | HPV          | 2,000   | 2,000  | 2,000  | 2000 | 2000    | 10,000         |
|                |                               | Influenza    | 2,000   | 2,000  | 2,000  | 2000 | 2000    | 10,000         |
| **Total**      | **All Roles**                 | **All Vaccine Types** | **12,000** | **12,000** | **12,000** | **12,000** | **12,000** | **60,000** |



## Example Text from VaxGuard Dataset

| Role                         | Generated Misinformation                                                                                                                                                                                                                                                                                                                                 | Keywords                        |
|-----------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------------------|
| Misinformation Spreader     | COVID-19 vaccines contain a small amount of toxic chemicals that can harm your DNA and cause long-term damage to your body. The vaccine makers are more interested in making money than in protecting public health, and they’re hiding the truth about the real risks associated with these injections.                                                     | Trials, Testing, Vaccination, Clinical |
| Religious Conspiracy Theorist | According to ancient scriptures such as Bhagavad Gita, purity of body is achieved without medical intervention; hence natural immunity should suffice against diseases like HPV-related cervical cancer instead of relying on modern vaccines created through unholy scientific practices.                                                                 | Help, Studies, Clinical, Use    |
| Anti Vacciner               | Influenza vaccines contain harmful chemicals that can weaken the immune system and make individuals more susceptible to other illnesses.                                                                                                                                                                                                                   | Regulatory, Agencies, Testing, Use |
| Fear Monger                | New York City hospitals have reported an alarming increase in miscarriages among pregnant women who received COVID-19 vaccines, a clear indication of the dangers these shots pose to unborn babies. This disturbing trend highlights the need for caution when considering vaccination during pregnancy.                                                  | Accurately, Clinical, Safety, Drug |

## How to use the Data Set
The dataset is provided in the data directory. Each file is a CSV named using the pattern
{VaccineType}_{LLM}_{Role}.csv (for example, COVID19_GPT-3.5_FearMonger.csv).
To use the dataset, download or copy the required CSV files from this folder and load them into your analysis environment

## Citation

If you use this dataset in your research, please cite:

```bibtex
@misc{ahmad2025vaxguardmultigeneratormultitypemultirole,
  title={VaxGuard: A Multi-Generator, Multi-Type, and Multi-Role Dataset for Detecting LLM-Generated Vaccine Misinformation},
  author={Syed Talal Ahmad and Haohui Lu and Sidong Liu and Annie Lau and Amin Beheshti and Mark Dras and Usman Naseem},
  year={2025},
  eprint={2503.09103},
  archivePrefix={arXiv},
  primaryClass={cs.CL},
  url={https://arxiv.org/abs/2503.09103}
}
