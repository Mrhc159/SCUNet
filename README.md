Codes
---------
1. Download SCUNet models
```python
python main_models.py --models "SCUNet" --model_dir "model_zoo"
```

2. Gaussian denoising
    1. grayscale images

    ```bash
    python main_test_scunet_gray_gaussian.py --model_name scunet_gray_25 --noise_level_img 25 --testset_name set12
    ```

    2. color images
    ```bash
    python main_test_scunet_color_gaussian.py --model_name scunet_color_25 --noise_level_img 25 --testset_name bsd68
    ```
3. Blind real image denoising

    ```bash
    python main_test_scunet_real_application.py --model_name scunet_color_real_psnr --testset_name real3
    ```
    ```bash
    python main_test_scunet_real_application.py --model_name scunet_color_real_gan --testset_name real3
    ```

