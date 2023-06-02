# stable-diffusion-colab-notebook




## Colab

| install | Info - Model Page
| --- | --- |

[![Install In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/wujun4code/stable-diffusion-colab-notebook/blob/main/chilloutmix/chillout_mix_webui_colab.ipynb) | [HuggingFace chilloutmix-ni](https://huggingface.co/swl-models/chilloutmix-ni/blob/main/chilloutmix-Ni.safetensors)

## extra Lora

```
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/amornlnw7/koreanDollLikeness_v15/resolve/main/koreanDollLikeness_v15.safetensors -d /content/stable-diffusion-webui/models/Lora/ -o koreanDollLikeness_v15.safetensors
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

## add api 

```
--api --cors-allow-origins-regex="https?://((localhost|127\.0\.0\.1|192\.168\.\d+\.\d+):\d+|aipromptor\.(com|org|app))"
```