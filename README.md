# VL-model-for-ultrasound
## A Multi-Task Ultrasound Image Analysis Model by Vision-language Co-training

Recent progress on vision language deep learning models, such as DALL·E 2 and GPT-4, demonstrates great potential for co-training on large-scale multimodal data. However, the application of deep learning to ultrasound images is currently limited to training one model tailored to a specific dataset. Directly combining two datasets which represent different distributions can confuse the model. To address this challenge, we propose a new approach that employs prompt embeddings to condition the model. This work also aims to present a user-friendlier human-computer interaction framework for ultrasound image analysis, where users can prompt the machine to perform various tasks through text inputs.

Our proposed model is capable of conducting segmentation and classification simultaneously for different datasets, with comparable or superior performance (see Figure below). This is achieved by introducing user text inputs, for instance, "Please segment and classify breast cancer", along with the corresponding image. In this scheme, we learn $p_\theta(x_i|c_i)$, instead of $p_\theta(x_i)$, where $x$ represents input data, $c$ represents prompts, and $\theta$ denotes model parameters to optimize.

## Demo
- [demo video](https://youtu.be/XDzBTuoFlx4)
- [demo web](https://9d69db583109df4062.gradio.live)
