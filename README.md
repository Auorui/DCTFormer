# DCTFormer
DCTFormer

Due to the length of the paper, we have abandoned some experimental demonstrations, but we have provided the complete experimental content in our Github repository


### Ablation Study

### Loss Function Ablation Study
Our loss ablation study was initially built upon the L1 + Contrast loss.
By further incorporating the frequency loss and systematically ablating each component, we observe that the L1 + Frequency combination consistently outperforms other variants.
In contrast, adding the contrast loss leads to noticeable performance degradation, indicating that contrast enhancement objectives may be incompatible with accurate restoration in dehazing scenarios.
| L1 Loss | Frequency | Contrast | PSNR / SSIM |
|:-------:|:---------:|:--------:|:-----------:|
| ✓ | ✗ | ✗ | 25.68 / 0.860 |
| ✗ | ✓ | ✗ | 25.56 / 0.867 |
| ✓ | ✓ | ✗ | **26.06 / 0.870** |
| ✓ | ✗ | ✓ | 24.99 / 0.844 |
| ✓ | ✓ | ✓ | 25.49 / 0.863 |



