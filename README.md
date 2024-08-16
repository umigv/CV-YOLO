# CV-YOLO
UMARV Computer Vision Team for development and reseearch of applying YOLO (You Only Look Once) to segment and detect objects and areas of interest.

Prerequisites:
- Completed Onboarding project
- Understanding of what ViTs are: Understanding [this](https://www.youtube.com/watch?v=NetSJM590Lo) video should be good enough. This is an important step and will make this project so much easier to understand and work through
- (Optional) PyTorch experience will help with most of this project. Some parts it is not necessary like part 3 below so if you want you may start there and begin to learn PyTorch in parallel

Rules:
- There is a linked project under the project tabs that is to be used to document tasks. Please mark tasks accuractely based on their actual status to avoid confusion and allow for effecient asynchronous work. Thank you
- Meet the Prerequisites before beggining work on the project


# Places to Start
1. Start from scratch and copy, adjust or develop architecture in PyTorch/TensorFlow (Advanced)
   <ol type="a">
     <li>The traditional ones: MaskFormer, SegFormer, and SAM</li>
     <li>[TransUNet](https://github.com/Beckschen/TransUNet)</li>
     <li>[SETR (SEgmentation TRansformer)](https://github.com/fudan-zvg/SETR)</li>
     <li>So many others are available and not just githubs either. If you are looking for a larger challenge and interested in diving into the architecture specifics, each of these models generally has a paper and a github that implements it. So although I have linked the githubs that apply the architectures already, you are free to read the paper and try it yourself!</li>
   </ol>
2. Fine-Tune an existing model given our lack of data
   <ol type="a">
     <li>[EffecientViT](https://github.com/mit-han-lab/efficientvit): Should definitley try this one extensively becasue it is already benchmarked on our exact hardware</li>
     <li>[SegViT](https://github.com/zbwxp/SegVit)</li>
     <li>Many others as well</li>
   </ol>
3. Use a HuggingFace or other service to almost completly abstract the implementation
   <ol type="a">
     <li>[Hugging Face ViT Intro](https://huggingface.co/learn/computer-vision-course/en/unit3/vision-transformers/vision-transformers-for-image-segmentation)</li>
   </ol>


# Things to Consider
1. Large amounts of data are needed to train ViTs from scratch. Looks for opportunites to fine-tune existing models or use transfer learning
2. The Sim can be used to artificially gather large amounts of data
3. Large AV datasets can also be used here to create a general model that we can gather our necessary data from
4. The Jetson can be used to train more intensive models. We may also be able to use the Great Lakes Computing Cluster
5. This team should also investigate the application of semi/un-supervisied learning
