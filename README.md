# DALLE-reproduction
This repository is for sharing pre-trained [OpenAI DALLE](https://openai.com/blog/dall-e/) model and generating images from given texts.

All models are trained by [lucidrains/DALLE-pytorch](https://github.com/lucidrains/DALLE-pytorch) + [VQGAN (Taming transformer)](https://github.com/CompVis/taming-transformers) with different training code and BPE model.

If you want to train DALLE, please go to [lucidrains/DALLE-pytorch](https://github.com/lucidrains/DALLE-pytorch) and support them to reproduce better DALLE models ✈️

### The notebook includes
#### 1. Text to image generation

#### 2. Pre-trained CLIP reranking
- CUB200

<img src="./images/cub_reranking.png" width="700px"></img>

- COCO

<img src="./images/coco_reranking.png" width="700px"></img>

#### 3. Generate rest of image based on the given cropped image
- CUB200

<img src="./images/cub_cropped.png" width="700px"></img>

- COCO

<img src="./images/coco_cropped.png" width="700px"></img>

## Usage
1. Install requirements
```
$ pip install -r requirements
```

2. Install DeepSpeed
- Follow the instruction [here](https://github.com/lucidrains/DALLE-pytorch#deepspeed-sparse-attention) and install DeepSpeed

### Models
- Download models below and save them in *pretrained* folder
- Check the link in *Details* for the model specifics

Dataset | Download | Password | Optimizer | Size | Details
-- | -- | -- | -- | -- | --
CUB200 | [link](https://dubox.com/s/1cBrzsPZ9WeBZ47OMlZV9rw) | v9ge | Adam | 1.1GB | [link](https://github.com/lucidrains/DALLE-pytorch/discussions/131#discussion-3296648)
CUB200 | [link](https://dubox.com/s/1e3RTwdWYsKcs4RtKATfQNg) | 47w1 | AdamW | 1.1GB | [link](https://github.com/lucidrains/DALLE-pytorch/discussions/139#discussioncomment-560790)
COCO | [link](https://dubox.com/s/1dbJSCyoQdPVQLJb2rxEvKg) | p3ki | Adam | 1.5GB | [link](https://github.com/lucidrains/DALLE-pytorch/discussions/181)
