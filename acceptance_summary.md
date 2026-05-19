# Task Type Classifier Acceptance Summary

## 1. Overall Results

| dataset | label_set | size | accuracy | macro_f1 | weighted_f1 | macro_recall | error_rate | low_confidence_count | close_margin_count |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| hard | core6 | 240 | 0.9917 | 0.9916 | 0.9916 | 0.9917 | 0.0083 | 1 | 2 |
| boundary | core6 | 80 | 0.9250 | 0.9382 | 0.9244 | 0.9500 | 0.0750 | 2 | 2 |
| realistic | core6 | 3577 | 0.5921 | 0.6360 | 0.5839 | 0.6158 | 0.4079 | 981 | 876 |

## 2. Notes

- For `--label-set core6`, `light_trouble` is mapped to `practical_help` in gold labels and predictions.
- If the model payload contains class_multipliers / rule_override settings, this script uses the training script's `predict_with_options` when available.
- Check `errors.csv`, `low_confidence.csv`, and `close_margin.csv` inside each dataset folder.
