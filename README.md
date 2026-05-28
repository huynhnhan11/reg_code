# Kaggle Notebooks

Generated from `uit/uit-train/entrypoints/tier*.py`.

Files:

- `tier1_spikingbert_impldiff_kaggle.ipynb`
- `tier2_variant_a_logit_kd_kaggle.ipynb`
- `tier2_variant_b_feature_stage2_kaggle.ipynb`
- `tier2_variant_c_full_twostage_kaggle.ipynb`
- `tier3_hybrid_impldiff_kaggle.ipynb`

Kaggle setup:

- Enable GPU.
- Upload UIT-VSFC so the notebook can find either `/kaggle/input/<dataset-name>/uit-vsfc` or `/kaggle/input/<dataset-name>`.
- Upload the fine-tuned teacher checkpoint so the notebook can find either `/kaggle/input/<model-dataset-name>/phobert_vsfc/best_model.pth` or `/kaggle/input/<model-dataset-name>/best_model.pth`.
- In Cell 3, replace `<dataset-name>` and `<model-dataset-name>` if auto-detection does not find them.
- Run the default dry-run first.
- Set `RUN_FULL = True` in Cell 12 only after dry-run succeeds.
- Keep `RUN_STAGE1_OPTIONAL = False` unless intentionally running optional Wikipedia Stage 1.

##Link to...
- Checkpoint of teacher "phobert-vsfc models" : https://drive.google.com/drive/folders/1Y7WaX44iyYyslC9OvLEabc7Tf1Mak0WO?usp=sharing
- wiki_dataset: https://drive.google.com/drive/folders/18BoI313y_r-ResTl6vD5MN_UerGEXPKI?usp=sharing
