## SLAIF AI Vision Toolbox by ViCoS
This is the public repository of the AI Vision Toolbox made by [ViCoS](https://vicos.si/) for [SLAIF](https://slaif.si/). It is distributed by 

### Development
The toolbox is validated and developed on a linux-based operating system running an nvidia gpu[^1].

Docker is used for bundling everything together. To build the image, run:
```bash
docker build -t toolbox-slaif \
    --build-arg "TOOLBOX_BRAND_NAME_LONG=SLAIF AI Vision Toolbox by ViCoS" \
    --build-arg "TOOLBOX_BRAND_NAME_SHORT=SLAIF Toolbox" \
    --build-context branding=https://github.com/vicoslab/toolbox-slaif.git \
    https://github.com/vicoslab/toolbox.git
```

[^1]: NixOS 26.05, Intel i7-14700K, 32GB DDR5, Nvidia RTX 3060