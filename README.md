# Public Release Dataset

This directory contains the subset of the human evaluation data prepared for public sharing.

## Source and Citation

This public release is derived from the Earnings2Insights shared task dataset published at
https://sigfintech.github.io/fineval.html. When using the dataset, please cite the official
overview paper:

```bibtex
@inproceedings{takayanagi2025earnings2insights,
  title     = "{Earnings2Insights: Analyst Report Generation for Investment Guidance}",
  author    = "Takehiro Takayanagi and Tomas Goldsack and Kiyoshi Izumi and Chenghua Lin and Hiroya Takamura and Chung-Chi Chen",
  booktitle = "Proceedings of the FinNLP Workshop at EMNLP 2025",
  year      = "2025",
  address   = "Suzhou, China",
  url       = "https://sigfintech.github.io/fineval.html",
  note      = "Overview paper for the Earnings2Insights shared task (FinEval) at FinNLP 2025"
}
```

## Files

- `wide_data_public.csv`: Aggregated evaluation responses with financial decision targets
  and review metadata. 

## Columns

- `Clarity`: Likert rating of how clear the generated report is.
- `Freecomment`: Free-form evaluator comment for the report.
- `Logic`: Likert rating of logical soundness.
- `Persuasiveness`: Likert rating of persuasive strength.
- `Readability`: Likert rating of readability.
- `Usefulness`: Likert rating of usefulness for decision making.
- `doc_id`: Identifier for the evaluated document.
- `financial_decision_day`: Next-day trading signal annotated by the evaluator.
- `financial_decision_month`: Next-month trading signal annotated by the evaluator.
- `financial_decision_week`: Next-week trading signal annotated by the evaluator.
- `day_label`: Model-provided next-day directional label where `1` = up and `-1` = down.
- `week_label`: Model-provided next-week directional label where `1` = up and `-1` = down.
- `month_label`: Model-provided next-month directional label where `1` = up and `-1` = down.
- `generated_report`: Text of the generated report reviewed by participants.
- `team_id`: Identifier for the evaluation team.
- `company_id`: Identifier for the underlying company.
- `company_name`: Name of the underlying company.

## License and Privacy

Review the originating datasets for any privacy or licensing constraints before further
sharing. Remove rows that contain sensitive information not intended for public release.
