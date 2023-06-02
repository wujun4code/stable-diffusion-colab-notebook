# stable-diffusion-colab-notebook




## Colab

| install | Info - Model Page
| --- | --- |

[![Install In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wujun4code/stable-diffusion-colab-notebook/blob/main/chillout_mix_webui_colab.ipynb) | [HuggingFace chilloutmix-ni](https://huggingface.co/swl-models/chilloutmix-ni/blob/main/chilloutmix-Ni.safetensors)

## extra Lora

```
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://civitai.com/api/download/models/31284 -d /content/stable-diffusion-webui/models/Lora/ -o koreanDollLikeness_v20.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/aimainia/japaneseDollLikeness_v10/resolve/main/japaneseDollLikeness_v10.safetensors -d /content/stable-diffusion-webui/models/Lora/ -o japaneseDollLikeness_v10.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/opsopus/taiwanDollLikeness/resolve/main/taiwanDollLikeness_v10.safetensors -d /content/stable-diffusion-webui/models/Lora/ -o taiwanDollLikeness_v10.safetensors

!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://civitai.com/api/download/models/21077 -d /content/stable-diffusion-webui/models/Lora -o breastinclassBetter_v13.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://civitai.com/api/download/models/16557 -d /content/stable-diffusion-webui/models/Lora -o shojovibe_v11.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://civitai.com/api/download/models/18117 -d /content/stable-diffusion-webui/models/Lora -o realisticVaginasAsian_asianpussy1V1.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://civitai.com/api/download/models/11371 -d /content/stable-diffusion-webui/models/Lora -o LORARealRefinedPussy_pussy10.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://civitai.com/api/download/models/16677 -d /content/stable-diffusion-webui/models/Lora -o cuteGirlMix4_v10.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://civitai.com/api/download/models/20745 -d /content/stable-diffusion-webui/models/Lora -o chineseQingchunGirl.safetensors
```

## replace Chillout-mix model 

```
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/swl-models/chilloutmix-ni/resolve/main/chilloutmix-Ni.safetensors -d /content/stable-diffusion-webui/models/Stable-diffusion -o chilloutmix-Ni.safetensors

```

## extra models

```
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/yesyeahvh/ulzzang-6500/resolve/main/ulzzang-6500.pt -d /content/stable-diffusion-webui/embeddings -o ulzzang-6500.pt
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/datasets/Nerfgun3/bad_prompt/resolve/main/bad_prompt_version2.pt -d /content/stable-diffusion-webui/embeddings -o bad_prompt.pt
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://civitai.com/api/download/models/5119 -d /content/stable-diffusion-webui/embeddings -o pureerosface_v1.pt
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/stabilityai/sd-vae-ft-mse-original/resolve/main/vae-ft-mse-840000-ema-pruned.ckpt -d /content/stable-diffusion-webui/models/VAE -o vae-ft-mse-840000-ema-pruned.ckpt
```

## add api 

```
--api --cors-allow-origins-regex="https?://((localhost|127\.0\.0\.1|192\.168\.\d+\.\d+):\d+|aipromptor\.(com|org|app))"
```